---
TOCTitle: 'MS11-JUN'
Title: Microsoft Güvenlik Bülteni Haziran 2011 Özeti
ms:assetid: 'ms11-jun'
ms:contentKeyID: 61235842
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms11-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Haziran 2011 Özeti
=============================================

Yayım Tarihi: 14 Haziran 2011 Salı | Güncelleştirme Tarihi: 18 Ocak 2012 Çarşamba

**Sürüm:** 3.1

Bu bülten özetinde Haziran 2011'de yayımlanan güvenlik bültenleri listelenir.

Haziran 2011 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 9 Haziran 2011'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://go.microsoft.com/fwlink/?linkid=217213).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 15 Haziran 2011 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Haziran Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455073&eventcategory=4). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212284">MS11-038</a></td>
<td style="border:1px solid black;"><strong>OLE Otomasyonundaki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2476490)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows Nesne Bağlama ve Katıştırma (OLE) Otomasyonu'ndaki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Windows Meta Dosyası (WMF) resminin bulunduğu bir Web sitesini ziyaret ederse uzaktan kod yürütülmesine izin verebilir. Ancak bu durumların hiçbirinde, saldırganın kullanıcıları bu tür bir Web sitesini ziyaret etmeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Anlık İleti isteğindeki bağlantıyı tıklatmalarını sağlayarak onları kötü amaçlı bir Web sitesine çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212287">MS11-039</a></td>
<td style="border:1px solid black;"><strong>.NET Framework ve Microsoft Silverlight'taki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2514842)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft .NET Framework ve Microsoft Silverlight'taki özel olarak bildirilen bir güvenlik açığını gidermektedir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web sayfasını XAML Tarayıcı Uygulamaları (XBAP) veya Silverlight uygulamaları çalıştırabilen bir Web tarayıcısı kullanarak görüntülerken istemci sistemde uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Güvenlik açığı, IIS çalıştıran bir sunucu sisteminde, söz konusu sunucu ASP.NET sayfalarının işlenmesine izin veriyorsa ve saldırgan özel hazırlanmış bir ASP.NET sayfasını başarıyla sunucuya yükleyip çalıştırırsa (Web barındırma senaryosunda bu durum geçerli olabilir) uzaktan kod yürütülmesine izin verebilmektedir. Bu güvenlik açığı, Windows .NET uygulamaları tarafından Kod Erişimi Güvenliği (CAS) kısıtlamalarını atlamak için de kullanılabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217470">MS11-040</a></td>
<td style="border:1px solid black;"><strong>Threat Management Gateway Güvenlik Duvarı İstemcisi'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2520426)</strong><br />
<br />
Bu güvenlik güncelleştirmesi daha önce Microsoft Forefront Threat Management Gateway Güvenlik Duvarı İstemcisi olarak adlandırılan Microsoft Forefront Threat Management Gateway (TMG) 2010 İstemcisi'ndeki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik güncelleştirmesi, bir saldırgan TMG güvenlik duvarı istemcisinin kullanıldığı bir sistemde istemci bilgisayar aracılığıyla belirli istemlerde bulunursa uzaktan kod yürütülmesine olanak verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Forefront Threat Management Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217499">MS11-041</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdek Modu Sürücülerindeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2525694)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir OpenType yazı tipi (OTF) içeren bir ağ paylaşımını (veya ağ paylaşımına işaret eden bir web sitesini) ziyaret ederse uzaktan kod yürütülmesine olanak verebilir. Ancak bu durumların hiçbirinde, saldırganın kullanıcıları bu tür bir web sitesini veya ağ paylaşımını ziyaret etmeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıyı bir e-posta iletisindeki veya Instant Messenger iletisindeki bağlantıyı tıklatmaya ikna ederek onu bu web sitesine ya da ağ paylaşımına çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;"><strong>Dağıtılmış Dosya Sistemi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2535512)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Dağıtılmış Dosya Sistemi'ndeki (DFS) özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıklarından daha önemli olanı, bir saldırgan istemci tarafından başlatılan bir DFS isteğine özel hazırlanmış bir DFS yanıtı gönderdiğinde uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan rasgele kod yürütebilir ve etkilenen sistemin tüm denetimini ele geçirebilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ yapılarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. En iyi uygulamalar, Internet'e bağlı sistemlerde olabildiğince az sayıda bağlantı noktasının açılmasını önerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215841">MS11-043</a></td>
<td style="border:1px solid black;"><strong>SMB İstemcisi'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2536276)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan istemci tarafından başlatılan bir SMB isteğine özel hazırlanmış bir SMB yanıtı gönderirse uzaktan kod yürütülmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için, kullanıcıyı özel hazırlanmış bir SMB sunucusuna SMB bağlantısı oluşturmaya ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=216436">MS11-044</a></td>
<td style="border:1px solid black;"><strong>.NET Framework'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2538814)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft .NET Framework'teki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web sayfasını XAML Tarayıcı Uygulamaları (XBAP) çalıştırabilen bir Web tarayıcısı kullanarak görüntülerken istemci sistemde uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Güvenlik açığı, IIS çalıştıran bir sunucu sisteminde, söz konusu sunucu ASP.NET sayfalarının işlenmesine izin veriyorsa ve saldırgan özel hazırlanmış bir ASP.NET sayfasını başarıyla sunucuya yükleyip çalıştırırsa (Web barındırma senaryosunda bu durum geçerli olabilir) uzaktan kod yürütülmesine izin verebilmektedir. Bu güvenlik açığı, Windows .NET uygulamaları tarafından Kod Erişimi Güvenliği (CAS) kısıtlamalarını atlamak için de kullanılabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer Toplu Güvenlik Güncelleştirmesi (2530548)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen on bir güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, yerel kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=218115">MS11-052</a></td>
<td style="border:1px solid black;"><strong>Vektör İşaretleme Dilindeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2544521)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Vektör İşaretleme Dili'nin (VML) Microsoft uygulamasındaki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik güncelleştirmesi Windows istemcileri üzerinde Internet Explorer 6, Internet Explorer 7 ve Internet Explorer 8 için Kritik; Windows sunucuları üzerinde Internet Explorer 6, Internet Explorer 7 ve Internet Explorer 8 için ise Orta olarak derecelendirilmiştir. Internet Explorer 9 bu güvenlik açığından etkilenmez.<br />
<br />
Güvenlik açığı, Internet Explorer kullanan bir kullanıcı özel hazırlanmış bir Web sayfasını görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217912">MS11-037</a></td>
<td style="border:1px solid black;"><strong>MHTML'deki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (2544893)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki MHTML protokolü işleyicisindeki genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir URL'yi saldırganın Web sitesinden açarsa bilginin açığa çıkmasına neden olabilir. Saldırganın kullanıcıyı bir e-posta iletisindeki veya Instant Messenger iletisindeki bağlantıyı tıklatmaya ikna ederek onu bu Web sitesine çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Bilginin Açığa Çıkması</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;"><strong>Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2537146)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen sekiz güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Excel dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, oturum açmış kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Office Dosya Doğrulaması'nı (OFV) yükleyip şüpheli dosyaların açılmasını engelleyecek şekilde yapılandırmak, CVE-2011-1272, CVE-2011-1273 ve CVE-2011-1279'da açıklanan güvenlik açıklarından yararlanmak için kullanılabilecek saldırı vektörlerini engeller. Microsoft Excel 2010 yalnızca bu bültende açıklanan CVE-2011-1273'ten etkilenir. Microsoft Bilgi Bankası makalesi 2501584'te sunulan &quot;Excel 2010'da Korumalı Görünümde Düzenlemeyi Devre Dışı Bırakma&quot; adlı otomatik Microsoft Düzelt çözümü, CVE-2011-1273'te açıklanan güvenlik açıklarından yararlanmak için kullanılabilecek saldırı vektörlerini engeller.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217464">MS11-046</a></td>
<td style="border:1px solid black;"><strong>Yardımcı İşlev Sürücüsündeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2503665)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows Yardımcı İşlev Sürücüsü'ndeki (AFD) genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan kullanıcının sisteminde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217468">MS11-047</a></td>
<td style="border:1px solid black;"><strong>Hyper-V Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2525835)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Server 2008 Hyper-V ve Windows Server 2008 R2 Hyper-V'deki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, Hyper-V sunucusu tarafından barındırılan konuk sanal makinelerden birinde kimliği doğrulanmış bir kullanıcı tarafından VMBus'a özel hazırlanmış bir paket gönderilirse hizmet reddine olanak verebilir. Bir saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve konuk sanal makinesinden özel hazırlanmış içerik gönderebilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215840">MS11-048</a></td>
<td style="border:1px solid black;"><strong>SMB Sunucusu'ndaki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2536275)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan özel hazırlanmış bir SMB paketi oluşturup bu paketi etkilenen bir sisteme gönderirse hizmet reddine olanak verebilir. Güvenlik duvarlarına yönelik en iyi uygulamalar ve standart olarak kullanılan varsayılan güvenlik duvarı yapılandırmaları, bu güvenlik açığından yararlanmak üzere işletme dışından gerçekleştirilen saldırılardan ağların korunmasına yardımcı olabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217077">MS11-049</a></td>
<td style="border:1px solid black;"><strong>Microsoft XML Düzenleyicisi'ndeki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (2543893)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft XML Düzenleyicisi'ndeki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web Hizmeti Bulma (.disco) dosyasını bu bültende listelenen etkilenen yazılımlardan biriyle açarsa bilginin açığa çıkmasına neden olabilir. Bu güvenlik açığının, bir saldırganın doğrudan kod yürütmesine veya kullanıcı haklarını yükseltmesine izin vermeyeceğini unutmayın; ancak, etkilenen sistemden daha fazla yararlanmak amacıyla kullanılacak bilgileri üretmek için kullanılabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Bilginin Açığa Çıkması</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft Visual Studio</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217101">MS11-051</a></td>
<td style="border:1px solid black;"><strong>Active Directory Sertifika Hizmetleri Web Kaydı'ndaki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2518295)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Active Directory Sertifika Hizmetleri Web Kaydı'ndaki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, ayrıcalık yükselmesine izin vererek bir saldırganın sitede hedef kullanıcının bağlamında rasgele komutlar yürütmesine olanak tanıyabilecek siteler arası komut dosyası çalıştırma (XSS) güvenlik açığıdır. Bu güvenlik açığından başarıyla yararlanan bir saldırganın özel hazırlanmış bir bağlantı göndermesi ve kullanıcıyı bu bağlantıyı tıklatmaya ikna etmesi gerekir. Ancak bu durumların hiçbirinde, saldırganın kullanıcıları bu tür bir Web sitesini ziyaret etmeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıyı bir e-posta iletisindeki veya Instant Messenger iletisindeki güvenlik açığından etkilenen Web sitesine götüren bir bağlantıyı tıklatmaya ikna ederek onu bu siteye çekmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, bülten numarasına ve ardından CVE numarasına göre listelenmektedir. Bültenlerde yalnızca önem derecesi Kritik veya Önemli olan güvenlik açıkları yer almaktadır.
  
