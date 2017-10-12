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

| ![](images/Cc720208.Important(WS.10).gif)Önemli                                                       |
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

| ![](images/Cc720208.note(WS.10).gif)Not                                                    |
|-------------------------------------------------------------------------------------------------------------------------|
        ```
| ![](images/Cc720208.Caution(WS.10).gif)Dikkat                                             |
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

<span id="BKMK_2"></span>
#### Sertifikaları ve Lisansları GUID'ye Göre İptal Etme

        ```
#### Uygulama bildirimiyle iptal etme

Uygulama bildirimiyle iptal etmek için sertifika verenin kimliğini, sertifika verenin ortak anahtarını, lisans kimliğini veya lisans karma değerini uygulama bildiriminden ayıklamanız gerekir. Bununla birlikte, uygulama bildirimleri base 64 kodludur; bu nedenle düz metinde bilgilere erişilemez. Rights Management Services Software Development Kit (SDK) ile; DRMConstructCertificateChain, DRMDeconstructCertificateChain ve DRMDecode yöntemlerini kullanarak uygulama bildiriminin şifresini çözmek ve gerekli bilgileri almak için bir program geliştirilebilir.

Belirli bir uygulamanın telif haklı içeriği kullanmasını engellemek istiyorsanız, RMS kümesinin bu uygulamalara kullanım lisansı vermesini engellemek için uygulama dışlama özelliğini kullanmayı düşünün. Dışlama ile ilgili kısıtlama, geçerli kullanım lisansına sahip birinin haklarla korunan içeriğin şifresini çözmeyi engelleyememesidir. Uygulamayı dışlama hakkında daha fazla bilgi için bu konuda daha önce geçen [Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) bölümüne bakın.

<span id="BKMK_3"></span>
#### Sertifikaları ve Lisansları Karma Değerine Göre İptal Etme

        ```
#### Uygulama bildirimiyle iptal etme

Uygulama bildirimiyle iptal etmek için sertifika verenin kimliğini, sertifika verenin ortak anahtarını, lisans kimliğini veya lisans karma değerini uygulama bildiriminden ayıklamanız gerekir. Bununla birlikte, uygulama bildirimleri base 64 kodludur; bu nedenle düz metinde bilgilere erişilemez. Rights Management Services SDK ile; DRMConstructCertificateChain, DRMDeconstructCertificateChain ve DRMDecode yöntemlerini kullanarak uygulama bildiriminin şifresini çözmek ve gerekli bilgileri almak için bir program geliştirilebilir.

Belirli bir uygulamanın telif haklı içeriği kullanmasını engellemek istiyorsanız, RMS kümesinin bu uygulamalara kullanım lisansı vermesini engellemek için uygulama dışlama özelliğini kullanmayı düşünün. Dışlama ile ilgili kısıtlama, geçerli kullanım lisansına sahip birinin RMS korumalı içeriğin şifresini çözmeyi engelleyememesidir. Uygulamayı dışlama hakkında daha fazla bilgi için bu konuda daha önce geçen [Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86) bölümüne bakın.

<span id="BKMK_4"></span>
#### Sertifikaları ve Lisansları Verenin Ortak Anahtarına Göre İptal Etme

        ```

<span id="BKMK_5"></span>
#### Sertifikaları ve Lisansları Verenin Kimliğine Göre İptal Etme

        ```
| ![](images/Cc720208.note(WS.10).gif)Not                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, genel benzersiz tanımlayıcı (GUID) ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_6"></span>
#### İçeriği İçerik Kimliğine Göre İptal Etme

        ```
| ![](images/Cc720208.note(WS.10).gif)Not                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, genel benzersiz tanımlayıcı (GUID) ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_10"></span>
#### Sorumluları Windows hesabına göre iptal etme

        ```
| ![](images/Cc720208.note(WS.10).gif)Not                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir kimlik türü belirtirken, Windows hesabı SID'si ve kapatma etiketi arasında satırbaşı işareti olmadığından emin olun. Yanlışlıkla bir satırbaşı işareti eklenmişse, RMS istemcisi iptal listesini ayrıştıramaz. |

<span id="BKMK_7"></span>
#### Sorumluları Windows Live Kimliğine Göre İptal Etme

        ```
| ![](images/Cc720208.note(WS.10).gif)Not                                                                                                                                                               |
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

| ![](images/Cc720208.note(WS.10).gif)Not |
|----------------------------------------------------------------------|
| RLsigner.exe boşluk içeren dosya isimlerini desteklemez.             |

<span id="BKMK_9"></span>
RLsigner.exe kullanımı
----------------------

RLsigner.exe'yi çalıştırdığınız zaman, ilk önce anahtar dosyasında verilen özel anahtarı kullanarak bir imza oluşturur. Bunun ardından, sağladığınız iptal listesi dosyasına göre bir çıkış dosyası oluşturur.

| ![](images/Cc720208.Important(WS.10).gif)Önemli                        |
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
  
| ![](images/Cc720208.note(WS.10).gif)Not |  
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
  
<codesnippet asp="http://msdn2.microsoft.com/asp" language displaylanguage="Visual Basic">const EVT\_SUCCESS = 0 const EVT\_ERROR = 1 const EVT\_WARNING = 2 const EVT\_INFORMATION = 4 const EVT\_AUDIT\_SUCCESS = 8 const EVT\_AUDIT\_FAILURE = 16 Dim WshShell, oExec Set WshShell = CreateObject( "WScript.Shell" ) Set oExec = WshShell.Exec("rlsigner.exe input\_file key\_file output\_file") Do While oExec.Status = 0 WScript.Sleep 100 Loop if WshShell.ExitCode &lt;&gt; 0 Then WshShell.LogEvent EVT\_ERROR, "RLsigner failed with error """ + WshShell.ExitCode + """" else WshShell.LogEvent EVT\_SUCCESS, "RLsigner completed successfully" end if  
```
