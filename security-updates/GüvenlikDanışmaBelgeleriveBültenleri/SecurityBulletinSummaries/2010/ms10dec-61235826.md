---
TOCTitle: 'MS10-DEC'
Title: Microsoft Güvenlik Bülteni Aralık 2010 Özeti
ms:assetid: 'ms10-dec'
ms:contentKeyID: 61235826
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms10-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Aralık 2010 Özeti
============================================

Yayım Tarihi: 14 Aralık 2010 Salı | Güncelleştirme Tarihi: 15 Aralık 2010 Çarşamba

**Sürüm:** 1.1

Bu bülten özetinde Aralık 2010'da yayımlanan güvenlik bültenleri listelenir.

Aralık 2010 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 9 Aralık 2010'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 15 Aralık 2010 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Aralık Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032454444&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206495">MS10-090</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer Toplu Güvenlik Güncelleştirmesi (2416400)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen dört ve genel olarak duyurulan üç güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=203895">MS10-091</a></td>
<td style="border:1px solid black;"><strong>OpenType Yazı Tipi (OTF) Sürücüsündeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2296199)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Windows OpenType Yazı Tipi (OTF) sürücüsündeki uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen birkaç güvenlik açığını giderir. Saldırgan, bir ağ paylaşımında özel hazırlanmış bir OpenType yazı tipi barındırabilir. Kullanıcı daha sonra bu paylaşıma Windows Gezgini'nde gittiğinde, etkilenen denetim yolu tetiklenir ve özel hazırlanmış yazı tipi etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=203463">MS10-092</a></td>
<td style="border:1px solid black;"><strong>Görev Zamanlayıcısı'ndaki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2305420)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Görev Zamanlayıcısı'ndaki genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan etkilenen sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206698">MS10-093</a></td>
<td style="border:1px solid black;"><strong>Windows Movie Maker'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2424434)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Movie Maker'daki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan kullanıcıyı özel hazırlanmış kitaplık dosyası ile aynı ağ dizininde bulunan meşru bir Windows Movie Maker dosyasını açmaya ikna ederse uzaktan kod yürütülmesine izin verebilir. Saldırının başarılı olması için, kullanıcının güvenilir olmayan bir uzak dosya sistemi konumunu veya WebDAV paylaşımını ziyaret etmesi ve güvenlik açığından etkilenen bir uygulama kullanarak bu konumdan bir belge açması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206699">MS10-094</a></td>
<td style="border:1px solid black;"><strong>Windows Media Kodlayıcısı'ndaki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2447961)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Media Kodlayıcısı'ndaki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan kullanıcıyı özel hazırlanmış kitaplık dosyası ile aynı ağ dizininde bulunan meşru bir Windows Media Profili (.prx) dosyasını açmaya ikna ederse uzaktan kod yürütülmesine izin verebilir. Saldırının başarılı olması için, kullanıcının güvenilir olmayan bir uzak dosya sistemi konumunu veya WebDAV paylaşımını ziyaret etmesi ve güvenlik açığından etkilenen bir uygulama kullanarak bu konumdan bir belge açması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206683">MS10-095</a></td>
<td style="border:1px solid black;"><strong>Microsoft Windows'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2385678)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir kitaplık dosyasıyla aynı ağ klasöründe bulunan .eml ve .rss (Windows Live Mail) ya da .wpost (Microsoft Live Yazar) gibi bir dosya türünü açarsa uzaktan kod yürütülmesine izin verebilir. Saldırının başarılı olması için, kullanıcının güvenilir olmayan bir uzak dosya sistemi konumunu veya WebDAV paylaşımını ziyaret etmesi ve güvenlik açığından etkilenen bir uygulama kullanarak bu konumdan bir belge açması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206738">MS10-096</a></td>
<td style="border:1px solid black;"><strong>Windows Adres Defteri'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2423089)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Adres Defteri'ndeki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir kitaplık dosyası ile aynı ağ klasöründe bulunan bir Windows Adres Defteri dosyasını açarsa uzaktan kod yürütülmesine olanak verebilir. Saldırının başarılı olması için, kullanıcının güvenilir olmayan bir uzak dosya sistemi konumunu veya WebDAV paylaşımını ziyaret etmesi ve güvenlik açığından etkilenen bir uygulama kullanarak bu konumdan bir belge açması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206689">MS10-097</a></td>
<td style="border:1px solid black;"><strong>Internet Bağlantısı Oturum Açma Sihirbazı'nda Güvenli Olmayan Şekilde Kitaplık Yükleme Uzaktan Kod Yürütülmesine İzin Verebilir (2443105)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki Internet Bağlantısı Oturum Açma Sihirbazı'nda genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik güncelleştirmesi Windows XP ve Windows Server 2003'ün tüm desteklenen sürümleri için Önemli olarak derecelendirilmiştir. Windows Vista, Windows Server 2008, Windows 7 ve Windows Server 2008 R2'nin tüm desteklenen sürümleri bu güvenlik açığından etkilenmez.<br />
<br />
Güvenlik açığı, bir kullanıcı özel hazırlanmış bir kitaplık dosyası ile aynı ağ klasöründe bulunan bir .ins veya .isp dosyasını açarsa uzaktan kod yürütülmesine olanak verebilir. Saldırının başarılı olması için, kullanıcının güvenilir olmayan bir uzak dosya sistemi konumunu veya WebDAV paylaşımını ziyaret etmesi ve güvenlik açığından etkilenen bir uygulama kullanarak bu konumdan bir belge açması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204869">MS10-098</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdek Modu Sürücülerindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (2436673)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki genel olarak duyurulan bir ve özel olarak bildirilen birkaç güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan yerel olarak oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açıklarından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206365">MS10-099</a></td>
<td style="border:1px solid black;"><strong>Yönlendirme ve Uzaktan Erişim'deki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2440591)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'un Yönlendirme ve Uzaktan Erişim NDProxy bileşenindeki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik güncelleştirmesi Windows XP ve Windows Server 2003'ün tüm desteklenen sürümleri için Önemli olarak derecelendirilmiştir. Windows Vista, Windows Server 2008, Windows 7 ve Windows Server 2008 R2'nin tüm desteklenen sürümleri bu güvenlik açığından etkilenmez.<br />
<br />
Bu güvenlik açığı, bir saldırgan etkilenen sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204906">MS10-100</a></td>
<td style="border:1px solid black;"><strong>İzin Alma Kullanıcı Arabirimi'ndeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2442962)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, İzin Alma Kullanıcı Arabirimi'ndeki (UI) özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan etkilenen bir sistemde özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine ve SeImpersonatePrivilege iznine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=201319">MS10-101</a></td>
<td style="border:1px solid black;"><strong>Windows Netlogon Hizmeti'ndeki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2207559)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, etki alanı denetleyicisi olarak hizmet vermek üzere yapılandırılmış olan etkilenen Windows Server sürümlerindeki Netlogon RPC Hizmeti'nde özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan etkilenen bir sistemdeki Netlogon RPC Hizmeti arabirimine özel hazırlanmış bir RPC paketi gönderirse hizmet reddine olanak verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için, etkilenen etki alanı denetleyicisi ile aynı etki alanına katılmış bir makinede yönetici ayrıcalıklarına sahip olması gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=205309">MS10-102</a></td>
<td style="border:1px solid black;"><strong>Hyper-V Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2345316)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Server 2008 Hyper-V ve Windows Server 2008 R2 Hyper-V'deki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, Hyper-V sunucusu tarafından barındırılan konuk sanal makinelerden birinde kimliği doğrulanmış bir kullanıcı tarafından VMBus'a özel hazırlanmış bir paket gönderilirse hizmet reddine olanak verebilir. Bir saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve konuk sanal makinesinden özel hazırlanmış içerik gönderebilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=198156">MS10-103</a></td>
<td style="border:1px solid black;"><strong>Microsoft Publisher'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2292970)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Publisher dosyasını Microsoft Publisher'da açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen beş güvenlik açığını giderir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=206469">MS10-104</a></td>
<td style="border:1px solid black;"><strong>Microsoft SharePoint'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2455005)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft SharePoint'teki özel olarak bildirilen bir güvenlik açığını giderir. Bir saldırgan Belge Dönüştürmeleri Yük Dengeleyici Hizmeti kullanılan bir SharePoint sunucu ortamında Belge Dönüştürmeleri Başlatıcı Hizmeti'ne özel hazırlanmış bir SOAP isteği gönderirse, bu güvenlik açığı, konuk kullanıcının güvenlik bağlamında uzaktan kod yürütülmesine izin verebilir. Belge Dönüştürmeleri Yük Dengeleyici Hizmeti ve Belge Dönüştürmeleri Başlatıcı Hizmeti varsayılan olarak, Microsoft Office SharePoint Server 2007'de etkinleştirilmemiş durumdadır.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft SharePoint</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147425">MS10-105</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Grafik Filtrelerindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (968095)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen yedi güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir resim dosyasını Microsoft Office kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, yerel kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=204624">MS10-106</a></td>
<td style="border:1px solid black;"><strong>Microsoft Exchange Server'daki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (2407132)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Exchange Server'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, kimliği doğrulanmış bir saldırgan Exchange hizmeti çalıştırılan bir bilgisayara özel hazırlanmış bir ağ iletisi gönderirse hizmet reddine olanak verebilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ yapılarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. En iyi uygulamalar, Internet'e bağlı sistemlerde olabildiğince az sayıda bağlantı noktasının açılmasını önerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Orta</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Exchange</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, yararlanılabilirlik değerlendirmesi düzeylerine ve sonra da CVE Kimliklerine göre azalan sırayla listelenmektedir. Bültenlerde yalnızca önem derecesi Kritik veya Önemli olan güvenlik açıkları yer almaktadır.
  
