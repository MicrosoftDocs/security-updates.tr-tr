---
TOCTitle: RMS Anahtar Tanımları
Title: RMS Anahtar Tanımları
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18125238
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747729(v=WS.10)'
---

RMS Anahtar Tanımları
=====================

Aşağıdaki tabloda bir RMS sisteminde kullanılan anahtarlar listelenmiştir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Anahtar</th>
<th style="border:1px solid black;" >Kullanım</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Sunucu anahtarları</td>
<td style="border:1px solid black;"><strong>Ortak anahtar</strong>
Yalnızca RMS sunucusunun içerik anahtarını alabilmesi ve yayımlama lisansı için kullanım lisansları verebilmesi amacıyla, yayımlama lisansındaki içerik anahtarını şifreler.
<strong>Özel anahtar</strong>
Sunucu tarafından verilen tüm sertifika ve lisansları imzalar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Makine anahtarları</td>
<td style="border:1px solid black;"><strong>Ortak anahtar</strong>
Hak hesabı sertifikası özel anahtarını şifreler.
<strong>Özel anahtar</strong>
Hak hesabı sertifikasının şifresini çözer.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">İstemci lisans anahtarları</td>
<td style="border:1px solid black;"><strong>Ortak anahtar</strong>
Verdiği yayımlama lisanslarında bulunan simetrik içerik anahtarını şifreler.
<strong>Özel anahtar</strong>
Kullanıcı ağa bağlı değilken yerel olarak verilen yayımlama lisanslarını imzalar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kullanıcı anahtarları</td>
<td style="border:1px solid black;"><strong>Ortak anahtar</strong>
Yalnızca belirli bir kullanıcının bu lisansı kullanarak RMS korumalı içeriği kullanabilmesi için, bir kullanım lisansındaki içerik anahtarını şifreler.
<strong>Özel anahtar</strong>
Kullanıcıların RMS korumalı içeriği kullanmasına olanak tanır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">İçerik anahtarları</td>
<td style="border:1px solid black;">Yazar RMS korumalı içeriği yayımladığında, içeriği şifreler.</td>
</tr>
</tbody>
</table>
