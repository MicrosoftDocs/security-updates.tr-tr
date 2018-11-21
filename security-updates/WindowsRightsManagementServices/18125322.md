---
TOCTitle: RMS için Küme Gereksinimlerini Planlama
Title: RMS için Küme Gereksinimlerini Planlama
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18125322
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747792(v=WS.10)'
---

RMS için Küme Gereksinimlerini Planlama
=======================================

RMS'yi küme dağıtımında kullanıyorsanız, kuruluşunuzda olabilecek aşağıdaki durumları göz önünde bulundurduğunuzdan emin olun.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Koşul</th>
<th style="border:1px solid black;" >Öneri</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS'yi kullanan çok sayıda masaüstü.</td>
<td style="border:1px solid black;">Microsoft Windows Rights Management Services istemci yazılımını yüklemek ve etkinleştirmek için Windows Update, komut dosyası veya Systems Management Server (SMS) veya Grup İlkesi gibi bir yazılım dağıtım yöntemi kullanabilirsiniz.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Çok sayıda istemci isteği.</td>
<td style="border:1px solid black;">İstekleri küme içinde dağıtmak için yük dengeleme sunucusu, Ağ Yük Dengeleme (NLB) hizmeti veya donanım yük dengeleme özelliğini kullanın.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Extranet ve intranet isteklerine hizmet vermek için sanal IP adresleme kullanan iki ağ bağdaştırıcısı.</td>
<td style="border:1px solid black;">Sanal IP adresini extranet'e göstermek üzere yapılan DNS kaydının, adresi intranet'e göstermek için de yapıldığından emin olun.
Intranet için DNS kaydı yapılmazsa, iç kullanım lisansı istekleri başarısız olur. DNS kaynak kayıtlarını değiştiremiyorsanız, kümedeki her sunucunun hosts tablosunu, küme URL'si kümenin sanal IP adresiyle eşlenecek şekilde değiştirebilirsiniz. DNS kaydı, RMS sağlama işleminden önce yapılmalıdır. RMS'yi önceden sağladıysanız, geri almalı ve yeniden sağlamalısınız.</td>
</tr>
</tbody>
</table>