**Bu tabloyu nasıl kullanabilirim?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
| Bülten Kimliği                                            | Güvenlik Açığı Başlığı                                                                                | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                       |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------|  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | pubconv.dll Dosyasındaki Boyut Değerinde Öbek Bozulması Güvenlik Açığı                                | [CVE-2010-2569](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2569) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | pubconv.dll Dosyasında Öbek Taşması Güvenlik Açığı                                                    | [CVE-2010-2570](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2570) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-097](http://go.microsoft.com/fwlink/?linkid=206689) | Internet Bağlantısı Oturum Açma Sihirbazı'nda Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı | [CVE-2010-3144](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3144) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığı genel olarak duyurulmuştur**                    |  
| [MS10-096](http://go.microsoft.com/fwlink/?linkid=206738) | Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı                                               | [CVE-2010-3147](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3147) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığı genel olarak duyurulmuştur**                    |  
| [MS10-092](http://go.microsoft.com/fwlink/?linkid=203463) | Görev Zamanlayıcısı Güvenlik Açığı                                                                    | [CVE-2010-3338](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3338) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır** |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | HTML Nesnesinde Bellek Bozulması Güvenlik Açığı                                                       | [CVE-2010-3340](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3340) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | HTML Nesnesinde Bellek Bozulması Güvenlik Açığı                                                       | [CVE-2010-3343](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3343) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | HTML Öğesinde Bellek Bozulması Güvenlik Açığı                                                         | [CVE-2010-3345](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3345) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | HTML Öğesinde Bellek Bozulması Güvenlik Açığı                                                         | [CVE-2010-3346](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3346) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k'de Arabellek Taşması Güvenlik Açığı                                                            | [CVE-2010-3939](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3939) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığı genel olarak duyurulmuştur**                    |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k PFE İşaretçisinde İki Kez Bırakma Güvenlik Açığı                                               | [CVE-2010-3940](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3940) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k'de İşaretçi Bağlama Güvenlik Açığı                                                             | [CVE-2010-3943](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3943) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k'de Bellek Bozulması Güvenlik Açığı                                                             | [CVE-2010-3944](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3944) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | FlashPix Resim Dönüştürücüsünde Arabellek Taşması Güvenlik Açığı                                      | [CVE-2010-3951](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3951) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | OpenType Yazı Tipinde İki Kez Bırakma Güvenlik Açığı                                                  | [CVE-2010-3957](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3957) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | OpenType CMAP Tablosu Güvenlik Açığı                                                                  | [CVE-2010-3959](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3959) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-100](http://go.microsoft.com/fwlink/?linkid=204906) | İzin Alma UI'de Kimliğe Bürünme Güvenlik Açığı                                                        | [CVE-2010-3961](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0483) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-090](http://go.microsoft.com/fwlink/?linkid=206495) | Başlatılmamış Belleğin Bozulması Güvenlik Açığı                                                       | [CVE-2010-3962](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3962) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır** |  
| [MS10-099](http://go.microsoft.com/fwlink/?linkid=206365) | Çekirdek NDProxy'de Arabellek Taşması Güvenlik Açığı                                                  | [CVE-2010-3963](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3963) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-104](http://go.microsoft.com/fwlink/?linkid=206469) | Hatalı Biçimlendirilmiş İstek Nedeniyle Kod Yürütme Güvenlik Açığı                                    | [CVE-2010-3964](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3964) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-094](http://go.microsoft.com/fwlink/?linkid=206699) | Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı                                               | [CVE-2010-3965](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3965) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığı genel olarak duyurulmuştur**                    |  
| [MS10-095](http://go.microsoft.com/fwlink/?linkid=206683) | BranchCache'de Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı                                | [CVE-2010-3966](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3966) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                               |  
| [MS10-093](http://go.microsoft.com/fwlink/?linkid=206698) | Güvenli Olmayan Şekilde Kitaplık Yükleme Güvenlik Açığı                                               | [CVE-2010-3967](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3967) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığı genel olarak duyurulmuştur**                    |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Pubconv.dll Dosyasında Dize Dizininin Geçersiz Olması Nedeniyle Bellek Bozulması Güvenlik Açığı       | [CVE-2010-2571](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2571) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k'de İki Kez Bırakma Güvenlik Açığı                                                              | [CVE-2010-3941](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3941) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-098](http://go.microsoft.com/fwlink/?linkid=204869) | Win32k'de WriteAV Güvenlik Açığı                                                                      | [CVE-2010-3942](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3942) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | CGM Resim Dönüştürücüsünde Arabellek Taşması Güvenlik Açığı                                           | [CVE-2010-3945](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3945) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | PICT Resim Dönüştürücüsünde Tamsayı Taşması Güvenlik Açığı                                            | [CVE-2010-3946](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3946) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | TIFF Resim Dönüştürücüsünde Öbek Taşması Güvenlik Açığı                                               | [CVE-2010-3947](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3947) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | TIFF Resim Dönüştürücüsünde Arabellek Taşması Güvenlik Açığı                                          | [CVE-2010-3949](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3949) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | TIFF Resim Dönüştürücüsünde Bellek Bozulması Güvenlik Açığı                                           | [CVE-2010-3950](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3950) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-105](http://go.microsoft.com/fwlink/?linkid=147425) | FlashPix Resim Dönüştürücüsünde Öbek Bozulması Güvenlik Açığı                                         | [CVE-2010-3952](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3952) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Dize Dizininde Bellek Bozulması Güvenlik Açığı                                                        | [CVE-2010-3955](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3955) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-091](http://go.microsoft.com/fwlink/?linkid=203895) | OpenType Yazı Tipinde Dizin Güvenlik Açığı                                                            | [CVE-2010-3956](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3956) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                               |  
| [MS10-101](http://go.microsoft.com/fwlink/?linkid=201319) | Netlogon RPC'de Boş Başvuru DOS Güvenlik Açığı                                                        | [CVE-2010-2742](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-2742) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – İşlevsel bir yararlanma kodu olasılığı düşük | Bu yalnızca bir Hizmet Reddi güvenlik açığıdır                      |  
| [MS10-106](http://go.microsoft.com/fwlink/?linkid=204624) | Exchange Server'da Sonsuz Döngü Güvenlik Açığı                                                        | [CVE-2010-3937](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3937) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – İşlevsel bir yararlanma kodu olasılığı düşük | Bu yalnızca bir Hizmet Reddi güvenlik açığıdır                      |  
| [MS10-103](http://go.microsoft.com/fwlink/?linkid=198156) | Microsoft Publisher'da Bellek Bozulması Güvenlik Açığı                                                | [CVE-2010-3954](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3954) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                               |  
| [MS10-102](http://go.microsoft.com/fwlink/?linkid=205309) | Hyper-V VMBus Güvenlik Açığı                                                                          | [CVE-2010-3960](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3960) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – İşlevsel bir yararlanma kodu olasılığı düşük | Bu yalnızca bir Hizmet Reddi güvenlik açığıdır                      |
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Yok
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6031d98a-cd0f-4dd8-80b6-70a7167e9e55)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=922a0835-7f69-4e37-a9f7-c64e976e3513)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a55b8029-9499-4219-99b7-65c30b0b864a)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cdef3358-ad3e-40a6-9ba5-3be220a56a65)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=46baa431-126c-4fa5-9a7b-525008e2817d)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fa9a1aac-b9c5-4d4e-9083-a080ad4ccc6f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=bb9d1657-5beb-4372-b74c-a612a6fff5a8)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4d0ae558-a4f2-4048-b5fd-ba072ca35e48)  
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5d3a5678-77f8-4ebc-8775-aedd25ef0eb8)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a7c826b0-4aac-41ce-b297-6b6e11105c14)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d5207bf5-7e58-4001-aa8f-f9a4b2c037d8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=070fef8e-ba09-40f4-abaa-9cebf08983c3)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Önemli)  
[Windows Media Kodlayıcısı 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9ce9d62-2eaa-48d8-bb6d-ea137e63d077)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6dabc306-c858-46b1-815c-cd8d011ff62e)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1f277ae4-4f85-4c8a-bfc5-dcdc8afed133)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=238bb885-eae6-464a-bb3d-679025f1cb50)  
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
<th colspan="14">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Yok
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4f1f41fb-368a-42e6-8d17-fca83b64f57b)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a3b57d26-5551-4785-86cf-41b532d78979)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4f5a3677-0990-4702-bf08-af64cf12cb6c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9b70334c-490d-446c-988a-a88a75595fd4)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=ef0ada2c-965f-438f-a1d3-bd45db8460c1)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0b2837c-019b-419b-954d-5bdc71a3a332)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8fa2cfa4-a01d-4910-b69f-736aeb585bab)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4aa39f59-2177-459f-9b8a-9543330d48ec)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c87af292-a068-4089-aab8-115c18b4b024)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ad843b97-2f6e-4406-a17a-627b7db8a926)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=6a9f56a0-230a-4dde-94da-f051ebf51f47)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8b0d2a3a-7fed-4d48-9ec5-8558000e51bb)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=1e134e5d-84fb-432b-99b1-593b1be5d5a4)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=08328e82-b012-4ea5-bf89-becb4881084f)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=dc777e61-e1e3-43bf-a84d-22c4a69c135d)  
(Önemli)  
[Windows Media Kodlayıcısı 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=550957c2-ce66-439f-95ea-681237513f75)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c5cb600-9a39-40a0-be42-1593b1e0b97d)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=17b0b340-73b2-42a7-9d86-1297c63dcc2b)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bca61d61-d5cf-49a4-ab99-b61e50e8f619)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e17b8878-d065-49cc-bdba-0f24cdf35ea3)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b0a06e7-0ae5-41f4-9ff5-d524fc0afbfa)  
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
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=7c1cf126-604c-4f70-bbe8-aa4d145eb68f)  
(Kritik)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=96884bfa-00c8-4263-9936-d7c054919dd3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=15588d6a-f576-4e3d-95e8-d422af8a94de)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=9abc8270-f3ac-474d-9ebc-410aaa6262cc)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=04a178cc-1afd-4e47-8cab-05e402e5a568)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=4fce129d-2b4e-4a66-af27-bbbde1e65ba1)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ad896d80-167f-4e8f-a448-cac93516f4d0)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=7c0c2850-e81d-4347-aeb3-47036caa7c1b)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="14">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=897351de-9697-4954-aa7e-169e980b932c)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=bebf0df0-5ebe-44b4-9ace-b3085a993e58)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2ddb8a06-c9cc-4d33-b6d1-22dbda2d871f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=48f10251-34d8-4149-b4b2-bf3ec28f5846)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=55141a02-3ad3-4691-98b9-80dd8ecb14c5)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=e8a57950-43cd-486f-bd97-70b0ad360a0b)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a1c7f1b5-e054-4cd6-857d-2ab0a2fe9f62)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b824d3b9-2ce1-4abc-ae06-68aef1250be9)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85265a23-5094-4007-8d33-f402cabd1664)  
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=171c02f9-f7d2-42f2-ba31-4c819a43784a)  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=837b6056-af04-4aed-8afe-cc392770a590)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a245f3c-ffb6-4ccd-956c-e7d1231fca30)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=099ccc5f-b92f-4d06-bcb5-92e35c49f613)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Movie Maker 2.6](http://www.microsoft.com/downloads/details.aspx?familyid=5b078136-a492-4a2e-939d-82799f774d82)<sup>[1]</sup>
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=f98c3b96-acb5-49f1-be42-3dd44d316408)  
(Önemli)  
[Windows Media Kodlayıcısı 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=e1054088-f484-4f44-ba0e-5cbd21773c0c)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=73624b68-a69d-4517-b971-f0b7d2ccc9d6)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f4c42cfe-b7f2-4436-919e-4bd305a3439a)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63c7257a-16bf-4108-80b9-9dfe53528348)  
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
<th colspan="14">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f3785f3b-64c6-46a4-8e3a-9b9448124a8f)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=98183a76-5642-4e19-b488-029eb7ed3942)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=87149ec2-74a8-4dea-b7e3-873558e0103e)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bdc9564a-4091-4cde-963a-239513db6c17)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=a4ea028f-edfc-4237-8325-7ece11fcf437)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=118f528f-bd05-49c2-a4a4-78314cd00992)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e2f572a-4169-47f2-a872-5466997122ed)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=14e079a8-01a4-47c9-bd47-f5c9a6ca070a)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6793f75b-cdf4-42ef-a53e-a1acb5b662d1)\*  
(Önemli)
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
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4b81aae5-6034-4c83-b5d2-e7e472435284)\*\*  
(Kritik)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d47b457d-e995-4a7e-9bfa-eebab9b3a729)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=523a47d3-771d-471a-889b-16311c276a00)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dff39bfe-0799-4912-ae22-392562178ae6)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Media Kodlayıcısı 9 x86](http://www.microsoft.com/downloads/details.aspx?familyid=f468d2b5-f02c-4691-9fb5-a7f69752f126)\*\*  
(Önemli)  
[Windows Media Kodlayıcısı 9 x64](http://www.microsoft.com/downloads/details.aspx?familyid=533d91d8-0291-421e-9701-3bd86d18bc45)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=77e288fb-b51f-4f57-baac-1443d8fbd37b)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09a4b646-989d-43ef-a3e8-64af8b380a14)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6baf92b7-a336-45f2-a1ba-c00c34dfb76f)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85add876-ca5a-4a92-984e-188a72e349fc)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8c06bbc-6e84-4cf1-89f0-c0d34cfffaed)\*  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=8ddafaaf-84a0-4325-b06f-4aac7cd61274)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=959146ee-0e70-4e56-9012-72ed59aeb24b)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cf341a35-32ea-4ff7-aca9-1a4683c100ee)  
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
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=82f71194-6f1f-4f43-8752-4bf5e5f94a93)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46522323-837e-4a74-9cf0-45f69343e776)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7a4b23d4-f68e-4d5b-8814-d9247145f164)  
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
<th colspan="14">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c288fe87-b113-4615-9b02-5e388bcb5241)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=ff590db8-4264-42ba-9e07-88d100e1c4f5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=cf85cdb6-58c7-4144-82f6-f01a6a4f9c3a)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=75591d37-2cb8-4cdf-acbb-89cd0d1a9290)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=4e8ad5cd-af27-4f00-9378-ad778b8ee7b3)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=aa7de2e4-ba48-4d58-b034-05349f0eb920)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=f7c7d57a-d031-46a3-9613-eae2b9cb6401)  
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
x64 tabanlı sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2cf4ac70-88b4-4840-9895-2bcf119312a7)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=4ea4e339-9db2-4b99-b567-80ee55ecdf92)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=0597018d-39f5-4ca9-b437-63d9e68f264d)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=3a0c4dd0-98b4-4e7a-99ed-22b9d9f76cd1)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=35a3e821-b463-411c-858b-d01eb5aed42b)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=b21db627-91c2-4ebf-b7c0-38ac58ae5b6c)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=e52c36f5-637b-4928-83d0-27514c6cc384)  
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
<th colspan="14">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-090**](http://go.microsoft.com/fwlink/?linkid=206495)
</td>
<td style="border:1px solid black;">
[**MS10-091**](http://go.microsoft.com/fwlink/?linkid=203895)
</td>
<td style="border:1px solid black;">
[**MS10-092**](http://go.microsoft.com/fwlink/?linkid=203463)
</td>
<td style="border:1px solid black;">
[**MS10-093**](http://go.microsoft.com/fwlink/?linkid=206698)
</td>
<td style="border:1px solid black;">
[**MS10-094**](http://go.microsoft.com/fwlink/?linkid=206699)
</td>
<td style="border:1px solid black;">
[**MS10-095**](http://go.microsoft.com/fwlink/?linkid=206683)
</td>
<td style="border:1px solid black;">
[**MS10-096**](http://go.microsoft.com/fwlink/?linkid=206738)
</td>
<td style="border:1px solid black;">
[**MS10-097**](http://go.microsoft.com/fwlink/?linkid=206689)
</td>
<td style="border:1px solid black;">
[**MS10-098**](http://go.microsoft.com/fwlink/?linkid=204869)
</td>
<td style="border:1px solid black;">
[**MS10-099**](http://go.microsoft.com/fwlink/?linkid=206365)
</td>
<td style="border:1px solid black;">
[**MS10-100**](http://go.microsoft.com/fwlink/?linkid=204906)
</td>
<td style="border:1px solid black;">
[**MS10-101**](http://go.microsoft.com/fwlink/?linkid=201319)
</td>
<td style="border:1px solid black;">
[**MS10-102**](http://go.microsoft.com/fwlink/?linkid=205309)
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
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=99a91ba7-035b-4717-ada5-c1ad6645db64)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=e52f7869-474a-44c8-a102-e766c576fc01)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=28c832fb-4937-4652-8799-eab6c76d05fb)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=f58a765f-cea9-456d-b0ab-bfc70b109cbf)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9e2c95f6-9381-4484-b11b-814ab9138118)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=d417ebce-7841-4bbb-8abc-b15ef5f4b733)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=b823a7aa-0eb9-42dd-bf56-8907d94b314a)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=d7307afd-84a0-434e-9658-bf9f8ae4b938)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=39b7abc7-65a4-4dfd-92ba-c638e3de1118)\*  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c26de145-94b8-404a-b946-744988fab83b)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=a21d061a-794a-4012-b3cd-c67445c074f5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=3ad64d5c-2d81-4ac8-934e-8917b2fcf961)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=13a9f838-ac07-43dc-9aee-a77207998e1e)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=cb4211f3-1082-4245-8f03-7cbac90e9a31)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=7eeac1bb-9f86-4ea5-b30f-980d52be5044)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=66b2506d-80e0-4e32-86e6-0908ef56ae90)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**Windows Server 2008 ve Windows Server 2008 R2 için Notlar**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği Yüklemesini Yönetme](http://technet.microsoft.com/en-us/library/ee441255(ws.10).aspx) ve [Sunucu Çekirdeği Yüklemesine Hizmet Verme](http://technet.microsoft.com/en-us/library/ff698994(ws.10).aspx) adlı TechNet makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS10-093 için Not**

<sup>[1]</sup>Windows Movie Maker 2.6, belirtilen işletim sistemlerine yüklenebilen isteğe bağlı bir karşıdan yüklemedir.

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
[**MS10-103**](http://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](http://go.microsoft.com/fwlink/?linkid=147425)
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f540692c-e404-4383-8937-4d6a36475da5)  
(KB2284692)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=724d0ad6-ba5f-4dbf-b280-3fb36335d33b)<sup>[1]</sup>
(KB2289162)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e600de65-3e9d-4e37-8906-8b7091ff523e)  
(KB2284695)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=976857e9-77fc-4667-88ca-7637e57536cd)<sup>[1]</sup>
(KB2289163)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=79275011-bdc1-446a-8ea6-56fc31bd9c35)  
(KB2284697)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=676eeed6-f2b7-4265-afc7-a82ffdbeb290)  
(KB2288931)  
(Önem derecesi yok<sup>[2]</sup>)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=99e18990-75e9-497e-9b4f-5d7ef8656ab2)  
(KB2409055)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=6d644494-b530-4b37-bc37-8a8a7edefe53)  
(KB2289078)  
(Önem derecesi yok<sup>[2]</sup>)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=9b27ee11-e563-4152-9691-25eec1ee9966)  
(KB2409055)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=58e54779-aa8f-41b3-9993-8cec12c49082)  
(KB2289078)  
(Önem derecesi yok<sup>[2]</sup>)
</td>
</tr>
<tr>
<th colspan="3">
Diğer Office Yazılımları
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-103**](http://go.microsoft.com/fwlink/?linkid=198156)
</td>
<td style="border:1px solid black;">
[**MS10-105**](http://go.microsoft.com/fwlink/?linkid=147425)
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
Microsoft Office Dönüştürücü Paketi
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Dönüştürücü Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=dcded2ee-0673-4afe-abe6-04941a2ad306)  
(KB2456849)  
(Önemli)
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
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=10f6f330-05d8-4b60-9ebb-822a7321ac0f)  
(KB2431831)  
(Önemli)
</td>
</tr>
</table>
 
