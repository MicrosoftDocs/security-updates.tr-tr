---
TOCTitle: 'MS12-APR'
Title: Microsoft Güvenlik Bülteni Nisan 2012 Özeti
ms:assetid: 'ms12-apr'
ms:contentKeyID: 61235848
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms12-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Nisan 2012 Özeti
===========================================

Yayım Tarihi: 10 Nisan 2012 Salı | Güncelleştirme Tarihi: 26 Nisan 2012 Perşembe

**Sürüm:** 2.0

Bu bülten özetinde Nisan 2012'de yayımlanan güvenlik bültenleri listelenir.

Nisan 2012 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 5 Nisan 2012'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://go.microsoft.com/fwlink/?linkid=217213).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 11 Nisan 2012 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Nisan Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499650). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://go.microsoft.com/fwlink/?linkid=217214).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242739">MS12-023</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer Toplu Güvenlik Güncelleştirmesi (2675157)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen beş güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, geçerli kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238623">MS12-024</a></td>
<td style="border:1px solid black;"><strong>Windows'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2653956)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı veya uygulama etkilenen bir sistemde özel hazırlanmış, imzalı bir taşınabilir yürütülebilir (PE) dosya çalıştırır ya da yüklerse uzaktan kod yürütülmesine olanak verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=242032">MS12-025</a></td>
<td style="border:1px solid black;"><strong>.NET Framework'teki Güvenlik Açığı Uzaktan Kod</strong> <strong>Yürütülmesine İzin Verebilir(2671605)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft .NET Framework'teki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir web sayfasını XAML Tarayıcı Uygulamaları (XBAP) çalıştırabilen bir web tarayıcısı kullanarak görüntülerken istemci sistemde uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Güvenlik açığı, IIS çalıştıran bir sunucu sisteminde, söz konusu sunucu ASP.NET sayfalarının işlenmesine izin veriyorsa ve saldırgan özel hazırlanmış bir ASP.NET sayfasını başarıyla sunucuya yükleyip çalıştırırsa (web barındırma senaryosunda bu durum geçerli olabilir) uzaktan kod yürütülmesine izin verebilmektedir. Bu güvenlik açığı, Windows .NET uygulamaları tarafından Kod Erişimi Güvenliği (CAS) kısıtlamalarını atlamak için de kullanılabilir. Web'de gezinme tabanlı saldırı senaryosunda, bir saldırgan bu açıktan yararlanmak için kullanılan bir web sayfası içeren bir web sitesi barındırabilir. Ayrıca, kullanıcı tarafından sağlanan içeriği veya reklamları kabul eden ya da barındıran güvenliği aşılmış web sitelerinde, bu güvenlik açığından yararlanılabilecek özel hazırlanmış içerik bulunabilir. Ancak bu durumların hiçbirinde, saldırganın, bu web sitelerini ziyaret etmek için kullanıcıyı zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi web sitesine götüren bir bağlantıyı tıklatmalarını sağlayarak onları bu web sitesine çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246275">MS12-027</a></td>
<td style="border:1px solid black;"><strong>Windows Ortak Bileşenleri'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2664258)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows ortak denetimlerindeki özel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı bu açıktan yararlanacak şekilde özel olarak tasarlanmış içerik bulunan bir web sitesini ziyaret ederse uzaktan kod yürütülmesine izin verebilir. Ancak bu durumların hiçbirinde, saldırganın kullanıcıları bu tür bir web sitesini ziyaret etmeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi web sitesine yönlendiren bir bağlantıyı tıklatmalarını sağlayarak onları bu web sitesini ziyaret etmeye ikna etmesi gerekir. Kötü amaçlı dosya bir e-posta eki olarak da gönderilebilir; ancak saldırganın bu güvenlik açığından yararlanabilmesi için, kullanıcıyı bu eki açmaya ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft Server Yazılımı,<br />
Microsoft Geliştirici Araçları</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238519">MS12-026</a></td>
<td style="border:1px solid black;"><strong>Forefront Unified Access Gateway'deki (UAG) Güvenlik Açıkları Bilginin Açığa Çıkmasına Neden Olabilir (2663860)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Forefront Unified Access Gateway'deki (UAG) özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıklarından önem düzeyi daha yüksek olanı, bir saldırgan UAG sunucusuna özel hazırlanmış bir istek gönderirse bilginin açığa çıkmasına olanak sağlayabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Bilginin Açığa Çıkması</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232498">MS12-028</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2639185)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office ve Microsoft Works'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Works dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, geçerli kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
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
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, bülten numarasına ve ardından CVE numarasına göre listelenmektedir. Bültenlerde yalnızca önem derecesi Kritik veya Önemli olan güvenlik açıkları yer almaktadır.
  
