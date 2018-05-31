---
TOCTitle: RMS Yetki Alma Hizmeti
Title: RMS Yetki Alma Hizmeti
ms:assetid: '97677e3b-bc83-47ec-b6db-d326cd94566c'
ms:contentKeyID: 18125210
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747695(v=WS.10)'
---

RMS Yetki Alma Hizmeti
======================

Yetki Alma hizmeti, RMS Kurulumu tarafından yüklenen özel bir Web hizmetidir. Hem kök kümesinde hem de lisans kümesinde çalışır. Bu hizmeti etkinleştirdiğinizde, sunucu üzerindeki tüm diğer RMS Web hizmetleri devre dışı kalır.

Bu hizmet, haklarla korunan içeriğin yayımlama lisansındaki içerik anahtarının şifresini çözer ve lisans isteği üzerine istemciye bu anahtarı sunar. Bu, içeriğin RMS koruması olmadan kaydedilebilmesini sağlar. Yetki alma hizmeti yapılan tüm istemci isteklerini günlüğe kaydeder ve günlük veritabanına kaydedilmek üzere günlük dinleyici hizmetine gönderir.

Yetki alma hizmetini Yönetim Web sitesindeki **Güvenlik ayarları** sayfasından etkinleştirebilirsiniz. Bu hizmeti etkinleştirdikten sonra, sunucuyu standart bir RMS yapılandırmasına geri yükleyemezsiniz.

Hizmeti etkinleştirdikten sonra, içeriklerini lisanslamak için bu sunucuyu kullanan kuruluşunuzdaki kullanıcılara erişim olanağı sağlamak için decommission.asmx dosyasının DACL'sini ayarlamalı ve RMS'nin işlemlerini yönetmesine olanak tanımak için RMS Service Group'u okuma ve yürütme izinleriyle DACL'ye eklemelisiniz. Bu sunucu tarafından yayımlanan içeriğin tümü korunmasız hale getirildikten sonra, özel anahtar bilgilerini yedeklemeniz ve ardından RMS'yi sunucudan kaldırmanız gerekir.

Bu hizmetteki varsayılan erişim denetim listesi aşağıdaki tabloda gösterilmektedir:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kullanıcı veya Grup</th>
<th style="border:1px solid black;" >Varsayılan İzin</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Tam Denetim</td>
</tr>
</tbody>
</table>