**Bu tabloyu nasıl kullanabilirim?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde kod yürütme ve hizmet reddi yararlanmalarının olasılığını öğrenmek amacıyla kullanın. Bu ayın güncelleştirmelerini hangi öncelikle dağıtacağınızı belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini inceleyin. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
Aşağıdaki sütunlarda yer alan "En Son Yazılım Sürümü" ve "Yazılımın Eski Sürümleri", bültenin "Etkilenen Yazılımlar" ve "Etkilenmeyen Yazılımlar" tablolarında listelenen ilgili yazılımın sırasıyla en son sürümü ve desteklenmeye devam eden eski sürümleri anlamına gelir.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Güvenlik Açığı Başlığı</th>
<th style="border:1px solid black;" >CVE Kimliği</th>
<th style="border:1px solid black;" >En Son Yazılım Sürümü için Kod Yürütme Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Yazılımın Eski Sürümleri için Kod Yürütme Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Hizmet Reddi Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Önemli Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217912">MS11-037</a></td>
<td style="border:1px solid black;">MHTML'de Mime Olarak Biçimlendirilmiş İstek Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1894">CVE-2011-1894</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur<br />
<br />
Bu bir bilginin açığa çıkması güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212284">MS11-038</a></td>
<td style="border:1px solid black;">OLE Otomasyonu'nda Boşalma Nedeniyle Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0658">CVE-2011-0658</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212287">MS11-039</a></td>
<td style="border:1px solid black;">.NET Framework'te Dizi Kaydırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0664">CVE-2011-0664</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217470">MS11-040</a></td>
<td style="border:1px solid black;">TMG Güvenlik Duvarı İstemcisi'nde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1889">CVE-2011-1889</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217499">MS11-041</a></td>
<td style="border:1px solid black;">Win32k'de OTF Doğrulama Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1873">CVE-2011-1873</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;">DFS'de Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1868">CVE-2011-1868</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;">DFS Başvurusu Yanıtında Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1869">CVE-2011-1869</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu bir hizmet reddi güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215841">MS11-043</a></td>
<td style="border:1px solid black;">SMB'de Yanıt Ayrıştırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1268">CVE-2011-1268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=216436">MS11-044</a></td>
<td style="border:1px solid black;">.NET Framework'te JIT İyileştirmesi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1271">CVE-2011-1271</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Kaydın Yeterince Doğrulanmaması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1272">CVE-2011-1272</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Hatalı Kayıt Ayrıştırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1273">CVE-2011-1273</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Sınırların Dışında Dizi Erişimi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1274">CVE-2011-1274</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Bellek Öbeğinin Üzerine Yazma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1275">CVE-2011-1275</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Arabellek Taşması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1276">CVE-2011-1276</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1277">CVE-2011-1277</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de WriteAV Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1278">CVE-2011-1278</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Excel'de Sınırların Dışında WriteAV Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1279">CVE-2011-1279</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217464">MS11-046</a></td>
<td style="border:1px solid black;">Yardımcı İşlev Sürücüsünde Ayrıcalık Yükselmesi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1249">CVE-2011-1249</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur<br />
<br />
Bu bir ayrıcalık yükseltmesi güvenlik açığıdır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217468">MS11-047</a></td>
<td style="border:1px solid black;">VMBus Kalıcı DoS Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1872">CVE-2011-1872</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">Bu bir hizmet reddi güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215840">MS11-048</a></td>
<td style="border:1px solid black;">SMB İsteğini Ayrıştırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1267">CVE-2011-1267</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu bir hizmet reddi güvenlik açığıdır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217077">MS11-049</a></td>
<td style="border:1px solid black;">XML Dış Varlıklarını Çözümleme Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1280">CVE-2011-1280</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Bu bir bilginin açığa çıkması güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Bağlantı Özelliklerini İşlemede Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1250">CVE-2011-1250</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">DOM İşlemede Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1251">CVE-2011-1251</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">toStaticHTML API'sinde Bilginin Açığa Çıkması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1252">CVE-2011-1252</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> – İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Bu bir bilginin açığa çıkması güvenlik açığıdır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sürükle ve Bırak Özelliğinde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1254">CVE-2011-1254</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Saat Öğesinde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1255">CVE-2011-1255</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">DOM Değiştirmede Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1256">CVE-2011-1256</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Düzende Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1260">CVE-2011-1260</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Seçim Nesnesinde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1261">CVE-2011-1261</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">HTTP Yeniden Yönlendirmede Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1262">CVE-2011-1262</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> – Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217101">MS11-051</a></td>
<td style="border:1px solid black;">Active Directory Sertifika Hizmetleri Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1264">CVE-2011-1264</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Bu bir ayrıcalık yükseltmesi güvenlik açığıdır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=218115">MS11-052</a></td>
<td style="border:1px solid black;">VML'de Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1266">CVE-2011-1266</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
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
  
