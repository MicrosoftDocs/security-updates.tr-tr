---
TOCTitle: RMS için Gerekli Hesaplar ve İzinler
Title: RMS için Gerekli Hesaplar ve İzinler
ms:assetid: '07a51daa-6823-41e6-b453-92f1a0592361'
ms:contentKeyID: 18124995
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720178(v=WS.10)'
---

RMS için Gerekli Hesaplar ve İzinler
====================================

Aşağıdaki tabloda RMS'yi dağıtmak ve yönetmek için gerekli kullanıcı hakları ve izinler belirtilmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Etkinlik</th>
<th style="border:1px solid black;" >Kullanıcı Hesabı ve İzinleri</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS'yi Yükleme</td>
<td style="border:1px solid black;">Yerel Administrators grubunun üyesi olan bir etki alanı hesabını kullanarak oturum açabilirsiniz.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS'yi Sağlama</td>
<td style="border:1px solid black;">Yerel Administrators grubunun üyesi olan bir etki alanı hesabını kullanarak oturum açabilirsiniz. Ayrıca, kullandığınız hesabın SQL Server veritabanına verilmiş Sistem Yöneticisi rolüne sahip SQL oturumu açma hakkı olmalıdır; böylece RMS, veritabanlarını ayarlayabilir.
Hazırlama sırasında, daha önceden oluşturmuş olmanız gereken RMS hizmeti hesabını belirtmelisiniz. Hesap, hiçbir ek izni olmayan standart etki alanı kullanıcı hesabı olmalıdır. Bu hesap RMS Service Group'un bir üyesi yapılır ve normal işlemler sırasında RMS'nin çalışacağı hesaptır.
Veritabanının kök sertifika sunucusu ile aynı bilgisayarda bulunduğu tek sunucu dağıtımları için Local System hesabını belirtebilirsiniz. Ancak, güvenlik nedenleriyle, her zaman Local System hesabı yerine RMS hizmeti hesabını belirtmeniz önerilir. Veritabanı ayrı bir sunucuda bulunduğunda, RMS hizmeti hesabını belirtmelisiniz.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS Yönetimi</td>
<td style="border:1px solid black;">Yerel Administrators grubunun üyesi olan bir etki alanı hesabını kullanarak oturum açabilirsiniz. Güvenlik ayarlarını yönetim Web sayfalarına erişimi yönetecek şekilde özelleştirebilirsiniz.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720178.note(WS.10).gif)Not                                                                                                                                                                                                                  |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| RMS sunucusuna oturum açmak için kullanılan hesap, Domain Admins gibi herhangi bir ek etki alanı grubuna üye olmayı gerektirmez. Ancak, hizmet bağlantı noktasını kaydetme ve güvenlik ilkelerini değiştirme gibi bazı yönetim görevleri ek ayrıcalıklara sahip bir hesap gerektirir. |
