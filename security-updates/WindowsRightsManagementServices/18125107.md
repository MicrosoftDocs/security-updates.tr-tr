---
TOCTitle: RMS Lisans Hizmeti
Title: RMS Lisans Hizmeti
ms:assetid: '5cad1baf-0304-4e82-b62d-83a4aac2140b'
ms:contentKeyID: 18125107
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720278(v=WS.10)'
---

RMS Lisans Hizmeti
==================

Kullanım lisanslarını yayımlayan lisans hizmeti, herhangi bir lisans sunucusunda çalışabildiği gibi RMS kök kümesinde de çalışır. Kullanım lisansları kullanıcıların haklarla korunan içeriği kullanmasına olanak tanır.

Lisans hizmeti uygulama dosyası License.asmx, IIS içindeki Licensing sanal dizininde bulunur.

| ![](/security-updates/images/Cc720278.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kök kümesinden gelen lisans istekleri yükünü azaltmak için ayrı bir lisans kümesi dağıtabilirsiniz. Örneğin şirketinizdeki bir bölümün kendi hak ilkelerini oluşturmasını sağlamak üzere söz konusu bölüm için ayrı lisans sunucusu veya kümesi de dağıtabilirsiniz. Bu değerlendirmeler hakkında daha fazla bilgi için, bu belge grubundaki "RMS: Planlama ve Mimari" bölümünde bulunan “Çekirdek Bileşenleri Belirleme” konusuna bakın. |

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
