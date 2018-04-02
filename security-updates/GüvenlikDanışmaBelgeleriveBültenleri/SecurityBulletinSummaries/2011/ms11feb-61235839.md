---
TOCTitle: 'MS11-FEB'
Title: Microsoft Security Bulletin Summary for Şubat 2011
ms:assetid: 'ms11-feb'
ms:contentKeyID: 61235839
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms11-feb(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary for Şubat 2011
==================================================

Yayım Tarihi: 8 Şubat 2011 Salı | Güncelleştirme Tarihi: 18 Mart 2011 Cuma

**Sürüm:** 4.0

Bu bülten özetinde Şubat 2011'de yayımlanan güvenlik bültenleri listelenir.

Şubat 2011 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 3 Şubat 2011'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 9 Şubat 2011 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Şubat Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032455047&eventcategory=4). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer Toplu Güvenlik Güncelleştirmesi (2482017)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen iki ve genel olarak duyurulan iki güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse veya özel hazırlanmış bir kitaplık dosyası yükleyen meşru bir HTML dosyasını açarsa uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, yerel kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;"><strong>Windows Kabuğu'nda Grafik İşleme Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2483185)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Kabuğu grafik işleyicisindeki genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir küçük resmi görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, oturum açan kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;"><strong>OpenType Küçük Yazı Tipi Biçimi (CFF) Sürücüsündeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2485376)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows OpenType Küçük Yazı Tipi Biçimi (CFF) sürücüsündeki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir CFF yazı tipinde işlenen içeriği görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu durumların hiçbirinde, saldırganın kullanıcıları özel hazırlanmış içeriği görüntülemeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi Web sitesine götüren bir bağlantıyı tıklatmalarını sağlayarak onları bu Web sitesini ziyaret etmeye ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;"><strong>Internet Information Services (IIS) FTP Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2489256)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Internet Information Services (IIS) FTP Hizmeti'ndeki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir FTP sunucusu özel hazırlanmış bir FTP komutu alırsa uzaktan kod yürütülmesine izin verebilir. FTP Hizmeti varsayılan olarak IIS'de yüklü değildir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;"><strong>Active Directory'deki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2478953)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Active Directory'deki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, etkilenen bir Active Directory sunucusuna özel hazırlanmış bir paket gönderirse hizmet reddine olanak verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için, etki alanına katılmış bilgisayarda geçerli yerel yönetici ayrıcalıkları olmalıdır.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;"><strong>Microsoft Visio'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2451879)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Visio'daki özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Visio dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, oturum açmış kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;"><strong>JScript ve VBScript Komut Dosyası Altyapılarındaki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (2475792)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, JScript ve VBScript komut dosyası altyapılarındaki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web sitesini ziyaret ederse bilginin açığa çıkmasına neden olabilir. Saldırganın, bu Web sitelerini ziyaret etmek için kullanıcıyı zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi Web sitesine götüren bir bağlantıyı tıklatmalarını sağlayarak onları bu Web sitesini ziyaret etmeye ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Bilginin Açığa Çıkması</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;"><strong>Windows İstemci Sunucu Çalışma Zamanı Alt Sistemi'ndeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2476687)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows XP ve Windows Server 2003'teki Microsoft Windows İstemci Sunucu Çalışma Zamanı Alt Sistemi'nde özel olarak bildirilen bir güvenlik açığını giderir.<br />
<br />
Güvenlik açığı, bir saldırgan kullanıcının sisteminde oturum açar ve saldırganın oturumu kapatıldıktan sonra kullanıcıların oturum açma kimlik bilgilerini edinmek üzere çalışmaya devam edecek şekilde özel hazırlanmış bir uygulamayı başlatırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2393802)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki genel olarak duyurulan ve özel olarak bildirilen birer güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan yerel olarak oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açıklarından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdek Modu Sürücülerindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2479628)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen beş güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan yerel olarak oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açıklarından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;"><strong>Kerberos'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2496930)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki özel olarak bildirilen ve genel olarak duyurulan birer güvenlik açığını giderir. Bu güvenlik açıklarından önem düzeyi daha yüksek olanı, kimliği doğrulanmış yerel bir saldırgan etki alanına katılmış bir bilgisayara kötü amaçlı bir hizmet yüklerse ayrıcalık yükselmesine izin verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;"><strong>Yerel Güvenlik Yetkilisi Alt Sistem Hizmeti'ndeki Güvenlik Açığı Yerel Olarak Ayrıcalık Yükselmesine İzin Verebilir (2478960)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows XP ve Windows Server 2003'teki Yerel Güvenlik Yetkilisi Alt Sistem Hizmeti'nde (LSASS) özel olarak bildirilen bir güvenlik açığını giderir.<br />
<br />
Bu güvenlik açığı, bir saldırgan sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
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
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, yararlanılabilirlik değerlendirmesi düzeylerine ve sonra da CVE Kimliklerine göre azalan sırayla listelenmektedir. Bültenlerde yalnızca önem derecesi Kritik veya Önemli olan güvenlik açıkları yer almaktadır.
  
