---
TOCTitle: 'MS10-MAR'
Title: Microsoft Güvenlik Bülteni Mart 2010 Özeti
ms:assetid: 'ms10-mar'
ms:contentKeyID: 61235831
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms10-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Mart 2010 Özeti
==========================================

Yayım Tarihi: 9 Mart 2010 Salı | Güncelleştirme Tarihi: 11 Ağustos 2010 Çarşamba

**Sürüm:** 3.1

Bu bülten özetinde Mart 2010'da yayımlanan güvenlik bültenleri listelenir.

Mart 2010 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 4 Mart 2010'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 10 Mart 2010 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Mart Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032427711&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

MS10-018 adlı bu bülten özetinin 2.0 sürümüne eklenen normal yayın döngüsü dışındaki güvenlik bültenine yönelik olarak, Microsoft, bu bültenle ilgili müşteri soruları için 30 Mart 2010 günü saat 13:00'te (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [30 Mart günü 13:00'teki Web yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032448112&culture=en-us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

Yürütmeyle İlgili Özetler
-------------------------

<span></span>
Aşağıdaki tabloda, bu ayın güvenlik bültenleri önem derecesine göre özetlenmektedir.

Etkilenen yazılımlar ile ilgili ayrıntılar için **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı sonraki bölüme bakın.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Bülten Başlığı ve Yürütmeyle İlgili Özet</th>
<th style="border:1px solid black;" >En Yüksek Önem Derecesi ve Güvenlik Açığının Etkisi</th>
<th style="border:1px solid black;" >Yeniden Başlatma Gereksinimi</th>
<th style="border:1px solid black;" >Etkilenen Yazılımlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=182969">MS10-018</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer için Toplu Güvenlik Güncelleştirmesi (980182)</strong> <br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen dokuz ve genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=183077">MS10-016</a></td>
<td style="border:1px solid black;"><strong>Windows Movie Maker'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (975561)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Windows Movie Maker ve Microsoft Producer 2003'te özel olarak bildirilen bir güvenlik açığını giderir. Windows Vista ve Windows 7 için kullanılabilen Windows Live Movie Maker bu güvenlik açığından etkilenmez. Bu güvenlik açığı, bir saldırgan özel hazırlanmış bir Movie Maker veya Microsoft Producer proje dosyası gönderir ve kullanıcıyı bu özel hazırlanmış dosyayı açmaya ikna ederse uzaktan kod yürütülmesine izin verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=182987">MS10-017</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (980150)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office Excel'deki özel olarak bildirilen yedi güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Excel dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, yerel kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, yararlanılabilirlik değerlendirmesi düzeylerine ve sonra da CVE Kimliklerine göre azalan sırayla listelenmektedir.
  
