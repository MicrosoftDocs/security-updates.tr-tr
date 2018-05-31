---
TOCTitle: RMS Sunucu Hizmeti
Title: RMS Sunucu Hizmeti
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18125154
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747566(v=WS.10)'
---

RMS Sunucu Hizmeti
==================

Sunucu hizmeti yalnızca RMS kök kümesinde çalışır. Sunucu hizmeti, sunucu lisans sertifikası almak için bir istemci tarafından çevrimiçi yayımlama kullanılarak yapılan bir isteği kullanıma açar.

Sunucu hizmeti uygulama dosyası Server.asmx, IIS içindeki Certification sanal dizininde bulunur.

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
