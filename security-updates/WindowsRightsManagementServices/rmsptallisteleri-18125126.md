---
TOCTitle: RMS İptal Listeleri
Title: RMS İptal Listeleri
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18125126
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720287(v=WS.10)'
---

RMS İptal Listeleri
===================

İptal listeleri; iptal edilmiş içerik, uygulama, kullanıcı veya diğer asıl öğeleri belirtir. Kuruluş bir varlığı iptal listesine aşağıdaki bir veya birkaç nedenle koyar:

-   Özel bir anahtarın güvenlik tehlikesi oluşturduğu bilinmekte veya bundan kuşkulanılmaktadır.
-   Anahtar sahibi, güvenlik tehlikesi oluşturduğuna inandığı bir anahtarın iptalini ister.
-   Sorumlu artık geçerli değildir (örneğin bir çalışan işten çıkarılmıştır).
-   Güvenlik açığı vardır (örneğin istemci bilgisayara verilen bir sertifika güvenlik tehlikesi oluşturmaktadır).
-   Yetki değişikliği nedeniyle yeni sertifika gereklidir.
-   RMS etkin bir uygulamadaki güvenlik açıkları, uygulamanın çok önemli veya korumalı içeriği kullanmak üzere uygun olmamasına neden olur.
-   Daha önceden dağıtılan bir içerik bölümü artık eskidir veya kullanıma uygun değildir.

Aşağıdaki tabloda, bir iptal listesinde belirtebileceğiniz varlıklar, bu varlıkları tanımlamak için kullanılan bilgilerle birlikte açıklanmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Varlık</th>
<th style="border:1px solid black;" >Tanıtıcı</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Bir lisans veya sertifika grubu</td>
<td style="border:1px solid black;">Verenin kimliği veya ortak anahtarı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bir uygulama bildirimleri grubu</td>
<td style="border:1px solid black;">Verenin kimliği veya ortak anahtarı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Belirli bir lisans veya sertifika</td>
<td style="border:1px solid black;">Lisans kimliği veya karması</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Belirli bir uygulama bildirimi</td>
<td style="border:1px solid black;">Lisans kimliği veya karması</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Belirli bir sorumlu</td>
<td style="border:1px solid black;">Sorumlu kimliği veya ortak anahtarı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Belirli bir içerik bölümü</td>
<td style="border:1px solid black;">İçerik kimliği</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| İptal ve dışlama için tüm karma değerleri, Güvenli Karma Algoritması'nın (SHA) bir düzeltmesi olan ve Güvenli Karma Standardı'nda (SHS, FIPS 180) belirtilen SHA-1'dir \[NIS94c\]. SHA-1, ANSI X9.30 (bölüm 2) standardında açıklanmaktadır. Uygulama bildirimiyle iptal etmek için sertifika verenin kimliğini, sertifika verenin ortak anahtarını, lisans kimliğini veya lisans karma değerini uygulama bildiriminden ayıklamanız gerekir. Bununla birlikte, uygulama bildirimleri taban 64 kodlamasıyla şifrelenmiştir; bu nedenle bilgilere düz metin biçiminde erişilemez. Uygulama bildiriminin şifresini çözmek ve gerekli bilgileri almak için, Rights Management Client SDK ile **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** ve **DRMDecode** yöntemleri kullanılarak bir program geliştirilebilir. Belirli bir uygulamanın RMS korumalı içeriği kullanmasını engellemek istiyorsanız, RMS sunucusunun bu uygulamalara kullanım lisansı vermesini engellemek için uygulama dışlama özelliğini kullanmayı düşünün. Dışlama ile ilgili kısıtlama, geçerli kullanım lisansına sahip birinin RMS korumalı içeriğin şifresini çözmeyi engelleyememesidir. Uygulama dışlama hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan Uygulamaları Dışlama konusuna bakın. |
  
İptal listeleri, aşağıdaki parametreleri belirten XrML dosyalarıdır.
  
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
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">XrML dosyasının oluşturulduğu sistem saati. Bu, kullanım lisansındaki REFRESH koşulu tarafından, iptal listesinin ömrünü belirlemek için kullanılır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">İptal listesini verenin adı, kimliği ve adresi.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">İptal listesi yayıncısının ortak anahtarı.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">İptal edilen varlığın adı, türü ve kimliği.</td>
</tr>
</tbody>
</table>
