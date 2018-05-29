---
TOCTitle: İptal Listeleri Oluşturma
Title: İptal Listeleri Oluşturma
ms:assetid: '1ef75199-3344-4225-84de-a863a777696a'
ms:contentKeyID: 18125025
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720208(v=WS.10)'
---

İptal Listeleri Oluşturma
=========================

İptal işlemini uygulama, Genişletilebilir Haklar Biçimlendirme Dili (XrML) kullanan XML belgesi olan bir iptal listesi dağıtmanızı gerektirir ve haklarla korunan içeriğe artık erişimi olmaması gereken sorumluların listesini verir. RMS ile birlikte verilen İptal Listesi İmzalama aracı (RLsigner.exe) kullanılarak zaman damgası vurulmuş ve uygun bir biçimde imzalanmış iptal listeleri oluşturmanız gerekir.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Önemli                                                       |
|------------------------------------------------------------------------------------------------------------------------------------|
| RLsigner.exe kullanarak iptal listesini imzalamak için, iptal listesi dosyasını bir unicode dosyası olarak kaydetmeniz gereklidir. |

İptal Listesi Örneği
--------------------

Bu konuda, her olası iptal mekanizmasını gösteren tam bir iptal listesi örneği sunulmaktadır. Bu örneği kendi iptal listelerinizi oluştururken model olarak kullanabilirsiniz.

İptal listesi XrML dili kullanan bir XML dosyasıdır.

BODY öğesi dört alt öğe içerir:

-   **ISSUEDTIME**. İptal listesinin verildiği tarih ve saati içerir. RLsigner.exe bu öğeyi dosyaya ekler. Bu öğe, örnekte yalnızca iptal listesi dosyasının genel yapısını göstermek amacıyla verilmiştir.
-   **DESCRIPTOR**. Dosyayı iptal listesi olarak tanımlayan verileri içerir.
-   **ISSUER**. İptal listesini veren varlığı tanıyan verileri içerir.
-   **REVOCATIONLIST**. Bu listenin iptal ettiği varlıkları belirten alt REVOKE öğelerini içerir.

Örnek bir iptal liste dosyası aşağıda gösterilmiştir.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not                                                    |
|-------------------------------------------------------------------------------------------------------------------------|
|ISSUEDTIME, PUBLICKEY ve SIGNATURE öğeleri RLsigner.exe tarafından ekleneceği veya üzerine yazılacağı için atlanabilir.|

```
<?xml version="1.0" ?> 
<XrML xml:space=”preserve” version=”1.2”>
  <BODY type="LICENSE" version="3.0">
    <ISSUEDTIME>...</ISSUEDTIME> 
    <DESCRIPTOR>
      <OBJECT type="Revocation-List">
        <ID type="MS-GUID">{d6373cba-01f1-4f32-ac58-260f580af0f8}</ID>
      </OBJECT>
    </DESCRIPTOR>
<ISSUER>
      <OBJECT type="Revocation-List">
        <ID type="acsii-tag">External revocation authority</ID>
        <NAME>Revocation list name</NAME>
        <ADDRESS type="URL">https://somedomain.com/revocation_list_file</ADDRESS>
      </OBJECT>
      <PUBLICKEY>...</PUBLICKEY>
    </ISSUER>
  <REVOCATIONLIST>
    <REVOKE>...<\REVOKE>
    <REVOKE>...<\REVOKE>
  </REVOCATIONLIST>
  <SIGNATURE>...</SIGNATURE>
</XrML>
```
        
| ![](/security-updates/images/Cc720208.Caution(WS.10).gif)Dikkat                                             |
|------------------------------------------------------------------------------------------------------------------------|
| İptal listesinde URL'yi belirtirken, RMS SP1 veya RMS SP2 içinde artık UNC yolu desteklenmez. Bir URL kullanmalısınız. |

REVOKE öğelerini tanımlamanızdan sonra, iptal listesi imzalanmaya hazır hale gelir.

REVOKE Öğesini Kullanma
-----------------------

İptal Listesi Örneği bölümündeki örnek iptal listesinde her REVOKE öğesi kaldırılacak bir sorumluyu belirtir. Açılış etiketinde iptal edilenin ne olduğunu ve hangi ölçütle iptal edildiğini tanımlayan category ve type öznitelikleri vardır. Farklı REVOKE öğeleri, category ve type öznitelikleriyle belirlenen eyleme göre farklı alt öğelere sahiptir.

REVOKE öğeleri hakkında daha fazla bilgi için aşağıdaki örneklere bakın:

