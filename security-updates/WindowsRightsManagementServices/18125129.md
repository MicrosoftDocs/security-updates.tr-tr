---
TOCTitle: RMS Etkinleştirme Proxy Hizmeti
Title: RMS Etkinleştirme Proxy Hizmeti
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18125129
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747608(v=WS.10)'
---

RMS Etkinleştirme Proxy Hizmeti
===============================

Tüm RMS sürüm 1.0 makine etkinleştirme istekleri, yalnızca RMS kök kümesinde çalışan etkinleştirme proxy hizmeti aracılığıyla gönderilir. Haklarla korunan içerik yayımlamak veya kullanmak üzere RMS ile kullanılabilmesi için, önce istemci bilgisayarı etkinleştirmeniz gerekir. RMS Service Pack 1'den itibaren, istemci “kendini etkinleştirir”; kasa ve makine sertifikası oluşturmak için etkinleştirme proxy sunucusunu veya Microsoft Etkinleştirme Hizmeti'ni kullanması gerekmez.

Etkinleştirme proxy hizmeti, RMS sürüm 1.0 istemcilerinden gelen makine etkinleştirme isteklerini Microsoft Etkinleştirme Hizmeti'ne iletir ve bu hizmet de ilgili kullanıcı ve bilgisayar için benzersiz olan özel olarak oluşturulan bir kasa ve bununla eşleşen bir RMS makine sertifikası döndürür. Etkinleştirme proxy hizmeti, daha sonra bu öğeleri istekte bulunan istemciye iletir.

Etkinleştirme proxy hizmeti uygulama dosyası Activation.asmx, IIS içindeki Certification sanal dizininde bulunur. Bu hizmetteki varsayılan erişim denetim listesi aşağıdaki tabloda gösterilmektedir:

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
<td style="border:1px solid black;">Guests</td>
<td style="border:1px solid black;">Okuma ve Yürütme</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS Service Group</td>
<td style="border:1px solid black;">Okuma ve Yürütme</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Tam Denetim</td>
</tr>
</tbody>
</table>
