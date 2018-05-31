---
TOCTitle: RMS Hizmet Bulma Hizmeti
Title: RMS Hizmet Bulma Hizmeti
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18125256
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747548(v=WS.10)'
---

RMS Hizmet Bulma Hizmeti
========================

Hizmet Bulma hizmeti hem RMS kökünde hem de lisans sunucularında çalışır. Hizmet Bulma hizmeti, RMS etkin istemciler tarafından bulunabilmesi için Active Directory'ye kümenin hizmet bağlantı URL'sini sağlar.

Hizmet bulma hizmeti uygulama dosyası ServiceLocator.asmx, IIS içindeki Certification ve Licensing sanal dizinlerinde bulunur.

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
<td style="border:1px solid black;">Administrators</td>
<td style="border:1px solid black;">Tam Denetim</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS Service Group</td>
<td style="border:1px solid black;">Okuma ve Yürütme</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Tam Denetim</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Users</td>
<td style="border:1px solid black;">Okuma ve Yürütme</td>
</tr>
</tbody>
</table>