-   [Sorumluları Ortak Anahtara Göre İptal Etme](#bkmk_1)
-   [Sertifikaları ve Lisansları GUID'ye Göre İptal Etme](#bkmk_2)
-   [Sertifikaları ve Lisansları Karma Değerine Göre İptal Etme](#bkmk_3)
-   [Sertifikaları ve Lisansları Verenin Ortak Anahtarına Göre İptal Etme](#bkmk_4)
-   [Sertifikaları ve Lisansları Verenin Kimliğine Göre İptal Etme](#bkmk_5)
-   [İçeriği İçerik Kimliğine Göre İptal Etme](#bkmk_6)
-   [Sertifikaları Sorumlu Kimliğine Göre İptal Etme](#bkmk_10)
-   [Sorumluları Windows Live Kimliğine Göre İptal Etme](#bkmk_7)

<span id="BKMK_1"></span>
#### Sorumluları Ortak Anahtara Göre İptal Etme

```
              <REVOKE category="principal" type="principal-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
6Jn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_2"></span>
#### Sertifikaları ve Lisansları GUID'ye Göre İptal Etme

```
<REVOKE category="license" type="license-id">
        <OBJECT>
          <ID type="MS-GUID">{06BCB94D-43E5-419f-B180-AA9FD321ED7A}</ID>
        </OBJECT>
      </REVOKE>
```

#### Uygulama bildirimiyle iptal etme

Uygulama bildirimiyle iptal etmek için sertifika verenin kimliğini, sertifika verenin ortak anahtarını, lisans kimliğini veya lisans karma değerini uygulama bildiriminden ayıklamanız gerekir. Bununla birlikte, uygulama bildirimleri base 64 kodludur; bu nedenle düz metinde bilgilere erişilemez. Rights Management Services Software Development Kit (SDK) ile; DRMConstructCertificateChain, DRMDeconstructCertificateChain ve DRMDecode yöntemlerini kullanarak uygulama bildiriminin şifresini çözmek ve gerekli bilgileri almak için bir program geliştirilebilir.

Belirli bir uygulamanın telif haklı içeriği kullanmasını engellemek istiyorsanız, RMS kümesinin bu uygulamalara kullanım lisansı vermesini engellemek için uygulama dışlama özelliğini kullanmayı düşünün. Dışlama ile ilgili kısıtlama, geçerli kullanım lisansına sahip birinin haklarla korunan içeriğin şifresini çözmeyi engelleyememesidir. Uygulamayı dışlama hakkında daha fazla bilgi için bu konuda daha önce geçen [Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) bölümüne bakın.

<span id="BKMK_3"></span>
#### Sertifikaları ve Lisansları Karma Değerine Göre İptal Etme

```
<REVOKE category="license" type="license-hash">
        <DIGEST>
          <ALGORITHM>SHA1</ALGORITHM>
          <VALUE encoding="base64" size="160">
            ABfB4mcEslVCMEZR9reACqXHCoQ=
          </VALUE>
        </DIGEST>
      </REVOKE>
```

#### Uygulama bildirimiyle iptal etme

Uygulama bildirimiyle iptal etmek için sertifika verenin kimliğini, sertifika verenin ortak anahtarını, lisans kimliğini veya lisans karma değerini uygulama bildiriminden ayıklamanız gerekir. Bununla birlikte, uygulama bildirimleri base 64 kodludur; bu nedenle düz metinde bilgilere erişilemez. Rights Management Services SDK ile; DRMConstructCertificateChain, DRMDeconstructCertificateChain ve DRMDecode yöntemlerini kullanarak uygulama bildiriminin şifresini çözmek ve gerekli bilgileri almak için bir program geliştirilebilir.

Belirli bir uygulamanın telif haklı içeriği kullanmasını engellemek istiyorsanız, RMS kümesinin bu uygulamalara kullanım lisansı vermesini engellemek için uygulama dışlama özelliğini kullanmayı düşünün. Dışlama ile ilgili kısıtlama, geçerli kullanım lisansına sahip birinin RMS korumalı içeriğin şifresini çözmeyi engelleyememesidir. Uygulamayı dışlama hakkında daha fazla bilgi için bu konuda daha önce geçen [Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) bölümüne bakın.

<span id="BKMK_4"></span>
#### Sertifikaları ve Lisansları Verenin Ortak Anahtarına Göre İptal Etme

```
<REVOKE category="license" type="issuer-key">
        <PUBLICKEY>
          <ALGORITHM>RSA-1024</ALGORITHM>
          <PARAMETER name="public exponent">
            <VALUE encoding="integer32">65537</VALUE>
          </PARAMETER>
          <PARAMETER name="modulus">
            <VALUE encoding="base64" size="1024">
AAn0kEAWU+1AFWtuUmBYL8Jza8tLhUv/BCmgcq/Pc08Au3DvXkH65s+0MEyZjM+71j3F1xaXUSst+wH2FjApkY1RxgL8VAKIuEvIy9hRrvY1YhJx/0Ite5fZeg2crUFrmoQgZzaJ50FvoakA2QMgZZgxoQmwiGE0y40cEJtIlE0=
            </VALUE>
          </PARAMETER>
        </PUBLICKEY>
      </REVOKE>
```

<span id="BKMK_5"></span>
#### Sertifikaları ve Lisansları Verenin Kimliğine Göre İptal Etme

```
      <REVOKE category="license" type="issuer-id">
        <OBJECT type="MS-DRM-Server">
          <ID type="MS-GUID">{2BE9E200-3040-41B9-8832-D4D0445EBBD6}</ID> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, genel benzersiz tanımlayıcı (GUID) ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_6"></span>
#### İçeriği İçerik Kimliğine Göre İptal Etme

```
<REVOKE category="content" type="content-id">
        <OBJECT type="Microsoft Office Document">
          <ID type="MS-GUID">{8702641D-3512-4AA4-A584-84C703A5B5C0}</ID>
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, genel benzersiz tanımlayıcı (GUID) ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_10"></span>
#### Sorumluları Windows hesabına göre iptal etme

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Windows">{Windows account SID}</ID> 
          <NAME>{E-mail address}</NAME> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, Windows hesabı SID'si ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_7"></span>
#### Sorumluları Windows Live Kimliğine Göre İptal Etme

```
<REVOKE category="principal" type="principal-id">
        <OBJECT type="Group-Identity">
          <ID type="Passport">{PUID}</ID> 
          <NAME>michael@contoso.com</NAME> 
        </OBJECT>
      </REVOKE>
```

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not                                                                                                                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, asıl öğe benzersiz tanımlayıcı (PUID) ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_8"></span>
İptal Listesine İmza Ekleme
---------------------------

İptal listesi oluşturmayı bitirdiğiniz zaman, iptal listesine bu başlıkta açıklandığı gibi bir imza eklemeniz gerekir. Bunun ardından, ilişkili hak ilkesi şablonunda belirttiğiniz URL veya UNC yolundaki iptal listesini kullanıcıların kullanımına sunabilirsiniz.

İmza eklemek için ilk adım, Sağlam Ad aracını (Sn.exe) kullanarak bir anahtar çifti ve anahtar dosyası üretmektir. Sn.exe aracı ([http://go.microsoft.com/fwlink/?LinkId=104796](http://go.microsoft.com/fwlink/?linkid=104796) (http://www.microsoft.com/) Microsoft Web sitesinde bulabileceğiniz .NET Framework SDK 1.1'de bulunmaktadır.

İptal listesi dosyasının RLsigner.exe kullanılarak imzalanabilmesi için bir unicode dosyası olarak kaydedilmesi gereklidir

**Sn.exe aracını yeni bir anahtar çifti üretmek ve bu çifti bir dosyaya yazmak üzere kullanmak için**
1.  Özel anahtarı oluşturun. Komut istemine aşağıdaki komutu yazın ve ENTER tuşuna basın:

    **sn -k** *özel\_anahtar\_dosyası***.snk**

    burada *özel\_anahtar\_dosyası* anahtar dosyasının adıdır.

2.  1. Adımda oluşturulan anahtar çiftinden ortak anahtarı ayıklamak ve ayrı bir dosyaya vermek için Sn.exe'yi kullanın. Aşağıdaki komutu yazın ve ENTER tuşuna basın:

    **sn -p** *özel\_anahtar\_dosyası ortak\_anahtar\_dosyası*

    burada *özel\_anahtar\_dosyası* 1. Adımda oluşturulan özel anahtar dosyasının adıdır ve *ortak\_anahtar\_dosyası* ortak anahtarın verildiği dosyanın adıdır.

3.  Özel anahtar dosyasının uzantısını (1. Adım'da oluşturulan) RLsigner.exe ile kullanmak için .snk'den .dat'a dönüştürün.

4.  İptal listesi dosyasına bir imza eklemek için RLsigner.exe aracını kullanın. Bu araç, RMS içinde bulunmaktadır. Varsayılan olarak, %systemdrive%\\Program Files\\Windows Rights Management Services\\Tools dizinindedir.

| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not |
|----------------------------------------------------------------------|
| RLsigner.exe boşluk içeren dosya isimlerini desteklemez.             |

<span id="BKMK_9"></span>
RLsigner.exe kullanımı
----------------------

RLsigner.exe'yi çalıştırdığınız zaman, ilk önce anahtar dosyasında verilen özel anahtarı kullanarak bir imza oluşturur. Bunun ardından, sağladığınız iptal listesi dosyasına göre bir çıkış dosyası oluşturur.

| ![](/security-updates/images/Cc720208.Important(WS.10).gif)Önemli                        |
|-----------------------------------------------------------------------------------------------------|
| İptal listesi dosyası RLsigner.exe ile kullanmak için unicode dosyası olarak kaydedilmiş olmalıdır. |

İptal listesini imzalamak amacıyla RLsigner.exe kullanmak için komut istemine aşağıdaki komutu yazın:

**rlsigner.exe** *giriş\_dosyası* **{-f** *anahtar\_dosyası* **| -h** *kapsayıcı\_adı* **CSP}** *çıkış\_dosyası*

Komutun giriş parametrelerini tamamlamak için aşağıdaki bilgileri kullanın:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametre</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><em>giriş_dosyası</em></td>
<td style="border:1px solid black;">Hazırlamış olduğunuz XrML uyumlu iptal listesi dosyasının adıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>anahtar_dosyası</em></td>
<td style="border:1px solid black;">Üretmiş olduğunuz ortak ve özel anahtarları içeren dosyanın adıdır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>kapsayıcı_adı</em></td>
<td style="border:1px solid black;">Anahtar kapsayıcısının adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>çıkış_dosyası</em></td>
<td style="border:1px solid black;">Aracın oluşturacağı imzalı iptal listesi dosyasının adıdır.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc720208.note(WS.10).gif)Not |  
|----------------------------------------------------------------------|  
| RLsigner.exe boşluk içeren dosya isimlerini desteklemez.             |
  
Aşağıdaki örnekler, RLsigner.exe aracını bir komut satırında farklı şifreleme hizmeti sağlayıcılarıyla nasıl kullanabileceğinizi açıklamaktadır:
  
-   Bir anahtar dosyası kullanan örnek komut satırı sözdizimi:  
    **rlsigner.exe rl.xml -f anahtar.dat çıkış.xml**  
-   Bir donanım güvenlik modülü kullanan örnek komut dosyası sözdizimi:  
    **rlsigner.exe rl.xml -h Kapsayıcı CSP çıkış.xml**
  
RLsigner.exe dönüş kodunda temel hata ve başarı bilgileri sağlar. Aşağıdaki tabloda olası dönüş kodları açıklanmaktadır.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Dönüş Kodu</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">Başarı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-1</td>
<td style="border:1px solid black;">Kaynak dosya okunamıyor</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-2</td>
<td style="border:1px solid black;">Anahtar dosyası okunamıyor</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-3</td>
<td style="border:1px solid black;">Geçersiz anahtar dosyası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-4</td>
<td style="border:1px solid black;">Geçersiz kaynak dosya</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">-5</td>
<td style="border:1px solid black;">Çıkış dosyasına yazılamıyor</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">-6</td>
<td style="border:1px solid black;">Bilinmeyen hata</td>
</tr>
</tbody>
</table>
  
İptal listelerinin imzalanmasını sunucunuz için belirttiğiniz yenileme aralığına göre zamanlayabilirsiniz.
  
İptal listesi imzalama işlemini komut dosyası kullanarak otomatikleştirebilirsiniz. Aşağıdaki örnek VBScript, RLsigner.exe aracını çağırır ve sonuçları Sistem olay günlüğüne yazar
  
```VB
const EVT_SUCCESS       = 0
const EVT_ERROR         = 1
const EVT_WARNING       = 2
const EVT_INFORMATION   = 4
const EVT_AUDIT_SUCCESS = 8
const EVT_AUDIT_FAILURE = 16

Dim WshShell, oExec

Set WshShell = CreateObject( "WScript.Shell" )
Set oExec = WshShell.Exec("rlsigner.exe input_file key_file output_file")
Do While oExec.Status = 0
     WScript.Sleep 100
Loop

if WshShell.ExitCode <> 0 Then
    WshShell.LogEvent EVT_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """"
else
    WshShell.LogEvent EVT_SUCCESS, "RLsigner completed successfully"
end if
```