**Bu tabloyu nasıl kullanabilirim?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde kod yürütme ve hizmet reddi yararlanmalarının olasılığını öğrenmek amacıyla kullanın. Bu ayın güncelleştirmelerini hangi öncelikle dağıtacağınızı belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini inceleyin. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/security/cc998259.aspx)'ne bakın.
  
Aşağıdaki sütunlarda yer alan "En Son Yazılım Sürümü" ve "Yazılımın Eski Sürümleri", bültenin "Etkilenen Yazılımlar" ve "Etkilenmeyen Yazılımlar" tablolarında listelenen ilgili yazılımın sırasıyla en son sürümü ve desteklenmeye devam eden eski sürümleri anlamına gelir.
  
| Bülten Kimliği                                            | Güvenlik Açığı Başlığı                                                | CVE Kimliği                                                                      | En Son Yazılım Sürümü için Yararlanma Değerlendirmesi                                             | Yazılımın Eski Sürümleri için Yararlanma Değerlendirmesi                                          | Hizmet Reddi Yararlanma Değerlendirmesi | Önemli Notlar                                                                                                    |  
|-----------------------------------------------------------|-----------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|-----------------------------------------|------------------------------------------------------------------------------------------------------------------|  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | Jscript9 Uzaktan Kod Yürütme Güvenlik Açığı                           | [CVE-2012-0169](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0169) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Etkilenmez                                                                                        | Geçici                                  | (Yok)                                                                                                            |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | OnReadyStateChange Uzaktan Kod Yürütme Güvenlik Açığı                 | [CVE-2012-0170](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0170) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                            |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | SelectAll Uzaktan Kod Yürütme Güvenlik Açığı                          | [CVE-2012-0171](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0171) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                            |  
| [MS12-023](http://go.microsoft.com/fwlink/?linkid=242739) | VML Stilinde Uzaktan Kod Yürütme Güvenlik Açığı                       | [CVE-2012-0172](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0172) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                            |  
| [MS12-024](http://go.microsoft.com/fwlink/?linkid=238623) | WinVerifyTrust'ta İmza Doğrulaması Güvenlik Açığı                     | [CVE-2012-0151](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0151) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Uygulanamaz                             | (Yok)                                                                                                            |  
| [MS12-025](http://go.microsoft.com/fwlink/?linkid=242032) | .NET Framework'te Parametre Doğrulaması Güvenlik Açığı                | [CVE-2012-0163](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0163) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Uygulanamaz                             | (Yok)                                                                                                            |  
| [MS12-026](http://go.microsoft.com/fwlink/?linkid=238519) | UAG Varsayılan Web Sitesine Filtre Uygulanmadan Erişim Güvenlik Açığı | [CVE-2012-0147](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0147) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Etkilenmez                                                                                        | Uygulanamaz                             | Bu, bir bilginin açığa çıkması güvenlik açığıdır.                                                                |  
| [MS12-027](http://go.microsoft.com/fwlink/?linkid=246275) | MSCOMCTL.OCX RCE Güvenlik Açığı                                       | [CVE-2012-0158](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0158) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Uygulanamaz                             | Microsoft bu güvenlik açığından yararlanmaya çalışan sınırlı sayıda hedefe yönelik saldırı olduğunu bilmektedir. |  
| [MS12-028](http://go.microsoft.com/fwlink/?linkid=232498) | Office WPS Dönüştürücüsünde Öbek Taşması Güvenlik Açığı               | [CVE-2012-0177](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0177) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Uygulanamaz                             | Microsoft Office 2007 Service Pack 3 ve Microsoft Office 2010'un tüm desteklenen sürümleri etkilenmez.           |
  
Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları  
--------------------------------------------------
  
<span></span>
Aşağıdaki tablolarda, bültenler başlıca yazılım kategorilerine ve önem derecelerine göre listelenmektedir.
  
**Bu tabloları nasıl kullanabilirim?**  
  
Bu tabloları, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip, yüklemenizle ilişkili güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.
  
**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.
  
#### Windows İşletim Sistemi ve Bileşenleri

 
<table style="border:1px solid black;">
<tr>
<th colspan="4">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a490c62-16c4-402a-b2d9-3e8cfb5bcebd)  
(KB2675157)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=81b28dd9-87aa-46cc-94c6-2da39d0298db)  
(KB2675157)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=74ce0e29-046b-4ac3-89a1-b292a177972f)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=575afd20-cee4-4fa9-b781-9f8dfdd41ebe)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1cfeae57-d4e9-4fff-8956-523e7b71453c)  
(KB2656378)  
(Yalnızca Media Center Edition 2005 ve Tablet PC Edition 2005)  
(Kritik)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a1b7be43-a32e-456b-8df0-c26cdf187682)  
(KB2675157)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=29ec7b06-c7aa-4149-bb2c-25af7d38a6a9)  
(KB2675157)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=646c6352-4d99-413a-a75b-71289b5d2b25)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=adc31695-1be6-4976-869c-007df8ac8508)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam** **Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=020e0d68-dd1c-4297-b565-fcc6dcf5f280)  
(KB2675157)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=17b0c139-2709-424d-9d17-827af468e858)  
(KB2675157)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=3289a80a-d1b1-4494-bede-03d0be579acf)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f79c8940-ca31-4ff7-924e-847f5eef7864)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ffd26218-e149-44ea-a0b9-f2a1315fce9e)  
(KB2656376)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=295292d3-01a3-4574-b994-8cdbcf5a0d2e)  
(KB2675157)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=04656a93-e958-4764-afe8-27c476855506)  
(KB2675157)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=dff4fb63-b319-49ed-8a9d-6b15e43d5bfd)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=03ebf111-1e7b-4dc2-b84f-a26c6b5f0d58)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=09011393-c7d5-4225-9b8e-5a234d4dbcd1)  
(KB2675157)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a5ef0147-595e-43b5-819f-73780fcef10d)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=734ff97a-7d72-4bfe-9557-7fac91902f8e)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1338821-d8b2-4513-aa35-087323188509)  
(KB2656369)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f598cad1-4d1a-40ce-a016-bb58778d5dc0)  
(KB2675157)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=44284277-06a7-405d-9187-8f50a042604d)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=51088164-13b7-4216-90f1-20c92c8b8ca9)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c7683919-6d46-4b3e-aa98-1bef20141835)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2717a997-2066-4a83-ae9b-4611a0851101)  
(KB2675157)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=19684033-ddeb-464f-9a22-f580a9c19f8e)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bbb99aee-aadd-4ec7-9e27-91cb8d90803e)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4d9f8a6e-17bd-4ed3-8bc7-d5e3b11ca12a)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3e361edd-234b-4053-aa49-278b9fde4d5c)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6eb6781e-7b38-4679-afbc-4e3bb5747fd8)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d34d7981-ed63-460d-95e4-e6da1ac41d2f)\*\*  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c36c20f7-a742-4151-b8f2-85ef80479d06)\*  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=60b76a3c-4530-4101-931f-45df621e1eed)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fd657467-a45c-4354-b947-3a3cceb9b690)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=c9d773e9-6a2e-45db-8f30-7da0082d909c)\*\*  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=330cea47-221d-439e-b106-58a146fc28ee)\*  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3235216f-497f-4934-81b8-1eb9929e98c9)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1ec74522-ec1e-4b3c-bfeb-6a505cc4f11a)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c376fbdc-2289-47b6-950b-4e668cd3a390)  
(KB2656370)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e1c10a1-9cb2-4815-8aa6-e401ced5df80)  
(KB2656374)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9a58ca0b-fad7-418e-80ae-ca478168f887)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e6724be3-ff4b-4dea-95f3-0b13998b6758)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac183b66-0247-4ae5-bda0-e8d0070917c8)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7215f707-c536-4d81-ad66-e7bff592e400)  
(KB2675157)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=0ff822d0-074a-409c-9174-8100618c6171)  
(KB2675157)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=27226e64-266f-499e-8c57-866593fc3430)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-023**](http://go.microsoft.com/fwlink/?linkid=242739)
</td>
<td style="border:1px solid black;">
[**MS12-024**](http://go.microsoft.com/fwlink/?linkid=238623)
</td>
<td style="border:1px solid black;">
[**MS12-025**](http://go.microsoft.com/fwlink/?linkid=242032)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)\*  
(KB2656372)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=237d94e6-b9b9-4177-81fa-a67df2806b0e)\*\*  
(KB2675157)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=d002bfe4-10e9-46d3-a460-06d112201ca5)\*\*  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=54db1495-31bb-4435-a442-74e484630b8a)\*  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)\*  
(KB2656373)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)\*<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c3f521a9-4dc8-46b7-a7f2-696b8759b398)  
(KB2656372)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7bdba902-0a6e-451e-a29b-6d0a03ff5664)  
(KB2675157)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9a4115bf-028b-4dcc-8995-d3341fdf42f2)  
(KB2653956)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=efccca8d-1371-4cda-96ab-ceef735742e2)  
(KB2656373)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=40b1ae34-28ad-41a0-88df-b905517e4acf)<sup>[1]</sup>
(KB2656368)  
(Kritik)
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Notlar**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS12-025 **için** **Not****