**Tablo 1**

 
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
</tr>
<tr>
<th colspan="8">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2371079f-fb20-4fd5-999e-e73f3701818c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=67a25abd-f43c-4b01-b507-a109b739238f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=492310d3-bbb4-4fff-b5fe-3470c17e7681)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=26ec66af-9727-4423-90da-012ed5b30856)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4203a59a-a809-45db-a234-fef0ff5063f9)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4a49ec89-2a8f-41d9-8f0b-ee57fdf21f50)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b53d6631-4ded-48f5-a503-925b89b322b2)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=035d5115-54b6-41d3-b9f0-890041ead178)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=af6b7627-c462-45fe-8948-70da37e60659)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e10a4c3c-2ef8-4cfc-ac9b-4d97bfa79ac1)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f6e05fef-ee8c-44ff-a106-d7b8659c8d91)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9fc734db-a177-43d2-a74a-b1fe6ea6f779)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4e4e18a4-97dc-4c5e-a078-8466913aa29e)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e6ff410-4552-4687-81ab-83d9c91f8af5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3aa8f1bc-07de-451a-8244-1733247e6f2e)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2719e0fb-3cfd-47b2-906d-3e07b0e3c978)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=638f6dd6-bea0-4356-b23a-45e865a6b28b)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a3bd0012-4a45-4f96-8a51-3ff1f85d1e37)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=19557984-5088-44cc-b5ba-9bab33df8e7e)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9c1a539f-1472-4394-8354-bd549d8332e0)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4aa8c003-0353-4a5b-8aea-c01a103af393)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9018258-5a72-47a1-8584-3d1aa52317c3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c962531e-f580-4195-989b-cf348cc96fa7)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ce616970-343d-49f1-994d-4269b9a11448)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=70ece3b4-e5bb-469c-bfef-c8310681f5a7)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c92d94c5-5e8f-45aa-a24a-f4d0efd93732)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=c194dd35-b9db-44a5-a252-38f9f803802f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=2e07b5fa-c9fa-495b-9352-c07ce46a7e8b)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=96309c49-4822-4c47-b364-2ba65327cac5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ea18a916-03cf-4eac-bacc-ceb006491f24)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritik)  
[Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f58ebc9e-00e1-413c-8076-d7a44003d0c7)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=80231a27-b37c-4101-a34f-19a26a040836)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f33c9e54-c2e5-498d-a798-5bbfe9e4249c)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1 ve Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritik)  
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritik)  
Yalnızca Windows Vista Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritik)  
Windows Vista Service Pack 1 ve Windows Vista Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=aded8f20-479d-40c1-9560-c0581c6f77a2)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a62edfd8-9016-4bb5-bf48-885498fa0042)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritik)  
Yalnızca Windows Vista Service Pack 1: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritik)  
Yalnızca Windows Vista Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritik)  
Windows Vista Service Pack 1 ve Windows Vista Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=fea735a8-032b-4fa6-8337-1fa411df0b88)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4cddfc68-eff6-4587-8607-63307d039489)  
(Kritik)  
Yalnızca Windows Vista Service Pack 2: [Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=392316fc-f531-469c-aa60-4ecf061a5354)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4566528f-62ee-4d78-b3af-131a7cc15e1f)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1 ve Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritik)  
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritik)  
Yalnızca Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritik)  
Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a519a5d7-bfe3-4e53-99e9-d85f7e34237f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=962cb40c-680c-4c37-98d4-ca9789ca7270)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb561ba6-af4d-40cc-947c-923f9cca9a7e)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritik)  
Yalnızca Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritik)  
Yalnızca Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritik)  
Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=49dcb47b-3c79-4f69-ba07-f471304c16e2)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e0a8fbac-2c31-4cf8-9967-6171edabd560)  
(Kritik)  
Yalnızca Windows Vista x64 Edition Service Pack 2: [Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=44b2aa73-c318-47ac-ad87-0d24afd9cdd7)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c9614d9-6f61-463d-b1fa-bd5eb2c1a5c5)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1 ve Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)\*\*  
(KB2478657)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)\*\*  
(KB2478659)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)\*\*  
(KB2478660)  
(Kritik)  
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*\*<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8ebfa067-0236-4454-8605-df1b99742f90)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8ab9679e-6a69-4ca3-9210-7ca4fb1980c2)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritik)  
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*\*<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b6547ff0-b059-495d-8816-bb094ac11be7)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c9650c47-ac52-433d-b409-ce1cfe8d3e87)\*\*  
(Kritik)  
Yalnızca 32-bit sistemler için Windows Server 2008 Service Pack 2: [Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7f9b1ba2-8247-494b-990c-f62003188c5a)\*\*  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36698775-0e4e-4980-ae4c-43542de424ca)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1 ve Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)\*\*  
(KB2478657)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)\*\*  
(KB2478659)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)\*\*  
(KB2478660)  
(Kritik)  
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*\*<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd8f3713-b408-4db6-aecd-7eed2176a715)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f1d76b82-9996-4d08-894b-9c16a4b3bb1e)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22c63fc3-2c5a-4e50-9026-2e04a6e74210)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritik)  
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*\*<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=feff3364-4bfd-45f5-99da-9192b47ef5d4)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=7dff9f08-19cb-41dd-a315-84c1dac81510)\*\*  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 Service Pack 2: [Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=fdf88a52-c099-44eb-95a0-650129c0e678)\*\*  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3edb613f-5bf0-4e28-9835-4afbb6ef0e01)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1 ve Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 ve Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritik)  
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a61f888-c81e-4b8a-8932-2fe67df4b2ad)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f80c89c6-27ab-4f6a-afad-9c8e92cbbce4)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5bb889de-8ff6-4587-8ef9-ffb13e8d60fd)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Önem derecesi yok<sup>[2]</sup>)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5](http://www.microsoft.com/downloads/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritik)  
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d81a9219-da95-4fbf-af7f-898f553b0572)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="8">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=50ae36ff-2406-48a4-97cc-12782b6d30ac)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca 32-bit sistemler için Windows 7: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritik)  
32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=9de1bf5d-6f25-496d-bc44-a32c5e8920fe)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=19a15098-1754-4536-a9ca-ff07d16464b7)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca 32-bit sistemler için Windows 7: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritik)  
Yalnızca 32-bit sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritik)  
32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=91b98f02-a09e-48f1-9f78-a949f7268542)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=79f846da-3b17-43c9-9016-a055c2c56975)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1241f0f8-a5c7-420a-a5b7-b6c3caa9e5e2)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows 7: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritik)  
x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için 7 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e7f52b13-5b3d-438c-ae14-86da50c8b67a)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=50d1c677-57aa-4e3f-bdfc-6f01b5d3bfe2)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b449f23e-b3df-46e5-bfe3-98268d20ad54)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows 7: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows 7 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritik)  
x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için 7 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=264107cc-68b4-401c-82f7-de64b535c18d)  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=e87a09f2-b755-48ef-9b85-fc78d0bfce43)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8181c359-cd79-438a-87be-093b363d0b04)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)\*  
(KB2478661)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)\*  
(KB2478662)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b77e5be6-d3eb-4e3a-9be2-831578f0447c)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9d66b1e7-dbf9-4475-a973-49fb85557eca)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=06008192-3cac-477b-a913-83eed39d8718)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)\*  
(KB2518867)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)\*  
(KB2518869)  
(Kritik)  
Yalnızca x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=8b18e6f9-96b8-4dec-bcd0-d71f1bac3eb0)\*\*  
(Kritik)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=81814b15-ebdf-4817-932b-5ea7a37fa6ed)\*\*  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6b63a1eb-445a-4cd3-b357-9a1dd82d7a35)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritik)  
Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c00a33bc-c874-4693-b0f7-5034c5df9424)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=3c8455f1-b8a0-4ba2-84a2-043d25ef75c5)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=93a32bd9-7e67-4ace-8c45-116f91b032f9)  
(Kritik)
</td>
<td style="border:1px solid black;">
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 R2: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritik)  
Yalnızca Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritik)  
Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1: [Microsoft .NET Framework 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ab2406a8-06f7-4f88-9af4-dc136d64bc35)  
(Kritik)
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Notlar**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS11-039 için Notlar**

