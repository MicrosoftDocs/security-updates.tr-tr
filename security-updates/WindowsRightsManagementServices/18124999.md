---
TOCTitle: RMS Ön Sertifika Hizmeti
Title: RMS Ön Sertifika Hizmeti
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18124999
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720191(v=WS.10)'
---

RMS Ön Sertifika Hizmeti
========================

Ön sertifika hizmeti yalnızca RMS kök kümesinde çalışır. Bu hizmet bir sunucunun kullanıcı adına hak hesabı sertifikası isteğinde bulunmasına olanak tanır ve özel uygulamalar geliştirmek için kullanılabilir. Bu hizmeti kullanan uygulamalara örnek olarak Microsoft Exchange Server 2007 ve Microsoft Office SharePoint Server 2007 gösterilebilir.

Ön sertifika hizmeti uygulama dosyası Precertification.asmx, IIS içindeki Certification sanal dizininde bulunur.

Özel uygulamalar geliştirme konusunda daha fazla bilgi için, MSDN Kitaplığı'nda bulunan Windows Rights Management Services Technology Documentation belgelerine [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972) bakın.

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