**Bu tabloyu nasıl kullanabilirim?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
| Bülten Kimliği                                            | Güvenlik Açığı Başlığı                                                                 | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                       |  
|-----------------------------------------------------------|----------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------|  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel Kaydında Bellek Bozulması Güvenlik Açığı                        | [CVE-2010-0257](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0257) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel MDXTUPLE Kaydında Öbek Taşması Güvenlik Açığı                   | [CVE-2010-0260](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0260) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel MDXSET Kaydında Öbek Taşması Güvenlik Açığı                     | [CVE-2010-0261](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0261) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel'de XLSX Dosyası Ayrıştırma Sırasında Kod Yürütme Güvenlik Açığı | [CVE-2010-0263](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0263) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel'de DbOrParamQry Kaydını Ayrıştırma Güvenlik Açığı               | [CVE-2010-0264](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0264) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-016](http://go.microsoft.com/fwlink/?linkid=183077) | Movie Maker ve Producer'da Arabellek Taşması Güvenlik Açığı                            | [CVE-2010-0265](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0265) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | HTML Nesnesinde Bellek Bozulması Güvenlik Açığı                                        | [CVE-2010-0491](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0491) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | HTML Nesnesinde Bellek Bozulması Güvenlik Açığı                                        | [CVE-2010-0492](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0492) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | HTML Öğesinde Etki Alanları Arası Güvenlik Açığı                                       | [CVE-2010-0494](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0494) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Yalnızca Windows 2000'de kod yürütülebilir                          |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Başlatılmamış Belleğin Bozulması Güvenlik Açığı                                        | [CVE-2010-0806](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0806) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır** |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | HTML İşlemede Bellek Bozulması Güvenlik Açığı                                          | [CVE-2010-0807](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0807) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel Sayfasında Nesne Türü Karıştırma Güvenlik Açığı                 | [CVE-2010-0258](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0258) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-017](http://go.microsoft.com/fwlink/?linkid=182987) | Microsoft Office Excel FNGROUPNAME Kaydında Başlatılmamış Bellek Güvenlik Açığı        | [CVE-2010-0262](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0262) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Yarış Durumunda Bellek Bozulması Güvenlik Açığı                                        | [CVE-2010-0489](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0489) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Bellek Bozulması Güvenlik Açığı                                                        | [CVE-2010-0805](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0805) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Başlatılmamış Belleğin Bozulması Güvenlik Açığı                                        | [CVE-2010-0267](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0267) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Kodlama Sonrasında Bilginin Açığa Çıkması Güvenlik Açığı                               | [CVE-2010-0488](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0488) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                               |  
| [MS10-018](http://go.microsoft.com/fwlink/?linkid=182969) | Başlatılmamış Belleğin Bozulması Güvenlik Açığı                                        | [CVE-2010-0490](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0490) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                               |
  
Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları  
--------------------------------------------------
  
<span></span>
Aşağıdaki tablolarda, bültenler başlıca yazılım kategorilerine ve önem derecelerine göre listelenmektedir.
  
**Bu tabloları nasıl kullanabilirim?**  
  
Bu tabloları, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip, yüklemenizle ilişkili güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.
  
**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.
  
#### Windows İşletim Sistemi ve Bileşenleri

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=389da7a9-e0a3-4b5d-801e-0a38fc55dcec)  
(Kritik)  
[Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=daf199c4-da56-4a7f-80e6-3936ce5c267b)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=6301e462-02be-4b9a-bae9-7c4821b42d2d)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2f2caa01-5cd1-45cb-9995-e34d933920d4)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=167ed896-d383-4dc0-9183-cd4cb73e17e7)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=46172617-293a-44c7-95b6-18202ab06a41)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Movie Maker 2.1](http://www.microsoft.com/downloads/details.aspx?familyid=cae81585-d0df-41b8-9277-ca02f1265056)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6c711387-6853-477c-917e-820a97613cf9)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=aadb1d97-5cec-45ed-9967-aaf41a0bcdac)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=284d70ea-24a3-4e67-a2a8-e9f272f728db)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=dc77f1c9-8240-42d9-aee9-30ac4f33bde7)  
(Önemli)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e957a7cf-e5ca-454d-b199-ec8fe6a6a2bf)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=53fc3285-63c4-487f-ad9a-7e1673aeffc7)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2be85462-28ec-4184-a326-0459554b7213)  
(Önemli)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=cb0e39f8-9730-4454-a0e3-479b610b1591)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5201a0c5-8162-4809-b9d1-0e972b0f0066)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=04abea55-ea2f-423f-b410-5536ea184ea3)  
(Önemli)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7ebd99b4-da6b-4dff-9f89-6a86d275a3da)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=ae2e9b75-1616-4fe3-91bb-e2e28252ff1c)<sup>[1]</sup>
(Önemli)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=ca2d1118-ca64-419d-86af-9396e61b90b0)<sup>[2]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=511aba0e-6f15-42cf-9c5d-b2f3e215b5a8)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c9584689-5196-4840-927c-23c8038f3382)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Movie Maker 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e27f353e-deb6-4d61-8808-c751d20a42a1)<sup>[1]</sup>
(Önemli)  
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=6a1f4126-97f2-4aee-bfe1-05bd13a0667b)<sup>[2]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c8933a45-62a7-4c19-be30-02e3a461f081)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=50809cc3-6baa-41b4-ba0a-596a1dd846ed)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=42f8c1f2-ee55-47af-b113-8d9f4bd40c8f)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c69a6dfe-66b1-4426-96a5-d64000296e76)\*\*  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=769043b5-df52-4446-9bd8-dc37d9fa00df)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e16c10d2-896d-48f3-bc76-5fa70881396a)\*\*  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c1c2309d-22db-4dbf-ad95-3219847cd42d)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c0145563-428e-47b6-b245-b59dce88ac0e)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6172dbec-6bfc-40bd-a0d4-67c39fb41b87)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="3">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
<td style="border:1px solid black;">
[**MS10-018**](http://go.microsoft.com/fwlink/?linkid=182969)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8b7c664b-8612-458f-bd0a-cf28b67f8374)\*\*  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=82fa6f47-002f-4943-888c-2e852675e76e)  
(Orta)
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Not**

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) ve [Windows Server 2008 R2 için Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) adlı MSDN makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008 ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS10-016 için Notlar**

<sup>[1]</sup>Windows Movie Maker'ın bu sürümleri belirtilen işletim sistemleriyle birlikte gelir.