<sup>[1]</sup>**.NET Framework 4.0 ve .NET Framework 4.0 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4.0 ve .NET Framework 4.0 İstemci Profili. .NET Framework 4.0 İstemci Profili, .NET Framework 4.0'ın bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4.0'ı hem de .NET Framework 4.0 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

**MS11-044 için Notlar**

<sup>[1]</sup>**.NET Framework 4.0 ve .NET Framework 4.0 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4.0 ve .NET Framework 4.0 İstemci Profili. .NET Framework 4.0 İstemci Profili, .NET Framework 4.0'ın bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4.0'ı hem de .NET Framework 4.0 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

<sup>[2]</sup>Bu bültende açıklanan güvenlik açığı bu yazılımı etkilemediği için önem dereceleri bu güncelleştirmeye uygulanmamıştır. Ancak Microsoft gelecekte tanımlanabilecek olası saldırı sektörlerine karşı kapsamlı bir savunma önlemi olarak, bu yazılımı kullanan müşterilerin bu güvenlik güncelleştirmesini uygulamalarını önerir.

**Tablo 2**

 
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
</tr>
<tr>
<th colspan="7">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6c760c7f-94f1-437f-a645-fd33b50d03f4)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0b88f9e9-3439-44e5-92c8-66a3c97cb03d)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=03b45ad8-cc6b-473b-8112-bd513ed97f5d)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ce5bc2d7-9438-4bf0-be5e-be9dd00c3286)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a1db7736-f3e4-45df-af1d-52746978a0a8)  
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=c94c0d17-fdbe-41b3-a23d-98f43f907b89)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ff955dc3-58ca-40ea-b7f1-9ff40c37f997)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ed502ece-737e-44cb-84fd-8a0d1bc321c8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b211b02-a005-46a3-ad1d-d4baaeec8289)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71497891-41a2-476d-b524-4eb5cecb9639)  
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
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Düşük**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5dafb455-969e-4be9-8735-d4ee0682d22f)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ba3beb80-a921-489e-a6ff-a7b2d665ada6)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a8038325-0d14-445b-a5d9-ce7ac1fa44b5)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6427ea5d-05d0-4367-805c-9cb305802b3c)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c614cb8b-223e-4f84-b94c-f15747760aa5)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ef90d6c1-ea7f-4c32-9c90-0303e04c7436)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=e78829d0-8215-4e56-8959-ebd3bc8e9a91)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3bec943e-5758-4439-a947-a8fafd30edec)  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5f7bcbad-f647-4fbb-88d4-b19c54db6f00)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e7f65891-32c0-4817-b3b2-d8be73145df9)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a951087-25c5-4f5c-8407-a1585491ae0b)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62944095-33d6-4131-be32-a79d9ec4d4a9)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1e822515-9f0a-4ef0-bb70-d4889d200f47)  
(Orta)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=47a0fdc6-7576-4c32-b8fd-cbb05d57599d)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ca8b1d09-9f80-417b-99b1-8f86e86e1f11)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=dd48b93b-24fa-45a3-91fb-9f9f9418c49f)  
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
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e541f1bb-c9bf-4dc8-96ec-58a3de5ba7fd)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=cd059690-52b0-4b37-9fbb-d9906ae46fed)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ebea38a7-1fbe-4141-a529-52d7a7326d6a)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b69e3bda-940b-4524-a724-0af4ae0ec719)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5f0007c3-8d11-4940-8766-1112e3777aae)  
(Önemli)
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6c7d7162-ef19-49f4-a8fc-5db7415445a4)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=256bb26f-df9e-4259-881b-e8313a9fafa8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=54833350-a385-4a31-995a-9ddc38798c21)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e3a26bc5-1757-4b38-9cae-419c919f4877)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fadf6f12-1f09-4d49-93b1-8fce01400b4f)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Düşük**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4446121a-0aab-4fbc-ba74-68d7650e8bca)\*\*  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ed089de4-c9ec-4ac7-a711-5f7cb29c05bc)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6a3bbd67-94db-40b2-8786-cb39a493ec92)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e34e4cf9-cdae-4240-8574-950c0be00822)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8960dd62-7cf7-41cb-97b2-b082bd1750aa)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46ade106-e0cb-4c71-8230-793a15062823)\*\*  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=01399fc7-dc2b-461e-a1a5-751a3b61bde0)\*\*  
(Orta)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=dd32b7c6-daa1-47aa-807f-25a678790cf2)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4cb870f3-9878-4075-b8fd-2ee90c8e3bc8)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a3604f05-26b2-451b-9153-0e718158371e)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=24789423-72b7-48d1-bdc1-f0e5174d99bb)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0abc6908-ac6a-4da3-843a-af6841ccc1db)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6141a1c5-ecaf-4553-9d27-dd6e5c4a13fd)\*\*  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=16a8b78a-3979-4cc7-bbe5-6d962aa64336)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e1243011-00e6-49f2-a676-c04cb805d36a)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8a82b44-e1d8-45f8-b8b8-b1f74e1efce0)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=057f1356-9c70-4457-a1df-69334fdab467)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="7">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=27e767d8-84e3-434f-bb8d-3b2303774ad0)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c3647646-658a-423b-b0cb-bba7613b67e7)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=63d8b801-5178-474b-a21e-72a0ce501d3e)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 ve 32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cf9e5ecd-68f7-4982-b4ed-be80859b757c)  
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
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=747ba56a-0d47-4946-99a4-bae1f11ea748)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7996511d-4b8e-49c3-a0fa-4da907a6c947)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cd7d3cb9-cb60-4b62-b0df-a38fe21802e9)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 ve x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2707650a-604c-4044-acc4-07a30b5640d8)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Düşük**](http://go.microsoft.com/fwlink/?linkid=21140)
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
x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=cff7f53d-0fd6-48f8-a9d6-bf19e0a32905)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=40354f73-4f4d-4a4a-abac-f8a3d4c3ae5f)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e67c73ca-d0f9-40c1-8b6e-25b1b13caa3a)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c9c6c36d-a455-42f7-b7d4-9fb9824c07cb)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f9824310-772d-4e1e-980e-11e2db3ac53e)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 ve x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1da04414-6210-43ea-8e0a-cf21cf144076)\*\*  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4dd2c0f4-b29c-4648-a123-83d3ae6a878f)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=22853823-8f63-4258-8991-1ad50e58a0d9)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72d1d6b6-e8bd-492b-b65a-82060beef441)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0533d293-e186-4d39-a925-ab3d9ed46290)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Not**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
Microsoft Office Paketleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=853c0663-94f7-4634-98ad-47ca4b1f7b1e)  
(KB2541003)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f38f183a-9c64-406b-9bf6-807cb2d55e56)  
(KB2541025)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b271f87-a279-419f-9437-ded224fa19f1)<sup>[1]</sup>
(KB2541007)  
(Önemli)
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
[Microsoft Excel 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=baba7ec1-4a5e-4e13-9d0e-9085a39a0554)  
(KB2523021)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=d6e9f422-43b0-4da5-8356-c38482e8eebb)  
(KB2523021)  
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
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=d12d0868-4f28-4c0a-ab61-338878064b70)  
(KB2555786)  
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
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=9e2d348b-c753-4eab-838c-370cd5af5e14)  
(KB2555785)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2011
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2011](http://www.microsoft.com/downloads/details.aspx?familyid=3c58555c-1eba-42fe-a10f-b30af9031e44)  
(KB2555784)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Açık XML Dosya Biçimi Dönüştürücüsü
</td>
<td style="border:1px solid black;">
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=6118d5f5-b6fd-4584-be25-209534772379)  
(KB2555787)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Microsoft InfoPath
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft InfoPath 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=88eedb0b-a2cf-4a1b-b1b9-0b2926c25872)  
(KB2510061)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft InfoPath 2010 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=90ffe910-bd9c-48aa-8007-2b43e1a99999)  
(KB2510065)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft InfoPath 2010 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f3244003-fb63-44d8-bedc-6399c39aacba)  
(KB2510065)  
(Önemli)
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
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=77c1e7e2-207f-46fd-81f2-43a25eddc010)  
(KB2541015)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3512a033-871d-49ec-a8d2-1b9c7dec4936)  
(KB2541012)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**MS11-045 için Not**