**Bu tabloyu nasıl kullanabilirim?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Güvenlik Açığı Başlığı</th>
<th style="border:1px solid black;" >CVE Kimliği</th>
<th style="border:1px solid black;" >Yararlanma Dizini Değerlendirmesi</th>
<th style="border:1px solid black;" >Önemli Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;">Windows Kabuğu'nda Grafik İşleme Sırasında Taşma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3970">CVE-2010-3970</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur ve yararlanma kodu kullanılabilir</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">CSS'de Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3971">CVE-2010-3971</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur ve güvenlik açığından Internet ekosisteminde yararlanılmaktadır</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Sürücünün Windows Çekirdeği ile Düzgün Etkileşim Kurmaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4398">CVE-2010-4398</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;">CSRSS'de Ayrıcalık Yükselmesi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0030">CVE-2011-0030</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Başlatılmamış Belleğin Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0035">CVE-2011-0035</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Başlatılmamış Belleğin Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0036">CVE-2011-0036</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;">LSASS'de Uzunluğu Doğrulama Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0039">CVE-2011-0039</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Kerberos'da Anahtar Oluşturulmamış Sağlama Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0043">CVE-2011-0043</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Windows Çekirdeğinde Tamsayı Kesilmesi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0045">CVE-2011-0045</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Win32k'de Kullanıcı Girişinin Düzgün Doğrulanmaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0086">CVE-2011-0086</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Win32k'de Kullanıcı Girişinin Yeterince Doğrulanmaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0087">CVE-2011-0087</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Win32k'de Pencere Sınıfı İşaretçisinin Karıştırılması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0088">CVE-2011-0088</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Win32k'de Pencere Sınıfı İşaretçisinin Düzgün Doğrulanmaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0089">CVE-2011-0089</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Win32k'de Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0090">CVE-2011-0090</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Visio Nesnesinde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0092">CVE-2011-0092</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Visio'da Veri Türü Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0093">CVE-2011-0093</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;">IIS FTP Hizmeti'nde Öbek Arabelleği Taşması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3972">CVE-2010-3972</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur ve PoC kodu kullanıma sunulmuş olabilir</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;">OpenType Yazı Tipi Olarak Kodlanmış Karakter Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0033">CVE-2011-0033</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;">Komut Dosyası Altyapılarında Bilginin Açığa Çıkması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0031">CVE-2011-0031</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Bu bir bilginin açığa çıkması güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;">Active Directory'de SPN Doğrulaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0040">CVE-2011-0040</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><strong>Bu güvenlik açığı genel olarak duyurulmuştur</strong><br />
<br />
Bu bir hizmet reddi güvenlik açığıdır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Kerberos'da Kimlik Sahtekarlığı Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0091">CVE-2011-0091</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Bu yalnızca bir kimlik sahtekarlığı güvenlik açığıdır</td>
</tr>
</tbody>
</table>
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="12">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ae343de6-ec61-4891-b136-cfc4234d97d9)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=85bf88b7-2dd9-4204-8492-b2c1d8d2264e)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c72fbb97-2313-45f6-842d-99db373822dd)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bbea7ead-6c5c-4da8-aa03-a40325fd2de3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f86e9e64-801a-431a-b24e-772011dfa66d)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfa10178-9859-4e03-bedc-e3f5297a0251)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a511d33a-9ae0-46ee-a225-9d97390de7d1)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=56f4f43e-c313-49dc-a278-e3e8a83a907e)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=486d1969-6814-4556-8dc0-5bfbaee528b0)  
(KB2478971)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=541f228f-79b3-402a-8ff9-366c1e595227)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d431100d-a627-4ea0-b75b-2d4157e38df2)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a795de21-13f4-4035-a4d5-4257ddc92fe7)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=69dfa24b-7c56-4521-850c-1485b062154a)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bcb7217e-624a-4d61-86a1-f2440a1afd57)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=074396f0-a68c-4190-8dac-0b883d56e3f1)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f0b7b77-5b90-4a4b-97a4-0c1ce6a70126)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7273a85-ce96-464b-8c4f-2710701213e3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e80db313-b470-4d71-bc34-70bfbfb6579f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a210c796-7077-4617-a9a8-9ea99fe11a5e)  
(KB2478971)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82189bf2-3f34-4949-92da-eea98036d18e)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5e0f4bf2-f727-483a-af3a-9a2abf0c36bb)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=45e504d4-c17d-4b73-b08e-d9c0cb3f4918)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=74238e08-fae2-4f17-ac72-681226a53a40)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2aa94528-5063-427b-97f7-2a0a55cbb6bf)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a99c2b13-db81-4f18-9cf7-c20614ba0132)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=651c1f4f-4e69-4d17-8aa2-72681dfc5463)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aed08b96-24cc-4e23-8fd5-c7e52f8ef41a)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6bf2eeec-8225-477f-a606-263d3ee434d6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54fe2669-8a63-4d96-8b82-5b10f45b293e)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8a1e2675-0bf0-4d94-b48a-6e846dd6d9f5)  
(KB2478971)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e31e6b1-577e-468e-9c94-67227d2273c2)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0592b520-88d1-45bc-8b15-d3f0c8fa2181)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=29adcfb5-540f-4980-b2ca-9a22aa7bba13)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ebef4869-9812-46ce-9c01-2fb8c866ec90)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e740922-6ce4-46ec-a35e-e94201a9e398)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aeed45fb-9395-4c2b-a674-e38b04fe0914)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=ec962b0e-e951-4e70-8d97-8c2afd360c28)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ca7879e1-e295-445d-a658-0a31be1928cc)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ec544894-ee98-4a2b-ac4d-33b0c3754213)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4632e1ce-6ae8-431c-9104-9a8840e5ac63)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e79bbbd4-8d5a-4c4c-8427-21c14400f041)  
(KB2478971)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=76e3c229-d812-433c-ad05-7cbd1f9c6a6d)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b2298b32-238a-4970-bc1f-2ede51a6c361)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=c41a0094-204b-4d05-ab39-a32915201af1)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=a4f9ec46-35b2-44c9-abf6-647f7a474b99)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=bc09e42b-2eed-41b3-a03f-cb8cc94adfee)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=4ac66eae-e6d8-4e8b-b4ea-e7a77cc74db0)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=50855101-a15c-4c81-ad81-a7fe3f1d2026)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=fcd48499-1bb4-4304-b9cc-27d9d92e11cd)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=a09c3e6e-c55c-492a-b7ad-3e3d35711643)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=856fbcc2-ead9-4ec1-92dd-988e6d22dae9)  
(KB2478971)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=a0cde8d8-7c85-4fcb-bcf7-205064970b41)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="12">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b176777e-4897-4cf1-9fc0-dd608930bb4c)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=77971c3c-55ec-4a9c-bcb8-8fb8c61431e3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c18ecca-afb9-4738-bc7b-76a0e815dfb8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d60a2098-7351-4fce-83b2-2c1c3a24faa0)  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.0 için Microsoft FTP Hizmeti 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=c09ccc72-8f94-416b-9a7f-ed16e90342a2)<sup>[1]</sup>
(Önemli)  
[IIS 7.0 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=da9b7982-1c6b-45ac-8dd0-d7101bb83949)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=66978514-bb7f-42cc-9360-2fd1c686f4e6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6fb7ebcc-2052-457b-b5bc-1bbcb17696b9)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=20ad0136-c6df-4c7b-811f-d6b3dd9e2c56)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d3580784-aada-4118-b7f2-3a23aec2ed04)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62dc454f-4b1e-4ac0-8ffe-6c73112f8d4d)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=065ad8fe-1caf-488e-a2e1-96db29f2fa57)  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.0 için Microsoft FTP Hizmeti 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=e88d072f-0f5f-4c85-ad2f-91b9b8bf6b3a)<sup>[1]</sup>
(Önemli)  
[IIS 7.0 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=6e4b9878-b5d2-4025-8839-b41515932cf2)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8fdb8c37-1b22-457b-bdc0-21f6a5061dd3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88d68757-1ab0-4585-9578-52a474b10882)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ee61f0dd-9797-4e11-8281-a05b201d0c0b)\*\*  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ef1ae382-8835-4f60-83bd-e84a3400d55c)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=253c47a0-69ac-437a-ad3e-778c37fa37cb)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88ba83b9-c14e-499a-8335-04bac1c49c0c)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.0 için Microsoft FTP Hizmeti 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=3cc55af7-5cd9-4923-8ec5-462ff201d734)<sup>[1]</sup>\*  
(Önemli)  
[IIS 7.0 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=4dfa0a25-b7e3-4fb6-a351-58ec3f8a8435)<sup>[1]</sup>\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b37418a-e044-415e-b566-4507f157934a)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80494972-db45-475f-97cd-dac46b9486a1)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=558bc86a-a49d-4d6c-b5e4-f12956f6b61b)\*\*  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5607df02-93fa-45fe-a928-e5f6329851f3)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ec7101aa-96c2-4931-a3e4-0c55cbc74d9c)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c74d7f4-6372-4809-89b8-c79b05e54cdd)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.0 için Microsoft FTP Hizmeti 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=f485b30d-dcaf-47c3-ac62-982b14670a1f)<sup>[1]</sup>\*  
(Önemli)  
[IIS 7.0 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=a98a74c1-0c91-446d-b822-fe57ff06d90b)<sup>[1]</sup>\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=163d3aca-3703-452e-b1cb-73932e2bcf8c)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5597d449-17e3-440f-8b0e-56a902a96569)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8c2abba5-0597-4565-9b87-a37e574690e0)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e62493cb-8d25-4975-bbe6-a368e039872b)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=91d5d34b-9d7e-4e83-89a4-f1aa388dc4e4)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=55b07bc0-dff5-4cd7-87c9-c08e5a49197d)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d10eda21-b3c3-4d8e-8596-bc45e4165f93)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="12">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
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
32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=07aa7ffc-47c7-4611-b32c-ecb3fbcad32f)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1da57fbc-9ea4-4fc4-911d-d5c7825e012c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.5 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=9dabd1d1-3f1e-46d1-b171-aafd3f08d291)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Önemli)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=e1224c90-b0bc-4e4b-999a-efae327213b4)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=078fe6c0-1b2c-4896-a345-25cc1b1105e2)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ffed7c76-0b75-4f57-9b63-3961a8b449f6)  
(KB2425227)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2b8ffafe-78bb-4fa7-aea2-01208b6a3dfe)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=587adb89-2f6a-4893-9906-b6d6d9ada2bd)  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.5 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=66fb4efe-bcd3-4e90-8e35-b013e014a952)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Önemli)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=ddcf352e-742c-485e-9ed5-19cdba673562)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b42642b3-fb78-4700-bfe8-bfa997b90c16)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c26cebcf-683f-4a51-be75-76535fb979a7)  
(KB2425227)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-003**](http://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](http://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](http://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](http://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](http://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](http://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](http://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](http://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](http://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](http://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](http://go.microsoft.com/fwlink/?linkid=208395)
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
Yok
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
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
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
x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=38b67efb-dd4b-4e8c-8460-0f40f0367441)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=638318ed-4000-4b1a-bb4b-65b795f59784)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.5 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=1e075f57-1723-4933-9b8e-7bce4a44a1c1)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Orta)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=70f5056a-72ad-46ff-a43f-ee151639b9a7)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d2c53f44-12eb-4293-9fa5-2a14075b636e)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46bb3ef1-24c3-41cb-8141-0fdbd85093f7)\*  
(KB2425227)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=0e41cbe5-5e5e-4ece-a71a-71f4b6319f0d)  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4688ea0d-a467-4f24-ac52-104d05c8cae8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[IIS 7.5 için Microsoft FTP Hizmeti 7.5](http://www.microsoft.com/downloads/details.aspx?familyid=bfddd539-c64f-4467-88ee-6bdfe645b478)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[JScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Orta)  
[VBScript 5.8](http://www.microsoft.com/downloads/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=1646b3a5-714f-4ea5-b109-566fa9b933b6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8c6bf720-f544-4f58-9b1c-2399957ec43d)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=01737933-e7de-451b-b02f-b7ca24693965)  
(KB2425227)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Notlar**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS11-004 için Not**

<sup>[1]</sup>Bu işletim sistemi için varsayılan FTP Hizmeti değildir

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Office Programları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-008**](http://go.microsoft.com/fwlink/?linkid=204799)
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
Microsoft Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=273d8078-0dc7-43d8-bcae-54c811e49e0e)  
(KB2434711)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1067eaa-d18d-4bff-a02e-1d990c36ca7f)  
(KB2434733)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=097a642b-b786-4724-a907-79f37cded836)  
(KB2434737)  
(Önemli)
</td>
</tr>
</table>
 

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

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) Web sitesini ziyaret edin.

