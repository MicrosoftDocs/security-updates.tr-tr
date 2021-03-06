---
TOCTitle: 'MS12-JUN'
Title: Microsoft Güvenlik Bülteni Haziran 2012 Özeti
ms:assetid: 'ms12-jun'
ms:contentKeyID: 61235851
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms12-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Haziran 2012 Özeti
=============================================

Yayım Tarihi: 12 Haziran 2012 Salı

**Sürüm:** 1.0

Bu bülten özetinde Haziran 2012'de yayımlanan güvenlik bültenleri listelenir.

Haziran 2012 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 7 Haziran 2012'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://go.microsoft.com/fwlink/?linkid=217213).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 13 Haziran 2012 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Haziran Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499671). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246927"><strong>MS12-036</strong></a></td>
<td style="border:1px solid black;"><strong>Uzak Masaüstü'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2685939)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Uzak Masaüstü Protokolü'ndeki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan etkilenen bir sisteme özel hazırlanmış bir dizi RDP paketi gönderirse uzaktan kod yürütülmesine izin verebilir. Varsayılan olarak, Uzak Masaüstü Protokolü (RDP) herhangi bir Windows işletim sisteminde etkin değildir. RDP'nin etkinleştirilmemiş olduğu sistemler risk altında değildir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=249045"><strong>MS12-037</strong></a></td>
<td style="border:1px solid black;"><strong>Internet Explorer Toplu Güvenlik Güncelleştirmesi (2699988)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Internet Explorer'daki genel olarak duyurulan bir ve özel olarak bildirilen on iki güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, geçerli kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251095"><strong>MS12-038</strong></a></td>
<td style="border:1px solid black;"><strong>.NET Framework'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2706726)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft .NET Framework'teki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir web sayfasını XAML Tarayıcı Uygulamaları (XBAP) çalıştırabilen bir web tarayıcısı kullanarak görüntülerken istemci sistemde uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Bu güvenlik açığı, Windows .NET uygulamaları tarafından Kod Erişimi Güvenliği (CAS) kısıtlamalarını atlamak için de kullanılabilir. Web'de gezinme tabanlı saldırı senaryosunda, bir saldırgan bu açıktan yararlanmak için kullanılan bir web sayfası içeren bir web sitesi barındırabilir. Ayrıca, kullanıcı tarafından sağlanan içeriği veya reklamları kabul eden ya da barındıran güvenliği aşılmış web sitelerinde, bu güvenlik açığından yararlanılabilecek özel hazırlanmış içerik bulunabilir. Ancak bu durumların hiçbirinde, saldırganın, bu web sitelerini ziyaret etmek için kullanıcıyı zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi web sitesine götüren bir bağlantıyı tıklatmalarını sağlayarak onları bu web sitesine çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=252488"><strong>MS12-039</strong></a></td>
<td style="border:1px solid black;"><strong>Lync'teki</strong> <strong>Güvenlik Açıkları</strong> <strong>Uzaktan Kod Yürütülmesine İzin Verebilir (2707956)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Lync'teki genel olarak duyurulan bir ve özel olarak bildirilen üç güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış TrueType yazı tiplerinin bulunduğu bir paylaşılan içeriği görüntülerse uzaktan kod yürütülmesine izin verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Lync</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251612"><strong>MS12-040</strong></a></td>
<td style="border:1px solid black;"><strong>Microsoft Dynamics AX Enterprise Portal'daki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2709100)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Dynamics AX Enterprise Portal'daki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir URL'yi tıklatırsa veya özel hazırlanmış bir web sitesini ziyaret ederse ayrıcalık yükselmesine izin verebilir. E-posta tabanlı saldırı senaryosunda, saldırgan özel hazırlanmış URL'yi içeren bir e-posta iletisini hedeflenen Microsoft Dynamics AX Enterprise Portal sitesinin kullanıcısına gönderip kullanıcıyı özel hazırlanmış bu URL'yi tıklatmaya ikna ederek bu güvenlik açığından yararlanabilir. Internet Bölgesi'nde bulunan bir Microsoft Dynamics AX Enterprise Portal sitesine gözatan Internet Explorer 8 ve Internet Explorer 9 kullanıcıları daha az risk altındadır. Internet Explorer 8 ve Internet Explorer 9'daki XSS Filtresi varsayılan olarak Internet Bölgesi'nde bu saldırıyı engeller. Ancak Internet Explorer 8 ve Internet Explorer 9'daki XSS Filtresi varsayılan olarak Intranet Bölgesi'nde etkinleştirilmemiş durumdadır.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Dynamics AX</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251707"><strong>MS12-041</strong></a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdek Modu Sürücülerindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2709162)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen beş güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açıklarından birinden yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=252515"><strong>MS12-042</strong></a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2711167)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki özel olarak bildirilen ve genel olarak duyurulan birer güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan etkilenen sistemde oturum açar ve güvenlik açığından yararlanacak şekilde özel olarak hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
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
  
