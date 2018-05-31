---
TOCTitle: RMS Alt Kayıt Hizmeti
Title: RMS Alt Kayıt Hizmeti
ms:assetid: '6b05e71c-5e7d-467c-9e13-35ac14d3718a'
ms:contentKeyID: 18125124
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720289(v=WS.10)'
---

RMS Alt Kayıt Hizmeti
=====================

Alt kayıt hizmeti yalnızca RMS kök kümesinde çalışır. Sunucu lisans sertifikaları için lisans kümeleri tarafından sağlama sırasında gönderilen isteklere yanıt verir.

Alt kayıt hizmeti uygulama dosyası (SubEnrollService.asmx), Certification sanal dizininde *RMS\_Web\_Sitesi*\\\_wmcs\\Certification\\ konumunda depolanır; burada, *RMS\_Web\_Sitesi* RMS'yi sağladığınız Web sitesinin adıyla değiştirilir.

Varsayılan olarak, bu hizmete erişim yerel SYSTEM hesabıyla sınırlandırılmıştır. Lisans kümesindeki bir alt lisans sunucusunu sağlamak için, yöneticinin lisans sunucusundaki kullanıcı hesabının tam denetim ayrıcalıklarıyla birlikte SubEnrollService.asmx isteğe bağlı erişim denetim listesine (DACL) eklenmesi gerekir.

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
