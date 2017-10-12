---
TOCTitle: Active Directory Hizmet Bulmayı Geçersiz Kılma
Title: Active Directory Hizmet Bulmayı Geçersiz Kılma
ms:assetid: '9d97e7fb-5b05-4853-ad7b-6cc82b9729f0'
ms:contentKeyID: 18125217
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747614(v=WS.10)'
---

Active Directory Hizmet Bulmayı Geçersiz Kılma
==============================================

RMS hizmetleri ve istemcileri hizmet konumlarını ilk olarak yerel kayıt defterine bakara bulurlar. Kayıt defterinde belirli anahtarların değeri yoksa, RMS hizmetleri ve istemcileri Active Directory'de hizmet bağlantı noktası (SCP) arar. Sunucu veya istemci kayıt defterine belirli anahtarlar yazarsanız, varsayılan Active Directory bulma ayarını geçersiz kılabileceğiniz anlamına gelir.

| ![](images/Cc747614.note(WS.10).gif)Not                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS kök kümeniz yapılandırılmışsa ve bu yüzden SCP Active Directory'de yayımlanmayacaksa, RMS istemcilerinizin doğru konuma yönlendirmek için bu anahtarları kullanabilirsiniz. |

Bu bölüm kayıt defteri anahtarlarını tanımlar ve bunları nasıl oluşturabileceğiniz hakkında ayrıntı verir.

Yalnızca Lisans Küme Alt Kaydı için Hizmet Bulmayı Geçersiz Kılma
-----------------------------------------------------------------

Yalnızca lisans sağlayıcı küme sağlıyorsanız ve lisans sağlayıcı kümenin Active Directory ormanında dağıttığınızdan farklı bir kök kümesine alt kayıt yaptırmak istiyorsanız, hem alt kayıt hem de hesap sertifika hizmetlerini de geçersiz kılmanız gerekir.

#### Kayıt defteri girdi açıklamaları

Aşağıdaki kayıt defteri girişleri alt kayıt ve hesap sertifika hizmetlerini geçersiz kılmak için kullanılır.

-   **SubEnrollmentURL**. Bu girdi lisans sunucusunun sunucu lisans sertifikası isterken kullandığı kök kümesinin yolunu belirtir.
-   **GicURL**. Bu girdi bu yalnızca lisans sağlayıcı kümenin hesap sertifika hizmetine olan yolu belirtir.

#### Girdi ayrıntıları

Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda, yalnızca lisans sağlayıcı küme alt kaydı için hizmet bulmaya ait tam kayıt defteri alt anahtar yolu şöyledir:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda, yalnızca lisans sağlayıcı küme alt kaydı için hizmet bulmaya ait tam kayıt defteri alt anahtar yolu şöyledir:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

Aşağıdaki tablo hizmet bulmayı geçersiz kılmak için ekleyebileceğiniz girdileri listeler.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Tür</th>
<th style="border:1px solid black;" >Değer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SubEnrollmentURL</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">http(veya https)://<em>sunucu_adı</em>/_wmcs/certification/subenrollservice.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GicURL</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">http(veya https)://<em>sunucu_adı</em>/_wmcs/certification/certification.asmx</td>
</tr>
</tbody>
</table>
  
Yayımlama için İstemci Tarafı Hizmet Bulmayı Geçersiz Kılma  
-----------------------------------------------------------
  
Kullanıcılarınız kendi bilgisayarlarından içerik yayımlıyorlarsa, kuruluşunuzda kullanılan topolojiye göre yayımlama için kullanılan sunucu konumlarını geçersiz kılmak isteyebilirsiniz. Yayımlama için kullanılan sunucuların konumları normalde Active Directory kullanılarak bulunur. İstemci bilgisayarlara uygun kayıt defteri anahtarlarını ekleyerek, istemciler bu yöntemleri atlar ve bunun yerine kayıt defteri girdi değerinde belirttiğiniz URL adreslerini kullanır.
  
| ![](images/Cc747614.note(WS.10).gif)Not                                                                                                                                  |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| İstemcinin bu bölümlerde listelenenleri geçersiz kılacakları ayrı girdiler olarak değil anahtar olarak oluşturulmalıdır. Bu anahtarların değeri her anahtarın varsayılan girdisinde oluşturulmalıdır. |
  