| Bülten Kimliği                                                | Güvenlik Açığı Başlığı                                           | CVE Kimliği                                                                      | En Son Yazılım Sürümü için Yararlanma Değerlendirmesi                                             | Yazılımın Eski Sürümleri için Yararlanma Değerlendirmesi                                          | Hizmet Reddi Yararlanma Değerlendirmesi | Önemli Notlar                                                                                                                               |  
|---------------------------------------------------------------|------------------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|-----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------|  
| [**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927) | Uzak Masaüstü Protokolü Güvenlik Açığı                           | [CVE-2012-0173](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0173) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Ortala Öğesinde Uzaktan Kod Yürütme Güvenlik Açığı               | [CVE-2012-1523](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1523) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | HTML Korunması Güvenlik Açığı                                    | [CVE-2012-1858](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1858) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Uygulanamaz                             | Bu, bir bilginin açığa çıkması güvenlik açığıdır. [MS12-039](http://go.microsoft.com/fwlink/?linkid=252488) da bu güvenlik açığını giderir. |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Boş Baytta Bilginin Açığa Çıkması Güvenlik Açığı                 | [CVE-2012-1873](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1873) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Uygulanamaz                             | Bu, bir bilginin açığa çıkması güvenlik açığıdır.                                                                                           |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Geliştirici Araç Çubuğunda Uzaktan Kod Yürütme Güvenlik Açığı    | [CVE-2012-1874](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1874) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Aynı Kimlik Özelliğinde Uzaktan Kod Yürütme Güvenlik Açığı       | [CVE-2012-1875](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1875) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | Microsoft bu güvenlik açığından yararlanmaya çalışan sınırlı sayıda saldırı olduğunu bilmektedir.                                           |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Sütun Öğesinde Uzaktan Kod Yürütme Güvenlik Açığı                | [CVE-2012-1876](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1876) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | Başlık Öğesini Değiştirmede Uzaktan Kod Yürütme Güvenlik Açığı   | [CVE-2012-1877](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1877) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | OnBeforeDeactivate Olayında Uzaktan Kod Yürütme Güvenlik Açığı   | [CVE-2012-1878](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1878) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | insertAdjacentText Öğesinde Uzaktan Kod Yürütme Güvenlik Açığı   | [CVE-2012-1879](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1879) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | insertRow Öğesinde Uzaktan Kod Yürütme Güvenlik Açığı            | [CVE-2012-1880](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1880) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045) | OnRowsInserted Olayında Uzaktan Kod Yürütme Güvenlik Açığı       | [CVE-2012-1881](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1881) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Geçici                                  | (Yok)                                                                                                                                       |  
| [**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095) | .NET Framework'te Bellek Erişimi Güvenlik Açığı                  | [CVE-2012-1855](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1855) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Uygulanamaz                             | (Yok)                                                                                                                                       |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | TrueType Yazı Tipini Ayrıştırma Güvenlik Açığı                   | [CVE-2011-3402](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3402) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Etkilenmez                                                                                        | Kalıcı                                  | Bu güvenlik açığı genel olarak duyurulmuştur.                                                                                               |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | TrueType Yazı Tipini Ayrıştırma Güvenlik Açığı                   | [CVE-2012-0159](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0159) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Etkilenmez                                                                                        | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | Lync'te Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı  | [CVE-2012-1849](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1849) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Etkilenmez                                                                                        | Uygulanamaz                             | (Yok)                                                                                                                                       |  
| [**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488) | HTML Korunması Güvenlik Açığı                                    | [CVE-2012-1858](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1858) | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | [3](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı düşük  | Uygulanamaz                             | Bu, bir bilginin açığa çıkması güvenlik açığıdır. [MS12-037](http://go.microsoft.com/fwlink/?linkid=249045) de bu güvenlik açığını giderir. |  
| [**MS12-040**](http://go.microsoft.com/fwlink/?linkid=251612) | Dynamics AX Enterprise Portal XSS Güvenlik Açığı                 | [CVE-2012-1857](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1857) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Etkilenmez                                                                                        | Uygulanamaz                             | (Yok)                                                                                                                                       |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Dize Atomunda Sınıf Adını İşleme Güvenlik Açığı                  | [CVE-2012-1864](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1864) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Dize Atomunda Sınıf Adını İşleme Güvenlik Açığı                  | [CVE-2012-1865](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1865) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Pano Biçiminde Atom Adını İşleme Güvenlik Açığı                  | [CVE-2012-1866](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1866) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Yazı Tipi Kaynağında Refcount Tamsayı Taşması Güvenlik Açığı     | [CVE-2012-1867](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1867) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707) | Win32k.sys Dosyasında Yarış Durumu Güvenlik Açığı                | [CVE-2012-1868](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1868) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515) | Kullanıcı Modu Zamanlayıcısı'nda Bellek Bozulması Güvenlik Açığı | [CVE-2012-0217](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0217) | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Etkilenmez                                                                                        | Kalıcı                                  | (Yok)                                                                                                                                       |  
| [**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515) | BIOS ROM'unun Bozulması Güvenlik Açığı                           | [CVE-2012-1515](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1515) | Etkilenmez                                                                                        | [1](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu olasılığı yüksek | Kalıcı                                  | Bu güvenlik açığı genel olarak duyurulmuştur.                                                                                               |
  
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
<th colspan="6">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fd2216eb-283b-4a23-b259-018a7fa5fe47)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=7f222e05-2a8d-4099-851f-2044811f7425)  
(KB2699988)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=07c75ac6-f92a-4204-aa58-bdf8c033df9e)  
(KB2699988)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5bc1656f-cf1d-4f77-a078-a8602401b8e1)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a399bd47-ffe1-4476-932c-9c119496222a)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0efff733-4c8d-4fce-8de3-28465c6b762b)  
(KB2707511)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e354955-32ae-447c-b16f-960acc01773b)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=57e8bf9d-97c3-4166-a5d4-6b0c99afc6a1)  
(KB2699988)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b35e90b-145d-44c2-a8bc-4f9108d46fa1)  
(KB2699988)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0a386b16-74f7-4d36-93d0-75e7da9bf9b5)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bdb356db-bd36-4159-8e64-ecdb3dfc61bf)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam** **Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8e856fec-9f05-49b7-91b6-11c2636a2f1d)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b1dcc826-7e96-464b-830e-39946e7802aa)  
(KB2699988)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=de828031-1ace-43df-80f2-db7d503fb0a2)  
(KB2699988)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4e6e5589-b767-4e8a-b8b3-df7b97e002e5)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0b39b00-d7db-4008-8310-1258e84a72a2)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=855611a1-91ad-4d22-8c1c-fdcd6af4cef0)  
(KB2707511)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b63fa4d-b42e-43ca-9f2c-cf60c37731a5)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b060e03b-e63e-446b-9cfd-ea4e1e9383a6)  
(KB2699988)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a36f7ffe-d537-4f9e-b676-22a24f50c089)  
(KB2699988)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b1acb2f0-63ba-4524-94cf-42b3534e21e7)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ed7359ce-13e8-42b2-956d-e8be534583aa)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=7dfdc5dc-54b0-49e3-bf5a-bbc40b0f159f)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=893667c4-ef9f-48d3-ab18-a0df51bd3dcc)  
(KB2699988)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=30a9d518-8067-44f4-90fd-09fec8a0c883)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3206a637-a25e-4cc7-830c-08454ae86f0f)  
(KB2686828)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=2317c8d9-cae8-497b-952e-78eb4a6d585c)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="6">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f55b62bf-0571-4888-9061-3f7cc75d7f17)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=16f4404e-e6d6-4bde-af15-3bb692412213)  
(KB2699988)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=610e753a-21db-43e6-bc42-3e1227fa4bb1)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=828fdb71-747b-481d-9683-895325331478)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9188f1eb-b568-4a99-9b39-745c760a693d)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab06290c-4f57-4349-8abd-a382b9044631)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=993c5bc4-8903-4c8c-bbc9-da2e47d959f9)  
(KB2699988)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=87100a7e-7feb-4a18-b7aa-04fdd2d6ef52)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7b551d67-e0f1-498a-ac4f-06376a0fcf18)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b94ae42-2882-444c-ad5e-74e34b805006)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8dcb487-0df7-46f4-8726-bd58e2722812)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e7f9ad40-d515-4224-90ff-4bd4bff9180f)  
(KB2699988)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c4eaeff8-7b7a-4418-a479-09b2146df2bf)  
(KB2699988)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=a20c839c-ce3b-46a5-becb-588de404878d)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6398a156-9618-4ca4-95bc-d36ecacf0745)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40c16540-7839-412c-b474-892292a96fa5)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7420c9f3-8f7e-4823-aaba-b14b957408d8)  
(KB2699988)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=fd5308b7-7430-4713-922c-f06c46886fad)  
(KB2699988)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=1a737d87-0689-470b-8fc0-8c874af18794)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc4412ee-8cb8-42e9-96fe-0be49af149b2)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c4b8af1c-b483-4aed-9be5-b0f1698b2c28)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=472842c4-5fe7-4d4c-a927-05be030b5b4e)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f4dadc9-733d-46ba-a6a8-92e7b4f49a7b)  
(KB2686833)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=098607b3-9424-4440-8832-fc1de010977e)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="6">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=e8549243-e6bf-4007-9bc3-d9c2a24936ef)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=595e72c3-f195-4f93-b24e-afe444abd628)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=48ca08c8-78cc-4b09-a0ec-bcd208668620)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=605f64bd-0615-47d8-bb32-6bc3e80da4a7)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e8549243-e6bf-4007-9bc3-d9c2a24936ef)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=595e72c3-f195-4f93-b24e-afe444abd628)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=48ca08c8-78cc-4b09-a0ec-bcd208668620)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=605f64bd-0615-47d8-bb32-6bc3e80da4a7)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=7f0f54e4-b9d9-45d8-bc58-05d7e7b75f07)  
(KB2685939)  
(Orta)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=30feb2fe-b19b-4d02-8c5b-4499dd6905d1)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bf8dbfee-573b-4d45-a752-90e1d485e503)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=3c77ca1f-2eec-4f95-a769-973b75af184c)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=c2b47091-534f-41c3-a229-b5a9ec4b64bb)  
(KB2709715)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7f0f54e4-b9d9-45d8-bc58-05d7e7b75f07)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=30feb2fe-b19b-4d02-8c5b-4499dd6905d1)  
(KB2699988)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=bf8dbfee-573b-4d45-a752-90e1d485e503)  
(KB2699988)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3c77ca1f-2eec-4f95-a769-973b75af184c)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c2b47091-534f-41c3-a229-b5a9ec4b64bb)  
(KB2709715)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9464b044-e40b-4300-97b8-dc3a13c85929)  
(KB2699988)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c8b04-b749-4c6c-8b9f-244abc5f8ecf)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=9464b044-e40b-4300-97b8-dc3a13c85929)  
(KB2699988)  
(Orta)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c8b04-b749-4c6c-8b9f-244abc5f8ecf)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=8ecc5d12-9921-4d04-a04c-d69e8f4349dc)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=40302688-fcda-489c-87c4-480d3b9d754c)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=039ddfe1-3ce5-48d8-8cb4-65481da3f29c)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8ecc5d12-9921-4d04-a04c-d69e8f4349dc)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=40302688-fcda-489c-87c4-480d3b9d754c)  
(KB2699988)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=039ddfe1-3ce5-48d8-8cb4-65481da3f29c)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="6">
Sunucu Çekirdeği yükleme seçeneği
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-036**](http://go.microsoft.com/fwlink/?linkid=246927)
</td>
<td style="border:1px solid black;">
[**MS12-037**](http://go.microsoft.com/fwlink/?linkid=249045)
</td>
<td style="border:1px solid black;">
[**MS12-038**](http://go.microsoft.com/fwlink/?linkid=251095)
</td>
<td style="border:1px solid black;">
[**MS12-041**](http://go.microsoft.com/fwlink/?linkid=251707)
</td>
<td style="border:1px solid black;">
[**MS12-042**](http://go.microsoft.com/fwlink/?linkid=252515)
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
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8dcb487-0df7-46f4-8726-bd58e2722812)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6398a156-9618-4ca4-95bc-d36ecacf0745)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=40c16540-7839-412c-b474-892292a96fa5)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc4412ee-8cb8-42e9-96fe-0be49af149b2)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=68d3694f-fcc9-49e6-93c2-0568b7280236)  
(KB2686830)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=12740f33-579c-4a75-bec0-9a69e9c64266)  
(KB2685939)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=30b16454-cf11-49e1-9032-71c8d2b5d44b)  
(KB2686831)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=fef24f6c-d81a-4078-af5d-dc7d0b53d145)<sup>[1]</sup>
(KB2686827)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34d16819-4a2f-42e2-a4f9-88995719cbe8)  
(KB2709162)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1696726a-ed04-4c0e-b9b6-3ac4ac775c4c)  
(KB2709715)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-038** **için** **Not**