**System Center Configuration Manager 2007**

Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, kuruluş genelindeki BT sistemlerine yönelik güncelleştirmeleri teslim etme ve yönetme görevini kolaylaştırır. Configuration Manager 2007 ile, BT yöneticileri Microsoft ürünlerine yönelik güncelleştirmeleri masaüstü bilgisayarlar, dizüstü bilgisayarlar, sunucular ve mobil aygıtlar gibi çeşitli aygıtlara teslim edebilirler.

Configuration Manager 2007'deki otomatik güvenlik açığı değerlendirmesi, güncelleştirme gereksinimini belirler ve önerilen eylemleri bildirir. Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, BT yöneticileri tarafından dünya genelinde kullanılan ve zaman içinde kendini kanıtlamış bir güncelleştirme altyapısı olan Microsoft Windows Software Update Services'a (WSUS) dayalıdır. Yöneticilerin güncelleştirmeleri dağıtmak üzere Configuration Manager 2007'yi nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Yazılım Güncelleştirme Yönetimi](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Configuration Manager hakkında daha fazla bilgi için, [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx)'ı sayfasını ziyaret edin.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir.

**Not** System Management Server 2003, 12 Ocak 2010'dan itibaren temel destek dışında kalmıştır. Ürün ömrü hakkında daha fazla bilgi için, [Microsoft Destek Ömrü](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle) Web sitesini ziyaret edin. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; önceki bölüm olan **System Center Configuration Manager 2007** konusuna bakın.

