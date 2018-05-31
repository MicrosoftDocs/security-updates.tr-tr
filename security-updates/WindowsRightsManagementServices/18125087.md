---
TOCTitle: RMS Yayımlama Hizmeti
Title: RMS Yayımlama Hizmeti
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18125087
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720267(v=WS.10)'
---

RMS Yayımlama Hizmeti
=====================

Yayımlama lisanslarını veren yayımlama hizmeti, herhangi bir lisans sunucusunda çalışabildiği gibi RMS kök kümesinde de çalışır. Yayımlama lisansları, kullanım lisanslarını teslim etmek için kullanılabilecek ilkeyi tanımlar.

Yayımlama hizmeti uygulama dosyası Publish.asmx, IIS içindeki Licensing sanal dizininde bulunur.

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
