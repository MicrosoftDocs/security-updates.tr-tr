---
TOCTitle: Sunucu Lisans Sertifikalarını Yönetme
Title: Sunucu Lisans Sertifikalarını Yönetme
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18125097
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720272(v=WS.10)'
---

Sunucu Lisans Sertifikalarını Yönetme
=====================================

Sunucu lisans sertifikalarının geçerliliği belirli bir süre sonunda, genellikle bir yıl sonra sona erer. Sunucu lisans sertifikasını yenilemek için yerel yönetici olarak oturum açmanız gerekir. Kök sertifika kümesinin sunucu lisans sertifikasını yenilediğinizde, RMS, Microsoft Kayıt Hizmeti'ne sunucu lisans sertifikasını yenileme isteği gönderir. Bir lisans sunucusunun sertifikasını yenilediğinizde, RMS yenileme isteğini geçerliliği sona ermiş sertifikayı yayınlayan kök sertifika sunucusuna gönderir.

RMS'nin Sistem olay günlüğüne işleyeceği, izlemeniz gereken üç olay vardır. Bu olaylar, sunucu lisans sertifikanızın yenilenme tarihi yaklaştığında veya geçerliliği sona erdiğinde sizi bilgilendirir. Aşağıdaki tabloda Olay kimlikleri ve adları liste halinde verilmiştir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Olay kimliği</th>
<th style="border:1px solid black;" >Olay Adı</th>
<th style="border:1px solid black;" >Olay Türü</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Uyarı Hizmet olağan çalışmasına devam eder.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Uyarı Hizmet olağan çalışmasına devam eder.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Hata. Hizmet devre dışı bırakıldı.</td>
</tr>
</tbody>
</table>