<sup>[1]</sup>**.NET Framework 4 ve .NET Framework 4 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4 ve .NET Framework 4 İstemci Profili. .NET Framework 4 İstemci Profili, .NET Framework 4'ün bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4'ü hem de .NET Framework 4 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<tr>
<th colspan="3">
Microsoft Office Paketleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fbf24cc6-89e1-48dd-bb83-23eed30195e1)  
(KB2596871)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)  
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Windows ortak denetimleri)  
(KB2598039)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=23c9d7bf-c9e0-4e01-8b66-da542332a28b)  
(Windows ortak denetimleri)  
(KB2598039)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Office Web Bileşenleri
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Web Bileşenleri Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Web Bileşenleri Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)  
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Diğer Microsoft Office Yazılımları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
<td style="border:1px solid black;">
[**MS12-028**](http://go.microsoft.com/fwlink/?linkid=232498)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=94e17a66-cf09-4314-89ec-53deadabfa66)  
(KB2680317)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 6–9 Dosya Dönüştürücüsü
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Works 6–9 Dosya Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=4605f684-6314-4758-adeb-2a8810dfc8d1)  
(KB2680326)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-027 için Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Server Yazılımı

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Analysis Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=198f1819-818b-4b2e-a424-4a45729746eb)  
(KB983807)  
(Kritik)  
GDR güncelleştirmesi:  
[Microsoft SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2a9d97e8-79e0-4997-88fe-1224707e1b37)  
(KB983808)  
(Kritik)  
QFE güncelleştirmesi:  
[Microsoft SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8d0cac2f-f227-4e00-9454-4df62be86407)  
(KB983809)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft SQL Server Bileşenleri
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Microsoft SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Microsoft SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Microsoft SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SQL Server 2005 Express Edition with Advanced Services Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2005 Express Edition with Advanced Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d0d34b4f-4bcd-4df7-8ebc-87367e889959)<sup>[1]</sup>
(Windows ortak denetimleri)  
(KB2597112)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Microsoft SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Microsoft SQL Server 2008 Service Pack 3
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft SQL Server 2008 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 3
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 3
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Microsoft SQL Server 2008 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Microsoft SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Microsoft SQL Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft SQL Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft SQL Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft SQL Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Microsoft SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Microsoft SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Microsoft SQL Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Microsoft SQL Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=17294713-5c03-4439-bcae-471e9b1e1ac9)<sup>[2]</sup>
(Windows ortak denetimleri)  
(KB2598041)  
(Kritik)
</td>
</tr>
</table>
 