<sup>[1]</sup>**.NET Framework 4 ve .NET Framework 4 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4 ve .NET Framework 4 İstemci Profili. .NET Framework 4 İstemci Profili, .NET Framework 4'ün bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4'ü hem de .NET Framework 4 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

#### Microsoft İletişim Platformları ve Yazılımları

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Communicator
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488)
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
Microsoft Communicator 2007 R2
</td>
<td style="border:1px solid black;">
[Microsoft Communicator 2007 R2](http://www.microsoft.com/downloads/details.aspx?familyid=75eea324-689a-4892-bdd9-03ef399c4cba)  
(KB2708980)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Lync
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-039**](http://go.microsoft.com/fwlink/?linkid=252488)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 (32-bit)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 (32-bit)](http://www.microsoft.com/downloads/details.aspx?familyid=425406ea-28b9-46f7-8c49-0c7ea46f16e3)  
(KB2693282)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 (64-bit)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 (64-bit)](http://www.microsoft.com/downloads/details.aspx?familyid=06e5285f-1947-4409-b608-e0a145fadba4)  
(KB2693282)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendee
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendee](http://www.microsoft.com/downloads/details.aspx?familyid=c40f0d38-af90-4966-a0f0-346fa48683d0)  
(yönetici düzeyinde yükleme)  
(KB2696031)  
(Önemli)  
[Microsoft Lync 2010 Attendee](http://www.microsoft.com/downloads/details.aspx?familyid=ad864c0e-5850-44a3-b74f-5980a998a384)<sup>[1]</sup>
(kullanıcı düzeyinde yükleme)  
(KB2693283)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendant (32-bit)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendant (32-bit)](http://www.microsoft.com/downloads/details.aspx?familyid=fe7ad0f9-ee84-4cda-b252-a8d31ead5053)  
(KB2702444)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Lync 2010 Attendant (64-bit)
</td>
<td style="border:1px solid black;">
[Microsoft Lync 2010 Attendant (64-bit)](http://www.microsoft.com/downloads/details.aspx?familyid=fe7ad0f9-ee84-4cda-b252-a8d31ead5053)  
(KB2702444)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-039 için** **Not**

<sup>[1]</sup>Bu güncelleştirme yalnızca Microsoft Yükleme Merkezi'nden edinilebilir.

#### Microsoft Kurumsal Kaynak Planlama (ERP) Çözümleri

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Dynamics ERP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-040**](http://go.microsoft.com/fwlink/?linkid=251612)
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
Microsoft Dynamics AX 2012
</td>
<td style="border:1px solid black;">
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=45df362d-8fed-4d99-91c1-81c61878300a)<sup>[1]</sup>
(KB2706738)  
(Önemli)  
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=780ddcef-19da-44c4-beca-d10b652cd22a)<sup>[1]</sup>
(KB2710639)  
(Önemli)  
[Microsoft Dynamics AX 2012 Enterprise Portal](http://www.microsoft.com/downloads/details.aspx?familyid=41dc5958-c224-40f9-89c2-179607a8ee2a)<sup>[1]</sup>
(KB2711239)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-040 için Not**

<sup>[1]</sup>Bu güncelleştirme yalnızca Microsoft Yükleme Merkezi, Microsoft Dynamics Müşteri Kaynağı ve Microsoft Dynamics İş Ortağı Kaynağı web sitelerinden edinilebilir.

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

**SystemCenter Configuration Manager**

System Center Configuration Manager'daki Yazılım Güncelleştirme Yönetimi, kuruluş genelindeki BT sistemlerine yönelik güncelleştirmeleri teslim etme ve yönetme görevini kolaylaştırır. System Center Configuration Manager ile, BT yöneticileri Microsoft ürünlerine yönelik güncelleştirmeleri masaüstü bilgisayarlar, dizüstü bilgisayarlar, sunucular ve mobil aygıtlar gibi çeşitli aygıtlara teslim edebilirler.

System Center Configuration Manager'deki otomatik güvenlik açığı değerlendirmesi, güncelleştirme gereksinimini belirler ve önerilen eylemleri bildirir. Software Update Management in System Center'deki Yazılım Güncelleştirme Yönetimi, BT yöneticileri tarafından dünya genelinde kullanılan ve zaman içinde kendini kanıtlamış bir güncelleştirme altyapısı olan Microsoft Windows Software Update Services'a (WSUS) dayalıdır. Yöneticilerin güncelleştirmeleri dağıtmak üzere System Center Configuration Manager'ı nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Yazılım Güncelleştirme Yönetimi](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). System Center Configuration Manager hakkında daha fazla bilgi için, [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx)'ı sayfasını ziyaret edin.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir.

**Not** System Management Server 2003, 12 Ocak 2010'dan itibaren temel destek dışında kalmıştır. Ürün ömrü hakkında daha fazla bilgi için, [Microsoft Destek Ömrü](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle) Web sitesini ziyaret edin. SMS'nin yeni sürümü olan System Center Configuration Manager artık kullanılabilir; önceki bölüm olan **System Center Configuration Manager** konusuna bakın.

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

-   Anonim bir araştırmacı, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-037'de açıklanan sorunu bildirdikleri için
-   [IBM Security Systems - Application Security](http://blog.watchfire.com/) için çalışan Adi Cohen, MS12-037'de açıklanan sorunu bildirdiği için
-   Masato Kinugawa, MS12-037'de açıklanan sorunu bildirdiği için
-   LinkedIn için çalışan Roman Shafigullin, MS12-037'de açıklanan sorunu bildirdiği için
-   [VulnHunt](http://www.vulnhunt.com) bünyesindeki Code Audit Labs, MS12-037'de açıklanan sorunu bildirdikleri için
-   [VulnHunt](http://www.vulnhunt.com) için çalışan Dark Son, MS12-037'de açıklanan sorunu bildirdiği için
-   [Qihoo 360 Security Center](http://www.360.cn/), MS12-037'de açıklanan sorun konusunda bizimle birlikte çalıştıkları için
-   McAfee Labs için çalışan Yichong Lin, MS12-037'de açıklanan sorun konusunda bizimle çalıştığı için
-   [Google Inc.](http://www.google.com/), MS12-037'de açıklanan sorun konusunda bizimle çalıştıkları için
-   [VUPEN Security](http://www.vupen.com), [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS12-037'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-037'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-037'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-037'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-037'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-037'de açıklanan sorunu bildirdikleri için
-   Vitaliy Toropov, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS12-038'de açıklanan sorunu bildirdikleri için
-   Secunia SVCRP aracılığıyla hamburgers maccoy, MS12-039'da açıklanan sorunu bildirdiği için
-   [IBM Security Systems - Application Security](http://blog.watchfire.com/) için çalışan Adi Cohen, MS12-039'da açıklanan sorunu bildirdiği için
-   Alin Rad Pop, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS12-039'da açıklanan sorunu bildirdikleri için
-   Finian Mackin, MS12-040'ta açıklanan sorunu bildirdiği için
-   [Azimuth Security](http://www.azimuthsecurity.com/) için çalışan Tarjei Mandt, MS12-041'de açıklanan üç sorunu bildirdiği için
-   [Google Inc.](http://www.google.com) için çalışan [Mateusz "j00ru" Jurczyk](http://j00ru.vexillium.org), MS12-041'de açıklanan sorunu bildirdiği için
-   [Bromium](http://www.bromium.com/) için çalışan Rafal Wojtczuk ve [SUSE](http://www.suse.com/) için çalışan Jan Beulich, MS12-042'de açıklanan sorunu bildirdikleri için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   BT uzmanları için güvenlik çözümleri: [TechNet Security Sitesinin Sorun Giderme ve Destek Bölümü](http://technet.microsoft.com/security/bb980617.aspx)
-   Windows çalışan bilgisayarınızın virüslere ve kötü amaçlı yazılımlara karşı korunmasına yardım edin: [Virüs ve Güvenlik Çözüm Merkezi](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Ülkenize göre yerel destek: [Uluslararası Destek](http://support.microsoft.com/common/international.aspx)

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (12 Haziran 2012): Bülten Özeti yayımlandı.

*Built at 2014-04-18T01:50:00Z-07:00*
