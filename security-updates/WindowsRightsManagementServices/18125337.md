---
TOCTitle: RMS Hesap Sertifikası Hizmeti
Title: RMS Hesap Sertifikası Hizmeti
ms:assetid: 'fb294969-850e-44b4-8f6a-ca5d5cec1bf1'
ms:contentKeyID: 18125337
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747802(v=WS.10)'
---

RMS Hesap Sertifikası Hizmeti
=============================

Hesap sertifikası hizmeti yalnızca kök kümesinde çalışır. Hesap sertifikası hizmeti kullanıcı hesaplarını belirli bilgisayarlarla ilişkilendiren hak hesabı sertifikalarını oluşturur. Hak hesabı sertifikası bir kullanıcının belirli bir bilgisayarı kullanırken haklarla korunan içerik yayımlamasına veya kullanmasına olanak tanır.

Hesap sertifikası hizmeti uygulama dosyası Certification.asmx, IIS içindeki Certification sanal dizininde bulunur.

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