#### Kayıt defteri anahtarı açıklamaları
  
RMS kümesinin otomatik bulunmasını geçersiz kılmak için aşağıdaki kayıt defteri anahtarları kullanılabilir.
  
-   **Activation**. Bu kayıt defteri anahtarı makine etkinleştirme hizmetinin URL adresini tanımlar. RMS Service Pack 1 veya daha yeni bir istemcisi çalıştırıyorsanız, bu kayıt defteri girdisi artık kullanılmaz.  
-   **EnterprisePublishing**. Bu kayıt defteri anahtarı, bu istemcinin lisans istekleri için kullanacağı RMS yüklemesinin URL adresini tanımlar.  
-   **CloudPublishing**. Bu kayıt defteri anahtarı, istemcinin RMS yüklemesine erişimi yok ancak Internet'e erişimi varsa kullanabileceği, Microsoft'un işlettiği lisans hizmetinin URL adresini tanımlar.
  
#### Anahtar ayrıntıları
  
Yayımlama için istemci tarafı hizmet bulma kayıt defteri alt anahtarını tam yolu şöyledir:
  
**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\MSDRM\\ServiceLocation\\**
  
Aşağıdaki tablo hizmet bulmayı geçersiz kılmak için RMS istemcisine ekleyebileceğiniz kayıt defteri anahtarlarını listeler.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Tür</th>
<th style="border:1px solid black;" >Değer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Activation</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">http(veya https)://<em>RMS_küme_adı</em>/_wmcs/Certification burada <em>RMS_küme_adı</em> RMS kümenizin adıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">EnterprisePublishing</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">http(veya https)://<em>RMS_küme_adı</em>/_wmcs/Licensing burada <em>RMS_küme_adı</em> RMS kümenizin adıdır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CloudPublishing</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">http(veya https)://<em>FQDN_küme_adı</em>/_wmcs/Licensing burada <em>FQDN_küme_adı</em> is RMS kümenizin tam etki alanı adıdır .</td>
</tr>
</tbody>
</table>
  
Bu kayıt defteri anahtarlarının uygulanmasını, kuruluşunuzdaki tüm istemcilerin doğru yayımlama sunucularının kullandığından emin olmak için Systems Management Server veya Grup İlkesi aracılığıyla yapmanızı öneririz.
  
| ![](images/Cc747614.Caution(WS.10).gif)Dikkat                                                                                                             |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Kayıt defterinin hatalı düzenlenmesi, sisteminize ciddi bir hasar verebilir. Kayıt defterinizde değişiklik yapmadan önce, bilgisayarınızdaki önemli verilerin tümünü yedeklemelisiniz. |
  
RMS kümesindeki her sunucuda doğru kayıt defterleri anahtarlarını almak için örnek bir kayıt defteri dosyası (.reg) kullanılabilir.
  
**RMS kümesindeki her sunucuda doğru kayıt defteri anahtarlarını almak için**  
1.  Aşağıdaki kayıt defteri dosyasını Not Defteri içine kopyalayın.
  
    `Windows Registry Editor Version 5.00`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation]`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\Activation]`
  
    `@="http://<RMS_cluster_name>/_wmcs/certification"`
  
    `[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\MSDRM\ServiceLocation\EnterprisePublishing]`
  
    `@="http://<RMS_cluster_name>/_wmcs/licensing"`
  
2.  &lt;RMS\_küme\_adı&gt; değerini RMS kümenizin adıyla değiştirin.
  
3.  Dosyayı .reg dosya adı uzantısıyla kaydedin.
  
4.  Dosyanın adını Windows Gezgini'nde çift tıklatın.
  
5.  **Kullanıcı Hesabı Denetimi** iletişim kutusu görüntülenirse, görüntülenen eylemin kullanmak istediğiniz eylem olduğunu doğrulayın ve sonra da **Devam**'ı tıklatın.. Bilgileri kayıt defterine eklemek isteyip istemediğinizi sorulduğunda, **Evet**'i tıklatın.