Yöneticilerin güvenlik güncelleştirmelerini dağıtmak üzere SMS 2003'ü nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Microsoft Systems Management Server 2003 Senaryoları ve Yordamları: Yazılım Dağıtımı ve Düzeltme Eki Yönetimi](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). SMS hakkında bilgi için, [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx)'ı ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler bu güncelleştirmeleri yüklemek için, Elevated Rights Deployment Tool'u kullanabilirler ([SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en) içinde bulunur).

**Güncelleştirme Uyumluluğu Değerlendiricisi ve Uygulama Uyumluluğu Araç Takımı**

Güncelleştirmeler genelde uygulamalarınızın çalışması için gerekli olan aynı dosyalara ve kayıt defteri ayarlarına yazar. Bu durum da uyumsuzlukları tetikleyebilir ve güvenlik güncelleştirmelerinin dağıtılması için gereken zamanı artırabilir. [Uygulama Uyumluluğu Araç Takımı](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) ile birlikte gelen [Güncelleştirme Uyumluluğu Değerlendiricisi](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) bileşenlerini kullanarak, Windows güncelleştirmelerinin yüklü uygulamalara göre sınanması ve doğrulanması sürecini hızlandırabilirsiniz.

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Microsoft Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Güncelleştirmeler

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

-   [Trend Micro](http://www.trendmicro.com) için çalışan Yuki Chen, MS11-003'te açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan SkyLined, MS11-003'te açıklanan sorunu bildirdiği için
-   [Fortinet bünyesindeki FortiGuard Labs](http://www.fortiguard.com/) için çalışan Haifei Li, MS11-003'te açıklanan sorunu bildirdiği için
-   Kobi Pariente ve Yaniv Miron, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-006'da açıklanan sorunu bildirdikleri için
-   Procyun, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS11-008'de açıklanan sorunu bildirdikleri için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Xin Ouyang, MS11-008'de açıklanan iki sorunu bildirdiği için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, MS11-009'da açıklanan sorunu bildirdiği için
-   Sihan Qing (Profesör), Weiping Wen (Doçent), Liang Yin ve Husheng Zhou (Lisans öğrencileri), [Bilişim Güvenliği Bölümü, Pekin Üniversitesi](http://www.ss.pku.edu.cn/en/), MS11-010'da açıklanan sorunu bildirdikleri için
-   [360safe](http://www.360.cn) için çalışan Zhengwenbin, MS11-011'de açıklanan sorunu bildirdiği için
-   Guo Bojun, MS11-011'de açıklanan sorunu bildirdiği için
-   Wei Zhang, MS11-011'de açıklanan sorunu bildirdiği için
-   [Prevx](http://www.prevx.com/) için çalışan Marco Giuliani, MS11-011'de açıklanan sorun konusunda bizimle birlikte çalıştığı için
-   std\_logic, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS11-011'de açıklanan sorunu bildirdikleri için
-   [Norman](http://www.norman.com) için çalışan Tarjei Mandt, MS11-012'de açıklanan beş sorunu bildirdiği için
-   [MIT Kerberos Team](http://web.mit.edu/kerberos), MS11-013'te açıklanan sorunu bildirdikleri için
-   [iSEC Partners](http://www.isecpartners.com/) için çalışan Scott Stender, MS11-013'te açıklanan sorunu bildirdiği için
-   Primavera BSS için çalışan güvenlik sınayıcısı Jorge Moura, MS11-014'te açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (8 Şubat 2011): Bülten Özeti yayımlandı.
-   V1.1 (9 Şubat 2011): MS11-013'te, CVE-2011-0091 için Yararlanma Dizini Değerlendirmesi "3 – İşlevsel bir yararlanma kodu olasılığı düşük" olarak düzeltildi. Bu yalnızca bilgilendirme amaçlı bir değişikliktir.
-   V2.0 (8 Mart 2011): MS11-003, MS11-004, MS11-007 ve MS11-009 için Etkilenen Yazılımlar arasında 32-bit sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 bulunduğu açıklığa kavuşturuldu. Daha fazla bilgi için, bu bültenlerin Güncelleştirme Hakkında SSS bölümüne bakın.
-   V3.0 (16 Mart 2011): MS11-013 için Etkilenen Yazılımlar arasında 32-bit sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 bulunduğu açıklığa kavuşturuldu. Daha fazla bilgi için, bu bültenin Güncelleştirme Hakkında SSS bölümüne bakın.
-   V4.0 (18 Mart 2011): MS11-012 için Etkilenen Yazılımlar arasında 32-bit sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 bulunduğu açıklığa kavuşturuldu. Daha fazla bilgi için, bu bültenin Güncelleştirme Hakkında SSS bölümüne bakın.

*Built at 2014-04-18T01:50:00Z-07:00*