**MS12-027 **için** **Notlar****

<sup>[1]</sup>Bu güncelleştirme Microsoft Office 2003 için yapılan KB2597112 güncelleştirmesi ile aynıdır

<sup>[2]</sup>Bu güncelleştirme Microsoft Office 2007 için yapılan KB2598041 güncelleştirmesi ile aynıdır

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft BizTalk Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft BizTalk Server 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft BizTalk Server 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d90b78d2-551b-499b-9bd2-85b40646dbc7)  
(KB2645025)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Commerce Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2002 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2002 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=35de8833-50ae-482d-aa07-497bf68fb38e)  
(KB2658674)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3f04fb90-8f11-4392-a4bc-800903091f04)  
(KB2658677)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009](http://www.microsoft.com/downloads/details.aspx?familyid=a8998b6b-e9a4-457e-a34f-0458dda81f2f)  
(KB2655547)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Commerce Server 2009 R2
</td>
<td style="border:1px solid black;">
[Microsoft Commerce Server 2009 R2](http://www.microsoft.com/downloads/details.aspx?familyid=e9221811-8913-412b-ae04-21a55ce7c4c5)  
(KB2658676)  
(Kritik)
</td>
</tr>
</table>
 
**MS12-027 için Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Geliştirici Araçları ve Yazılımları

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Visual FoxPro
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3a7ff474-f1e0-4c86-9555-64e8e7357890)  
(KB2647488)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=53c0132e-7724-4e94-abe9-e79b76ce35d7)  
(KB2647490)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Visual Basic
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-027**](http://go.microsoft.com/fwlink/?linkid=246275)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Basic 6.0 Çalışma Zamanı Modülü
</td>
<td style="border:1px solid black;">
[Visual Basic 6.0 Çalışma Zamanı Modülü](http://www.microsoft.com/downloads/details.aspx?familyid=0afe933a-1e62-45c4-910c-ea94b203df5a)  
(KB2641426)  
(Kritik)
</td>
</tr>
</table>
 
**MS12-027 için Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Uzaktan Erişim Yazılımı

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-026**](http://go.microsoft.com/fwlink/?linkid=238519)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d4b4ecc4-8bc6-43d0-b872-93673e0d9a6f)<sup>[1]</sup>
(KB2649261)  
(Önemli)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1 Update 1](http://www.microsoft.com/downloads/details.aspx?familyid=e0f9acab-bfb8-4758-b60d-64e68a84fba0)<sup>[1]</sup>
(KB2649262)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-026** **için** **Not**

<sup>[1]</sup>Bu güncelleştirme yalnızca Microsoft Yükleme Merkezi'nden edinilebilir.

Algılama ve Dağıtım Araçları ve Kılavuzu
----------------------------------------

<span></span>
**Güvenlik Merkezi**

Kuruluşunuzdaki sunuculara, masaüstü bilgisayarlara ve taşınabilir bilgisayarlara dağıtmanız gereken yazılımları ve güvenlik güncelleştirmelerini yönetin. Daha fazla bilgi için, bkz: [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171), Microsoft ürünlerinde güvenlik konusunda ek bilgi sağlar. Müşteriler, bu bilgilerin "En Son Güvenlik Güncelleştirmeleri" tıklatılarak da edinilebileceği [Evde Güvenlik](http://go.microsoft.com/fwlink/?linkid=85102) sitesini de ziyaret edebilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) ve [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) sitelerinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.

Mac için Microsoft Office müşterileri, Microsoft yazılımlarının güncel kalmasına yardımcı olmak üzere Mac için Microsoft OtomatikGüncelleştir'i kullanabilirler. Mac için Microsoft OtomatikGüncelleştir'i kullanma hakkında daha fazla bilgi için, bkz: [Yazılım güncelleştirmelerini otomatik olarak denetleme](http://mac2.microsoft.com/help/office/14/en-us/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Son olarak, güvenlik güncelleştirmeleri [Microsoft Update Kataloğu](http://go.microsoft.com/fwlink/?linkid=96155)'ndan karşıdan yüklenebilir. Microsoft Update Kataloğu, Windows Update ve Microsoft Update aracılığıyla sunulan güvenlik güncelleştirmeleri, sürücüler ve hizmet paketleri gibi içeriğin arama yapılabilen bir kataloğunu sunar. Güvenlik bülteni numarasını kullanarak arama yaptığınızda (“MS07-036” gibi), uygulanabilen tüm güncelleştirmeleri sepete ekleyebilir (bir güncelleştirmenin farklı dilleri de dahil) ve istediğiniz klasöre karşıdan yükleyebilirsiniz. Microsoft Update Kataloğu hakkında daha fazla bilgi için, bkz: [Microsoft Update Kataloğu Hakkında SSS](http://go.microsoft.com/fwlink/?linkid=97900).

**Algılama ve Dağıtım Kılavuzu**

Microsoft, güvenlik güncelleştirmeleri için algılama ve dağıtım kılavuzu sağlar. Bu kılavuz, güvenlik güncelleştirmelerini algılamak ve dağıtmak üzere kullanılabilecek çeşitli araçların nasıl kullanılacağını BT uzmanlarının anlamasına yardımcı olabilecek öneriler ve bilgiler içerir. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 961747](http://support.microsoft.com/kb/961747).

**Microsoft Baseline Security Analyzer**

Microsoft Baseline Security Analyzer (MBSA), yöneticilerin eksik güvenlik güncelleştirmeleri ve ayrıca sık rastlanan güvenlik yapılandırması hataları için yerel ve uzak sistemleri taramasına olanak sağlar. MBSA hakkında daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

**Windows Server Update Services**

Windows Server Update Services'ı (WSUS) kullanarak, yöneticiler en son kritik güncelleştirmeleri ve güvenlik güncelleştirmelerini Microsoft Windows 2000 işletim sistemlerine ve sonrasına, Office XP'ye ve sonrasına, Exchange Server 2003'e, SQL Server 2000'e, Microsoft Windows 2000 ve sonraki işletim sistemi sürümlerine hızla ve güvenilir şekilde dağıtabilir.

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://technet.microsoft.com/en-us/wsus/default.aspx) Web sitesini ziyaret edin.

**System Center Configuration Manager 2007**

Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, kuruluş genelindeki BT sistemlerine yönelik güncelleştirmeleri teslim etme ve yönetme görevini kolaylaştırır. Configuration Manager 2007 ile, BT yöneticileri Microsoft ürünlerine yönelik güncelleştirmeleri masaüstü bilgisayarlar, dizüstü bilgisayarlar, sunucular ve mobil aygıtlar gibi çeşitli aygıtlara teslim edebilirler.

Configuration Manager 2007'deki otomatik güvenlik açığı değerlendirmesi, güncelleştirme gereksinimini belirler ve önerilen eylemleri bildirir. Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, BT yöneticileri tarafından dünya genelinde kullanılan ve zaman içinde kendini kanıtlamış bir güncelleştirme altyapısı olan Microsoft Windows Software Update Services'a (WSUS) dayalıdır. Yöneticilerin güncelleştirmeleri dağıtmak üzere Configuration Manager 2007'yi nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Yazılım Güncelleştirme Yönetimi](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Configuration Manager hakkında daha fazla bilgi için, [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx)'ı sayfasını ziyaret edin.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir.

**Not** System Management Server 2003, 12 Ocak 2010'dan itibaren temel destek dışında kalmıştır. Ürün ömrü hakkında daha fazla bilgi için, [Microsoft Destek Ömrü](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle) Web sitesini ziyaret edin. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; önceki bölüm olan **System Center Configuration Manager 2007** konusuna bakın.

Yöneticilerin güvenlik güncelleştirmelerini dağıtmak üzere SMS 2003'ü nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Microsoft Systems Management Server 2003 Senaryoları ve Yordamları: Yazılım Dağıtımı ve Düzeltme Eki Yönetimi](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=tr). SMS hakkında bilgi için, [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx)'ı ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler bu güncelleştirmeleri yüklemek için, Elevated Rights Deployment Tool'u kullanabilirler ([SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=tr) içinde bulunur).

**Güncelleştirme Uyumluluğu Değerlendiricisi ve Uygulama Uyumluluğu Araç Takımı**

Güncelleştirmeler genelde uygulamalarınızın çalışması için gerekli olan aynı dosyalara ve kayıt defteri ayarlarına yazar. Bu durum da uyumsuzlukları tetikleyebilir ve güvenlik güncelleştirmelerinin dağıtılması için gereken zamanı artırabilir. [Uygulama Uyumluluğu Araç Takımı](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=tr) ile birlikte gelen [Güncelleştirme Uyumluluğu Değerlendiricisi](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) bileşenlerini kullanarak, Windows güncelleştirmelerinin yüklü uygulamalara göre sınanması ve doğrulanması sürecini hızlandırabilirsiniz.

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Güncelleştirmeler

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): Yazılım Güncelleştirme Hizmetleri ve Windows Server Güncelleştirme Hizmetleri'nin tanımı içeriğe bağlı olarak değişir. Tüm Windows içeriğini içerir.
-   [Windows Server Update Services için Geçmiş Aylardaki Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft Windows dışındaki Microsoft ürünleri için yeni, yeniden düzenlenen ve yeniden yayımlanan tüm güncelleştirmeleri görüntüler.

#### Microsoft Etkin Koruma Programı (MAPP)

Microsoft müşterilerinin güvenlik korumalarını artırmak için, güvenlik açığı bilgilerini aylık güvenlik güncelleştirmesi yayın döngüsünden daha önce başlıca güvenlik yazılımı sağlayıcılarına sunmaktadır. Güvenlik yazılımı sağlayıcıları böylece bu güvenlik açığı bilgilerini kullanarak müşterilere virüsten koruma, ağ tabanlı davetsiz giriş algılama sistemleri veya ana bilgisayar tabanlı davetsiz giriş algılama sistemleri gibi güvenlik yazılımları ya da aygıtları aracılığıyla güncelleştirilmiş koruma sağlayabilirler. Güvenlik yazılımı sağlayıcıları tarafından hazırlanmış etkin korumaların bulunup bulunmadığını belirlemek üzere, [Microsoft Etkin Koruma Programı (MAPP) Ortakları](http://go.microsoft.com/fwlink/?linkid=215201) altında listelenen program ortaklarınca sağlanan etkin koruma Web sitelerini ziyaret edin.

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

-   [AISec](http://www.aisec.cn/) için çalışan linx2008, MS12-023'te açıklanan bir sorunu bildirdiği için
-   [TOPdesk](http://www.topdesk.com) için çalışan Roel Spilker, MS12-023'te açıklanan bir sorunu bildirdiği için
-   [VeriSign iDefense Labs](http://labs.idefense.com) ile birlikte çalışan Jose Antonio Vazquez Gonzalez, MS12-023'te açıklanan bir sorunu bildirdiği için
-   [TippingPoint](http://www.tippingpoint.com) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-023'te açıklanan sorunu bildirdiği için
-   [TippingPoint](http://www.tippingpoint.com) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-023'te açıklanan sorunu bildirdiği için
-   Masato Kinugawa, MS12-023'ün içerdiği kapsamlı savunma değişiklikleri konusunda bizimle birlikte çalıştığı için
-   [Avast Software](http://www.avast.com/) için çalışan Robert Zacek ve Igor Glucksmann, MS12-024'de açıklanan bir sorunu bildirdikleri için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Vitaliy Toropov, MS12-025'de açıklanan bir sorunu bildirdiği için
-   [IOActive, Ltd.](http://ioactive.co.uk/) için çalışan Shaun Colley, MS12-028'de açıklanan bir sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   BT uzmanları için güvenlik çözümleri: [TechNet Security Sitesinin Sorun Giderme ve Destek Bölümü](http://technet.microsoft.com/security/bb980617.aspx)
-   Windows çalışan bilgisayarınızın virüslere ve kötü amaçlı yazılımlara karşı korunmasına yardım edin: [Virüs ve Güvenlik Çözüm Merkezi](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Ülkenize göre yerel destek: [Uluslararası Destek](http://support.microsoft.com/common/international.aspx)

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (10 Nisan 2012): Bülten Özeti yayımlandı.
-   V2.0 (26 Nisan 2012): MS12-027 için, Etkilenen Yazılımlar bölümüne SQL Server 2008 R2'nin Service Pack 1 sürümleri eklendi ve Microsoft SQL Server 2000 Analysis Services Service Pack 4 için QFE ve GDR ayrımı geçerli olmadığından, güncelleştirmenin bu ürünün tüm yüklemelerine uygulandığı Etkilenen Yazılımlar tablosunda açıklığa kavuşturuldu. Bunlar yalnızca bilgilendirme amaçlı değişikliklerdir. Güvenlik güncelleştirmesi dosyalarında veya algılama mantığında herhangi bir değişiklik yapılmamıştır. Güncelleştirmeler ilk sürümlerinden itibaren doğru şekilde sunulmuş oldukları için, bu güncelleştirmeleri daha önce başarıyla yüklemiş olan müşterilerin herhangi bir işlem gerçekleştirmeleri gerekmez.

*Built at 2014-04-18T01:50:00Z-07:00*