<sup>[1]</sup>Microsoft Office Excel 2007 Service Pack 2 için, müşterilerin bu bültende açıklanan güvenlik açıklarına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB2541007'nin yanı sıra, Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2 (KB2541012) güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

**MS11-049 için Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Server Yazılımı

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
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
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Önemli)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 4
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Önemli)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Express Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Express Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Express Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Express Edition Service Pack 4
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Express Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Express Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Express Edition with Advanced Services Service Pack 3
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Express Edition with Advanced Services Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Express Edition with Advanced Services Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Express Edition with Advanced Services Service Pack 4
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Express Edition with Advanced Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Önemli)  
QFE güncelleştirmesi:  
[SQL Server 2005 Express Edition with Advanced Services Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server Management Studio Express (SSMSE) 2005
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server Management Studio Express (SSMSE) 2005](http://www.microsoft.com/downloads/details.aspx?familyid=34c3ba21-b158-4e6d-82ba-831053d41161)  
(KB2546869)  
(Önemli)  
QFE güncelleştirmesi:  
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server Management Studio Express (SSMSE) 2005 x64 Edition
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server Management Studio Express (SSMSE) 2005 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=34c3ba21-b158-4e6d-82ba-831053d41161)  
(KB2546869)  
(Önemli)  
QFE güncelleştirmesi:  
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için SQL Server 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)<sup>[1]</sup>
(KB2494096)  
(Önemli)  
QFE güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)<sup>[1]</sup>
(KB2494100)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için SQL Server 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)<sup>[1]</sup>
(KB2494096)  
(Önemli)  
QFE güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)<sup>[1]</sup>
(KB2494100)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)  
(KB2494096)  
(Önemli)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)  
(KB2494100)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)<sup>[1]</sup>
(KB2494089)  
(Önemli)  
QFE güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)<sup>[1]</sup>
(KB2494094)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)<sup>[1]</sup>
(KB2494089)  
(Önemli)  
QFE güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)<sup>[1]</sup>
(KB2494094)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)  
(KB2494089)  
(Önemli)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)  
(KB2494094)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)<sup>[1]</sup>
(KB2494088)  
(Önemli)  
QFE güncelleştirmesi:  
[32-bit sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)<sup>[1]</sup>
(KB2494086)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)<sup>[1]</sup>
(KB2494088)  
(Önemli)  
QFE güncelleştirmesi:  
[x64 tabanlı sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)<sup>[1]</sup>
(KB2494086)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2008 R2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)  
(KB2494088)  
(Önemli)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)  
(KB2494086)  
(Önemli)
</td>
</tr>
</table>
 