<sup>[2]</sup>Windows Movie Maker 2.6, belirtilen işletim sistemlerine yüklenebilen isteğe bağlı bir karşıdan yüklemedir.

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Office Paketleri, Sistemleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-017**](http://go.microsoft.com/fwlink/?linkid=182987)
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e0136f62-60ce-4ebd-8660-be81eba29ae8)  
(KB978471)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7e42793e-747b-48da-968a-1ec29ea37151)  
(KB978474)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 ve Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03429f8a-8aab-4a59-97e4-7ce047f100a5)<sup>[1]</sup>
(KB978382)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Mac için Microsoft Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-017**](http://go.microsoft.com/fwlink/?linkid=182987)
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=ae5936f8-fe3f-4d23-a37c-d80f228e475e)  
(KB980837)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2008
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=e0ed1569-ab2f-407c-b728-4eddc463c385)  
(KB980839)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Açık XML Dosya Biçimi Dönüştürücüsü
</td>
<td style="border:1px solid black;">
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=4c5487d5-c912-4087-8c83-769e3fb78ea9)  
(KB980840)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Diğer Office Yazılımları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-017**](http://go.microsoft.com/fwlink/?linkid=182987)
</td>
<td style="border:1px solid black;">
[**MS10-016**](http://go.microsoft.com/fwlink/?linkid=183077)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer Service Pack 1 ve Microsoft Office Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=010d0a4d-02a4-4142-963b-a38cd06cc897)  
(KB978383)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1 ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=314f076e-8f9d-46c2-b666-86599a02bf15)  
(KB978380)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 ve Microsoft Office SharePoint Server 2007 Service Pack 2 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=94ddf6ef-3392-4d77-a02b-3bc0470721cd)<sup>[2]</sup>
(KB979439)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 ve Microsoft Office SharePoint Server 2007 Service Pack 2 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=06f6bffb-3fad-4fb5-878b-39550812e9b5)<sup>[2]</sup>
(KB979439)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Producer 2003
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Producer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=1b3c76d5-fc75-4f99-94bc-784919468e73)<sup>[3]</sup>
(Önemli)
</td>
</tr>
</table>
 
**MS10-017 için Notlar**

<sup>[1]</sup>Microsoft Office Excel 2007 Service Pack 1 ve Microsoft Office Excel 2007 Service Pack 2 için, müşterilerin bu bültende açıklanan güvenlik açıklarına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB978382'nin yanı sıra [Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1 ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=314f076e-8f9d-46c2-b666-86599a02bf15) (KB978380) güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

<sup>[2]</sup>Bu güncelleştirme Microsoft Office SharePoint Server 2007 Enterprise sürümünün varsayılan yapılandırması ve Internet Siteleri için Microsoft Office SharePoint Server 2007 gibi Excel Hizmetleri'nin yüklü olduğu sunuculara uygulanır. Microsoft Office SharePoint Server 2007 Standard sürümü Excel Hizmetleri'ni içermemektedir.

**MS10-016 için Notlar**

<sup>[3]</sup>Bu karşıdan yükleme Microsoft Producer 2003 yüklemenizi yeni sürüm olan Microsoft Producer'a yükseltir. Microsoft Producer yalnızca İngilizce olarak kullanılabilir.

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

Algılama ve Dağıtım Araçları ve Kılavuzu
----------------------------------------

<span></span>
**Güvenlik Merkezi**