**MS10-105 için Notlar**

<sup>[1]</sup>Belirtilen yazılımları kullanan müşterilerin MS10-105'te açıklanan güvenlik açıklarına karşı korunabilmeleri için MS10-087'de sağlanan Microsoft Office güncelleştirmesini de yüklemeleri gerekmektedir.

<sup>[2]</sup>Bu bültende açıklanan güvenlik açıkları bu yazılımı etkilemediği için önem dereceleri bu güncelleştirmeye uygulanmamıştır. Ancak Microsoft gelecekte tanımlanabilecek olası saldırı sektörlerine karşı kapsamlı bir savunma önlemi olarak, bu yazılımı kullanan müşterilerin bu güvenlik güncelleştirmesini uygulamalarını önerir.

#### Microsoft Server Yazılımı

 
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
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-104**](http://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](http://go.microsoft.com/fwlink/?linkid=204624)
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
Microsoft Office SharePoint Server 2007 Service Pack 2 (32-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=3c8fb9f9-7920-43ea-b618-e26dc3360c60)  
(KB2433089)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007 Service Pack 2 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 2 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=3db09280-24bd-42e0-9ae3-02c9bf3e8ee3)  
(KB2433089)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-104**](http://go.microsoft.com/fwlink/?linkid=206469)
</td>
<td style="border:1px solid black;">
[**MS10-106**](http://go.microsoft.com/fwlink/?linkid=204624)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Microsoft Exchange Server 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Microsoft Exchange Server 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7b983156-9e9f-4d29-9e9b-2369747e3b62)  
(KB2407132)  
(Orta)
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

**System Center** **Configuration Manager 2007**

Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, kuruluş genelindeki BT sistemlerine yönelik güncelleştirmeleri teslim etme ve yönetme görevini kolaylaştırır. Configuration Manager 2007 ile, BT yöneticileri Microsoft ürünlerine yönelik güncelleştirmeleri masaüstü bilgisayarlar, dizüstü bilgisayarlar, sunucular ve mobil aygıtlar gibi çeşitli aygıtlara teslim edebilirler.

Configuration Manager 2007'deki otomatik güvenlik açığı değerlendirmesi, güncelleştirme gereksinimini belirler ve önerilen eylemleri bildirir. Configuration Manager 2007'deki Yazılım Güncelleştirme Yönetimi, BT yöneticileri tarafından dünya genelinde kullanılan ve zaman içinde kendini kanıtlamış bir güncelleştirme altyapısı olan Microsoft Windows Software Update Services'a (WSUS) dayalıdır. Yöneticilerin güncelleştirmeleri dağıtmak üzere Configuration Manager 2007'yi nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Yazılım Güncelleştirme Yönetimi](http://www.microsoft.com/systemcenter/en/us/configuration-manager/cm-software-update-management.aspx). Configuration Manager hakkında daha fazla bilgi için, [System Center Configuration Manager](http://www.microsoft.com/systemcenter/en/us/configuration-manager.aspx)'ı sayfasını ziyaret edin.

**Systems Management Server 2003**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir.

**Not** System Management Server 2003, 12 Ocak 2010'dan itibaren temel destek dışında kalmıştır. Ürün ömrü hakkında daha fazla bilgi için, [Microsoft Destek Ömrü](http://support.microsoft.com/common/international.aspx?rdpath=dm;en-us;lifecycle) Web sitesini ziyaret edin. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; önceki bölüm olan **System Center** **Configuration Manager 2007** konusuna bakın.

Yöneticilerin güvenlik güncelleştirmelerini dağıtmak üzere SMS 2003'ü nasıl kullanabilecekleri hakkında daha fazla bilgi için, bkz: [Microsoft Systems Management Server 2003 Senaryoları ve Yordamları: Yazılım Dağıtımı ve Düzeltme Eki Yönetimi](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). SMS hakkında bilgi için, [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx)'ı ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler bu güncelleştirmeleri yüklemek için, Elevated Rights Deployment Tool'u kullanabilirler ([SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/en/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=en) içinde bulunur).

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

-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Aniway, MS10-090'da açıklanan sorunu bildirdiği için
-   [VUPEN Vulnerability Research Team](http://www.vupen.com/) için çalışan Nicolas Joly, MS10-090'da açıklanan sorunu bildirdiği için
-   Stephen Fewer, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-090'da açıklanan sorunu bildirdikleri için
-   [Peter Vreugdenhil](http://vreugdenhilresearch.nl/), [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-090'da açıklanan sorunu bildirdikleri için
-   [AZIA CO., LTD.](http://www.azia.jp) için çalışan Masatoshi Sato, MS10-090'da açıklanan sorunu bildirdiği için
-   [Yosuke Hasegawa](http://utf-8.jp/), MS10-090'da açıklanan sorun konusunda bizimle çalıştığı için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Jose Antonio Vazquez Gonzalez, MS10-090'da açıklanan sorunu bildirdiği için
-   [Red Hat Security Response Team](https://www.redhat.com/security/team/) için çalışan Marc Schoenefeld, [Opera Security Team](http://www.opera.com/security/) ile birlikte çalışarak MS10-091'de açıklanan sorunu bildirdikleri için
-   [Red Hat Security Response Team](https://www.redhat.com/security/team/) için çalışan Marc Schoenefeld, MS10-091'de açıklanan sorunu bildirdiği için
-   Paul-Kenji Cahier Furuya, MS10-091'de açıklanan sorunu bildirdiği için
-   [Kaspersky Lab](http://usa.kaspersky.com/) için çalışan Sergey Golovanov, Alexander Gostev, Maxim Golovkin ve Alexey Monastyrsky ile [Design and Test Lab](http://www.dnt-lab.com/) için çalışan Vitaly Kiktenko ve Alexander Saprykin, MS10-092'de açıklanan sorunu bildirdikleri için
-   [Symantec](http://www.symantec.com/index.jsp) için çalışan Liam O Murchu, MS10-092'de açıklanan sorunu bildirdiği için
-   [ESET](http://www.eset.com/) için çalışan Alexandr Matrosov, Eugene Rodionov, Juraj Malcho ve David Harley, MS10-092'de açıklanan sorunu bildirdikleri için
-   [Fortinet bünyesindeki FortiGuard Labs](http://www.fortiguard.com/) için çalışan Haifei Li, MS10-095'te açıklanan sorunu bildirdiği için
-   [ACROS Security](http://www.acrossecurity.com/) için çalışan Simon Raner, MS10-096'da açıklanan sorunu bildirdiği için
-   [Rapid7](http://www.rapid7.com/) için çalışan HD Moore, MS10-096'da açıklanan sorunu bildirdiği için
-   [NGS Software](http://www.ngssoftware.com/) için çalışan Muhaimin Dzulfakar, MS10-096'da açıklanan sorunu bildirdiği için
-   [NGS Software](http://www.ngssoftware.com/) için çalışan Muhaimin Dzulfakar, MS10-097'de açıklanan sorunu bildirdiği için
-   [Norman](http://www.norman.com/) için çalışan Tarjei Mandt, MS10-098'de açıklanan sorunu bildirdiği için
-   [Sysdream](http://www.sysdream.com/) için çalışan Stéfan Le Berre, MS10-098'de açıklanan sorunu bildirdiği için
-   [Fortinet bünyesindeki FortiGuard Labs](http://www.fortiguard.com/) için çalışan Honggang Ren, MS10-099'da açıklanan sorunu bildirdiği için
-   [Argeniss](http://www.argeniss.com/) için çalışan Cesar Cerrudo, MS10-100'de açıklanan sorunu bildirdiği için
-   The Samba Team için çalışan Matthias Dieter Wallnöfer ve Andrew Bartlett, MS10-101'de açıklanan sorunu bildirdikleri için
-   [HP](http://www.hp.com/) ve [techit](http://www.techit.de), MS10-102'de açıklanan sorunu bildirdikleri için
-   [VUPEN Vulnerability Research Team](http://www.vupen.com/) için çalışan Chaouki Bekrar, MS10-103'te açıklanan beş sorunu bildirdiği için
-   Oleksandr Mirosh, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-104'te açıklanan sorunu bildirdikleri için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, MS10-105'te açıklanan iki sorunu bildirdiği için
-   [Secunia Research](http://secunia.com/) için çalışan Alin Rad Pop, MS10-105'te açıklanan sorunu bildirdiği için
-   [Secunia Research](http://secunia.com/) için çalışan Carsten Eiram, MS10-105'te açıklanan üç sorunu bildirdiği için
-   [Secunia Research](http://secunia.com/) için çalışan Dyon Balding, MS10-105'te açıklanan iki sorunu bildirdiği için
-   Oleksandr Mirosh, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-106'da açıklanan sorunu bildirdikleri için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (14 Aralık 2010): Bülten Özeti yayımlandı.
-   V1.1 (15 Aralık 2010): Microsoft Office XP ve Microsoft Office 2003 müşterilerinin MS10-105'te açıklanan güvenlik açıklarından korunmaları için MS10-087'de sağlanan güncelleştirmeyi uygulamaları gerektiği açıklığa kavuşturuldu.

*Built at 2014-04-18T01:50:00Z-07:00*