**MS11-049** **için** **Notlar**

<sup>[1]</sup>Bu güncelleştirme, karşılık gelen Express ve Express with Advanced Services Edition sürümlerine de uygulanır.

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Geliştirici Araçları ve Yazılımları

 
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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
Mac üzerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8)  
(KB2512827)  
(Kritik)  
Tüm Microsoft Windows istemci sürümlerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8)  
(KB2512827)  
(Kritik)  
Tüm Microsoft Windows sunucu sürümleri üzerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8)\*\*  
(KB2512827)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Visual Studio
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e5ce8a9a-e89b-4095-9f21-7e6f307fbf2b)  
(KB2251481)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cc01bce9-3f38-4590-9c6e-a4048c886d33)  
(KB2251487)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](http://www.microsoft.com/downloads/details.aspx?familyid=213b820f-dcba-4895-b339-b50eeb92524d)  
(KB2251489)  
(Önemli)
</td>
</tr>
</table>
 
**MS11-039 için Notlar**

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

**MS11-049 için Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Güvenlik Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Forefront
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS11-040**](http://go.microsoft.com/fwlink/?linkid=217470)
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
Microsoft Forefront Threat Management Gateway 2010 İstemcisi
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Threat Management Gateway 2010 İstemcisi](http://www.microsoft.com/downloads/details.aspx?familyid=d1c85acd-a6df-4634-9cd4-c562ad92097e)  
(Kritik)
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

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Microsoft Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Güncelleştirmeler

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): Yazılım Güncelleştirme Hizmetleri ve Windows Server Güncelleştirme Hizmetleri'nin tanımı içeriğe bağlı olarak değişir. Tüm Windows içeriğini içerir.
-   [Windows Server Update Services için Geçmiş Aylardaki Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Microsoft Windows dışındaki Microsoft ürünleri için yeni, yeniden düzenlenen ve yeniden yayımlanan tüm güncelleştirmeleri görüntüler.

#### Microsoft Etkin Koruma Programı (MAPP)

Microsoft müşterilerinin güvenlik korumalarını artırmak için, güvenlik açığı bilgilerini aylık güvenlik güncelleştirmesi yayın döngüsünden daha önce başlıca güvenlik yazılımı sağlayıcılarına sunmaktadır. Güvenlik yazılımı sağlayıcıları böylece bu güvenlik açığı bilgilerini kullanarak müşterilere virüsten koruma, ağ tabanlı davetsiz giriş algılama sistemleri veya ana bilgisayar tabanlı davetsiz giriş algılama sistemleri gibi güvenlik yazılımları ya da aygıtları aracılığıyla güncelleştirilmiş koruma sağlayabilirler. Güvenlik yazılımı sağlayıcıları tarafından hazırlanmış etkin korumaların bulunup bulunmadığını belirlemek üzere, [Microsoft Etkin Koruma Programı (MAPP) Ortakları](http://go.microsoft.com/fwlink/?linkid=215201) altında listelenen program ortaklarınca sağlanan etkin koruma web sitelerini ziyaret edin.

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

-   [Google Security Team](http://www.google.com/) için çalışan Billy Rios ve Eduardo Vela Nava, MS11-037'deki değişiklikler üzerinde bizimle birlikte çalıştıkları için.
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, MS11-038'de açıklanan sorunu bildirdiği için
-   Michael J. Liu, MS11-039'da açıklanan sorunu bildirdiği için
-   [www.korosoft.net](http://www.korosoft.net/) sitesinden Koro, MS11-041'de açıklanan sorunu bildirdiği için
-   [NGS Software](http://www.ngssoftware.com/) için çalışan Laurent Gaffié, MS11-042'de açıklanan sorunu bildirdiği için
-   Dan Kaminsky, MS11-044'te açıklanan sorun konusunda bizimle çalıştığı için
-   [Fortinet bünyesindeki FortiGuard Labs](http://www.fortiguard.com/) için çalışan Bing Liu, MS11-045'de açıklanan sorunu bildirdiği için
-   Anonim bir araştırmacı, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-045'de açıklanan sorunu bildirdikleri için
-   Omair, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-045'te açıklanan sorunu bildirdikleri için
-   Anonim bir araştırmacı, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-045'de açıklanan sorunu bildirdikleri için
-   [Agarri](http://www.agarri.fr/) için çalışan Nicolas Gregoirei [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-045'te açıklanan sorunu bildirdikleri için
-   Omair, MS11-045'te açıklanan sorunu bildirdiği için
-   [CERT/CC](http://www.cert.org/) için çalışan Will Dormann, MS11-045'te açıklanan iki sorunu bildirdiği için
-   [Shadowserver Foundation](http://www.shadowserver.org) için çalışan Steven Adair ve Chris S. MS11-046'da açıklanan sorunu bildirdikleri için
-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Nicolas Economou, MS11-047'de açıklanan sorunu bildirdiği için
-   [Cigital](http://www.cigital.com) için çalışan Jesse Ou, MS11-049'da açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan Robert Swiecki, MS11-050'de açıklanan sorunu bildirdiği için
-   [NSFOCUS Security Team](http://www.nsfocus.com/), MS11-050'de açıklanan sorunu bildirdikleri için
-   Anonim bir araştırmacı, [Beyond Security bünyesindeki SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html) programı ile birlikte çalışarak MS11-050'de açıklanan sorunu bildirdikleri için
-   [IBM Rational Application Security](http://blog.watchfire.com/) için çalışan Adi Cohen, MS11-050'de açıklanan sorunu bildirdiği için
-   [Trend Micro](http://www.trendmicro.com/), MS11-050'te açıklanan sorun konusunda bizimle çalıştıkları için
-   [Norman](http://www.norman.com) için çalışan Nirmal Singh Bhary, MS11-050'de açıklanan sorunu bildirdiği için
-   Anonim bir araştırmacı, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS11-050'de açıklanan sorunu bildirdikleri için
-   Damian Put, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS11-050'de açıklanan sorunu bildirdikleri için
-   [salesforce.com](http://www.salesforce.com/) sitesinin Ürün Güvenliği ekibinden Yoel Gluck, Yogesh Badwe ve Varun Badhwar, MS11-050'de açıklanan sorunu bildirdikleri için
-   Jose Antonio Vazquez Gonzalez, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS11-050'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS11-050'te açıklanan sorunu bildirdiği için
-   Peter Winter-Smith, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS11-050'de açıklanan sorunu bildirdikleri için
-   [Harmony Security](http://www.harmonysecurity.com/) için çalışan Stephen Fewer, [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte MS11-050'de açıklanan kapsamlı savunma değişiklikleri üzerinde bizimle çalıştıkları için
-   Ruggero Strabla, [Emaze](http://www.emaze.net/)Networks; [Saipem Security Team](http://www.saipem.com/), MS11-051'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS11-052'te açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (14 Haziran 2011): Bülten Özeti yayımlandı.
-   V1.1 (14 Haziran 2011): MS11-042'deki **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** alt bölümünde yer alan 32-bit sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows 7 Service Pack 1, x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 ve Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1 kaldırıldı. Bu yalnızca bilgilendirme amaçlı bir değişikliktir. Güvenlik güncelleştirmesi dosyalarında veya algılama mantığında herhangi bir değişiklik yapılmamıştır.
-   V2.0 (9 Ağustos 2011): Bir kararlılık sorununu gidermek üzere MS11-043'teki güncelleştirmeyi tüm desteklenen işletim sistemlerine yeniden sunmak üzere bülten yeniden yayımlandı. Sistemlerini daha önce başarıyla güncelleştirmiş olan müşteriler MS11-043'ü yeniden yüklemelidir. İlgili yazılımlara yönelik algılama eklemek üzere Microsoft Visual Studio 2005 Service Pack 1 güncelleştirmesindeki bir algılama değişikliğini duyurmak için MS11-049 da yeniden yayımlanmıştır. MS11-049'daki güvenlik güncelleştirmesi dosyalarında hiçbir değişiklik yapılmamıştır. Sistemlerini daha önce başarıyla güncelleştirmiş olan müşterilerin MS11-049'u yeniden yüklemeleri gerekmez.
-   V2.1 (26 Ekim 2011): MS11-039 ve MS11-044 için, x64 tabanlı sistemler için Windows Server 2008 R2 üzerinde .NET Framework 4 için Doğrulanmış Sunucu Çekirdeği yüklemesi.
-   V3.0 (8 Kasım 2011): Windows XP ve Windows Server 2003'ün tüm desteklenen sürümlerine yönelik güncelleştirmeyi yeniden sunmak üzere MS11-037 tekrar yayımlandı. 14 Haziran 2011 tarihinde özgün olarak sunulan güncelleştirmeyi yüklemiş olanlar da dahil olmak üzere Windows XP veya Windows Server 2003 kullanan müşterilerin yeniden sunulan güncelleştirmeyi yüklemeleri gerekmektedir.
-   V3.1 (18 Ocak 2012): MS11-049 için, bu güncelleştirmenin 32-bit ve x64 tabanlı SQL Server 2008, SQL Server 2008 R2 Express ve Express Advanced Edition sürümlerine de uygulandığını açıklığa kavuşturmak üzere Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümüne bir not eklendi.

*Built at 2014-04-18T01:50:00Z-07:00*
