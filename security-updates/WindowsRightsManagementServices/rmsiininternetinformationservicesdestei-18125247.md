---
TOCTitle: RMS için Internet Information Services Desteği
Title: RMS için Internet Information Services Desteği
ms:assetid: 'bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c'
ms:contentKeyID: 18125247
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747649(v=WS.10)'
---

RMS için Internet Information Services Desteği
==============================================

Birincil RMS hizmetleri, bir ASP .NET Web hizmetleri kümesi tarafından sağlanır. Bu Web hizmetleri Microsoft® Internet Information Services (IIS) üzerinde çalışır. Sunucu sağlama işlemi sırasında RMS, IIS'de sanal dizinler oluşturur. Sanal dizinlere Web hizmetlerine ait uygulama dosyaları yüklenir.

Sunucu sağlama aşamasında, sunucu üzerinde bulunan Web siteleri listesinden, altında sanal dizinler oluşturmak istediğiniz Web sitesini seçebilirsiniz. Bir sunucuyu sağlamadan önce, RMS için özel bir Web sitesi oluşturmak isteyebilirsiniz. Bunu yaparsanız, RMS dağıtımınıza özel kimlik doğrulamasını ve erişim kısıtlamalarını yapılandırabilirsiniz.

Varsayılan olarak Web hizmetleri dosyaları ve sanal dizinler, özelliklerine yetkisiz erişimi engellemek için isteğe bağlı erişim denetim listeleri (DACL) tarafından korunur. Bu öğelerdeki erişim denetim girdileri (ACE) aşağıdaki gibidir:

-   Administrators grubu tam denetime sahiptir
-   Yerel Sistem tam denetime sahiptir
-   RMS Service Group, Okuma ve Yürütme izinlerine sahiptir
-   Konuklar ve Kullanıcılar, Okuma ve Yürütme, Klasör İçeriğini Listeleme ve Okuma izinlerine sahiptir
-   Anonim erişime izin verilmez

Aşağıdaki tabloda IIS içinde oluşturulan sanal dizinler ve sanal dizinlere yüklenen hizmetler listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Sanal dizin</th>
<th style="border:1px solid black;" >Hizmet</th>
<th style="border:1px solid black;" >Web hizmeti dosyası</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">_wmcs</td>
<td style="border:1px solid black;">Bu, RMS küme yönetimi sanal dizinidir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sertifika</td>
<td style="border:1px solid black;">Bu sanal dizin RMS sertifikasını destekleyen hizmetleri içerir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Etkinleştirme proxy hizmeti</td>
<td style="border:1px solid black;">Activation.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Hesap sertifikası</td>
<td style="border:1px solid black;">Certification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Ön sertifika</td>
<td style="border:1px solid black;">Precertification.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Hizmet bulma</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Sunucu</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Sunucu Sertifikası</td>
<td style="border:1px solid black;">ServerCertification.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Mobil Aygıt Sertifikası</td>
<td style="border:1px solid black;">MobileDeviceCertfication.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kayıt</td>
<td style="border:1px solid black;">SubEnrollService.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lisans</td>
<td style="border:1px solid black;">Bu sanal dizin RMS lisansını destekleyen hizmetleri içerir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Lisans</td>
<td style="border:1px solid black;">License.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Yayımlama</td>
<td style="border:1px solid black;">Publish.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Sunucu</td>
<td style="border:1px solid black;">Server.asmx</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Hizmet bulma</td>
<td style="border:1px solid black;">ServiceLocator.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Admin</td>
<td style="border:1px solid black;">Bu sanal dizin RMS yönetimini destekleyen hizmetleri içerir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Yönetim</td>
<td style="border:1px solid black;">AdminSvc.asmx</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">.NET Uzaktan Erişim arabirimi</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DirectoryServices</td>
<td style="border:1px solid black;">Bu, DrmRemote'un alt dizinidir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747649.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Yönetim hizmeti, sağlanan arabirimlerin RMS'yi yapılandırmanıza olanak sağlaması nedeniyle diğer Web hizmetlerinden daha katı kısıtlamalara sahiptir. Bu nedenle, Users grubu üyeleri Yönetim hizmetine erişemezler. Ayrıca IP filtresi yalnızca yerel bilgisayara erişim izni verecek şekilde etkinleştirilir. DirectoryServices sanal dizini Konuk kullanıcılara erişim izni vermez. Hizmet bulma hizmeti Ağ Hizmeti hesabına tam denetleme izni verir. Lisans sunucusunu sağlamak üzere, RMS yöneticisinin erişimine izin vermek için varsayılan ACE'leri değiştirmeniz gerekir. |