Kuruluşunuzdaki sunuculara, masaüstü bilgisayarlara ve taşınabilir bilgisayarlara dağıtmanız gereken yazılımları ve güvenlik güncelleştirmelerini yönetin. Daha fazla bilgi için, bkz: [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171), Microsoft ürünlerinde güvenlik konusunda ek bilgi sağlar. Müşteriler, bu bilgilerin "En Son Güvenlik Güncelleştirmeleri" tıklatılarak da edinilebileceği [Evde Güvenlik](http://go.microsoft.com/fwlink/?linkid=85102) sitesini de ziyaret edebilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) ve [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) sitelerinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.

Son olarak, güvenlik güncelleştirmeleri [Microsoft Update Kataloğu](http://go.microsoft.com/fwlink/?linkid=96155)'ndan karşıdan yüklenebilir. Microsoft Update Kataloğu, Windows Update ve Microsoft Update aracılığıyla sunulan güvenlik güncelleştirmeleri, sürücüler ve hizmet paketleri gibi içeriğin arama yapılabilen bir kataloğunu sunar. Güvenlik bülteni numarasını kullanarak arama yaptığınızda (“MS07-036” gibi), uygulanabilen tüm güncelleştirmeleri sepete ekleyebilir (bir güncelleştirmenin farklı dilleri de dahil) ve istediğiniz klasöre karşıdan yükleyebilirsiniz. Microsoft Update Kataloğu hakkında daha fazla bilgi için, bkz: [Microsoft Update Kataloğu Hakkında SSS](http://go.microsoft.com/fwlink/?linkid=97900).

**Not** Microsoft, 1 Ağustos 2009'dan itibaren Office Update ve Office Update Envanter Aracı desteği sağlamayacaktır. Microsoft Office ürünlerine yönelik en son güncelleştirmeleri almaya devam etmek için [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) kullanın. Daha fazla bilgi için, [Microsoft Office Update Hakkında: Sık Sorulan Sorular](http://office.microsoft.com/en-us/downloads/fx010402221033.aspx) bölümüne bakın.

**Algılama ve Dağıtım Kılavuzu**

Microsoft, güvenlik güncelleştirmeleri için algılama ve dağıtım kılavuzu sağlar. Bu kılavuz, güvenlik güncelleştirmelerini algılamak ve dağıtmak üzere kullanılabilecek çeşitli araçların nasıl kullanılacağını BT uzmanlarının anlamasına yardımcı olabilecek öneriler ve bilgiler içerir. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 961747](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

Microsoft Baseline Security Analyzer (MBSA), yöneticilerin eksik güvenlik güncelleştirmeleri ve ayrıca sık rastlanan güvenlik yapılandırması hataları için yerel ve uzak sistemleri taramasına olanak sağlar. MBSA hakkında daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

**Windows Server Update Services**

Windows Server Update Services'ı (WSUS) kullanarak, yöneticiler en son kritik güncelleştirmeleri ve güvenlik güncelleştirmelerini Microsoft Windows 2000 işletim sistemlerine ve sonrasına, Office XP'ye ve sonrasına, Exchange Server 2003'e, SQL Server 2000'e, Microsoft Windows 2000 ve sonraki işletim sistemi sürümlerine hızla ve güvenilir şekilde dağıtabilir.

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) Web sitesini ziyaret edin.

**Systems Management Server**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; ayrıca bkz. [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Yöneticilerin güvenlik güncelleştirmelerini dağıtmak için SMS 2003'ü nasıl kullanacakları hakkında daha fazla bilgi için, bkz. [SMS 2003 Güvenlik Düzeltme Eki Yönetimi](http://go.microsoft.com/fwlink/?linkid=22939). SMS 2.0 kullanıcıları güvenlik güncelleştirmelerini dağıtmak için Güvenlik Güncelleştirmesi Envanter Aracı'nı (SUIT) da kullanabilirler. SMS hakkında daha fazla bilgi için, [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) Web sitesini ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler bu güncelleştirmeleri yüklemek için, Elevated Rights Deployment Tool'u kullanabilirler ([SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) içinde bulunur).

**Güncelleştirme Uyumluluğu Değerlendiricisi ve Uygulama Uyumluluğu Araç Takımı**

Güncelleştirmeler genelde uygulamalarınızın çalışması için gerekli olan aynı dosyalara ve kayıt defteri ayarlarına yazar. Bu durum da uyumsuzlukları tetikleyebilir ve güvenlik güncelleştirmelerinin dağıtılması için gereken zamanı artırabilir. [Uygulama Uyumluluğu Araç Takımı](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) ile birlikte gelen [Güncelleştirme Uyumluluğu Değerlendiricisi](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) bileşenlerini kullanarak, Windows güncelleştirmelerinin yüklü uygulamalara göre sınanması ve doğrulanması sürecini hızlandırabilirsiniz.

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Microsoft Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Yüksek Öncelikli Güncelleştirmeler

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): Yazılım Güncelleştirme Hizmetleri ve Windows Server Güncelleştirme Hizmetleri'nin tanımı içeriğe bağlı olarak değişir. Tüm Windows içeriğini içerir.
-   [Windows Server Update Services için Geçmiş Aylardaki Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft Windows dışındaki Microsoft ürünleri için yeni, yeniden düzenlenen ve yeniden yayımlanan tüm güncelleştirmeleri görüntüler.

#### Microsoft Etkin Koruma Programı (MAPP)

Microsoft müşterilerinin güvenlik korumalarını artırmak için, güvenlik açığı bilgilerini aylık güvenlik güncelleştirmesi yayın döngüsünden daha önce başlıca güvenlik yazılımı sağlayıcılarına sunmaktadır. Güvenlik yazılımı sağlayıcıları böylece bu güvenlik açığı bilgilerini kullanarak müşterilere virüsten koruma, ağ tabanlı davetsiz giriş algılama sistemleri veya ana bilgisayar tabanlı davetsiz giriş algılama sistemleri gibi güvenlik yazılımları ya da aygıtları aracılığıyla güncelleştirilmiş koruma sağlayabilirler. Güvenlik yazılımı sağlayıcıları tarafından hazırlanmış etkin korumaların bulunup bulunmadığını belirlemek üzere, [Microsoft Etkin Koruma Programı (MAPP) Ortakları](http://www.microsoft.com/security/msrc/mapp/partners.mspx) altında listelenen program ortaklarınca sağlanan etkin koruma Web sitelerini ziyaret edin.

#### Güvenlik Stratejileri ve Topluluğu

**Güncelleştirme Yönetim Stratejileri**

[Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) Web sitesi, güvenlik güncelleştirmelerini uygulamayla ilgili Microsoft'un en iyi uygulama önerilerini sağlar.

**Diğer Güvenlik Güncelleştirmelerini Edinme**

Diğer güvenlik sorunlarıyla ilgili güncelleştirmeler aşağıdaki konumlardan edinilebilir:

-   Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.
-   Tüketici platformlarına yönelik güncelleştirmeler [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) Web sitesinden edinilebilir.
-   Windows Update sitesinde bu ay için sunulan güvenlik güncelleştirmelerini, Yükleme Merkezi'nden Güvenlik ve Kritik Sürümler ISO CD'si Yansıması dosyaları olarak edinebilirsiniz. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Topluluğu**

Güvenliği geliştirmeyi ve BT altyapınızı en iyi duruma getirmeyi öğrenin; ayrıca [IT Pro Security Topluluğu](http://go.microsoft.com/fwlink/?linkid=21164)'nda güvenlik konularında diğer BT Uzmanlarının çalışmalarına katılın.

#### İlgili Kaynaklar

Microsoft, müşterilerimizi korumamıza yardım etmek için bizimle işbirliği yapan aşağıdaki kişi ve kuruluşlara [teşekkür eder](http://go.microsoft.com/fwlink/?linkid=21127):

-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Damián Frizza, MS10-016'da açıklanan sorunu bildirdiği için
-   [VUPEN Vulnerability Research Team](http://www.vupen.com/) için çalışan Nicolas Joly, MS10-017'de açıklanan sorunu bildirdiği için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Sean Larsson, MS10-017'de açıklanan dört sorunu bildirdiği için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS10-017'de açıklanan sorunu bildirdiği için
-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Damián Frizza, MS10-017'de açıklanan sorunu bildirdiği için
-   [Secunia](http://secunia.com), MS10-018'de açıklanan sorun konusunda bizimle çalıştıkları için
-   [Cyber Defense Institute Inc.](http://www.cyberdefense.jp/) için çalışan Daiki Fukumori, MS10-018'de açıklanan sorunu bildirdiği için
-   [Red Database Security](http://www.red-database-security.com/) için çalışan Alexander Kornbrust, MS10-018'de açıklanan sorunu bildirdiği için
-   [iSIGHT Partners](http://www.isightpartners.com/) Global Vulnerability Partnership için çalışan Ivan Fratric, MS10-018'de açıklanan sorunu bildirdiği için
-   [team509](http://www.team509.com/) için çalışan Wushi, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS10-018'de açıklanan sorunu bildirdikleri için
-   Simon Zuckerbraun, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-018'de açıklanan sorunu bildirdikleri için
-   [Context Information Security](http://www.contextis.co.uk/) için çalışan Paul Stone, MS10-018'de açıklanan sorunu bildirdiği için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS10-018'de açıklanan sorunu bildirdikleri için
-   [VenusTech](http://www.venustech.com.cn/) bünyesindeki ADLab, MS10-018'de açıklanan iki sorunu bildirdikleri için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (9 Mart 2010): Bülten Özeti yayımlandı.
-   V2.0 (30 Mart 2010): Microsoft Güvenlik Bülteni MS10-018, Internet Explorer için Toplu Güncelleştirme (980182) eklendi. Normal yayın döngüsü dışındaki bu güvenlik bülteni için bülten web yayını bağlantısı da eklendi.
-   V3.0 (3 Mayıs 2010): MS10-016 ile ilişkili Microsoft Producer karşıdan yüklemesinin kullanıma sunulduğu duyuruldu.
-   V3.1 (11 Ağustos 2010): MS10-016 için etkilenen bileşen olarak Windows 7 üzerinde Windows Movie Maker 2.6 kaldırıldı.

*Built at 2014-04-18T01:50:00Z-07:00*
