---
TOCTitle: 'MS10-FEB'
Title: Microsoft Güvenlik Bülteni Şubat 2010 Özeti
ms:assetid: 'ms10-feb'
ms:contentKeyID: 61235827
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms10-feb(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Şubat 2010 Özeti
===========================================

Yayım Tarihi: 9 Şubat 2010 Salı | Güncelleştirme Tarihi: 10 Şubat 2010 Çarşamba

**Sürüm:** 1.1

Bu bülten özetinde Şubat 2010'da yayımlanan güvenlik bültenleri listelenir.

Şubat 2010 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 4 Şubat 2010'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 10 Şubat 2010 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Şubat Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032427679&culture=en-us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178850">MS10-006</a></td>
<td style="border:1px solid black;"><strong>SMB İstemcisi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (978251)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen iki güvenlik açığını giderir. Güvenlik açıkları, bir saldırgan istemci tarafından başlatılan bir SMB isteğine özel hazırlanmış bir SMB yanıtı gönderirse uzaktan kod yürütülmesine izin verebilir. Saldırganın bu güvenlik açıklarından yararlanabilmesi için, kullanıcıyı kötü amaçlı bir SMB sunucusuna SMB bağlantısı oluşturmaya ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179067">MS10-007</a></td>
<td style="border:1px solid black;"><strong>Windows Kabuğu İşleyicisi'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (975713)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows 2000, Windows XP ve Windows Server 2003'teki özel olarak bildirilen bir güvenlik açığını giderir. Windows'un diğer sürümleri bu güvenlik açığından etkilenmez. Bu güvenlik açığı, Web tarayıcısı gibi bir uygulama Windows Kabuğu İşleyicisi aracılığıyla ShellExecute API işlevine özel hazırlanmış veriler gönderirse uzaktan kod yürütülmesine izin verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179106">MS10-008</a></td>
<td style="border:1px solid black;"><strong>ActiveX Kill Bitlerine Yönelik Toplu Güvenlik Güncelleştirmesi (978262)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft yazılımlarındaki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik güncelleştirmesi Microsoft Windows 2000 ve Windows XP'nin tüm desteklenen sürümleri için Kritik, Windows Vista ve Windows 7'nin tüm desteklenen sürümleri için Önemli, Windows Server 2003'ün tüm desteklenen sürümleri için Orta, Windows Server 2008 ve Windows Server 2008 R2'nin tüm desteklenen sürümleri için Düşük olarak derecelendirilmiştir.<br />
<br />
Güvenlik açığı, bir kullanıcı Internet Explorer kullanarak bir ActiveX denetiminin örneğini oluşturan özel hazırlanmış bir Web sayfasını görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Bu güncelleştirme ayrıca üçüncü taraflara ait dört ActiveX denetiminin kill bitlerini de içerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167190">MS10-009</a></td>
<td style="border:1px solid black;"><strong>Windows TCP/IP'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (974145)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen dört güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, IPv6'nın etkinleştirilmiş olduğu bir bilgisayara özel hazırlanmış paketler gönderilirse uzaktan kod yürütülmesine olanak verebilir. Saldırgan, özel hazırlanmış ICMPv6 paketleri oluşturup bu paketleri IPv6'nın etkinleştirilmiş olduğu bir sisteme göndermek yoluyla bu açıktan yararlanmaya çalışabilir. Saldırgan yalnızca bağlantı üzerindeyse bu güvenlik açığından yararlanabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=167321">MS10-013</a></td>
<td style="border:1px solid black;"><strong>Microsoft DirectShow'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (977935)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft DirectShow'daki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir AVI dosyasını açtıysa uzaktan kod yürütülmesine izin verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=178812">MS10-003</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office'teki (MSO) Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (978214)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Office dosyasını Microsoft Office'te açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen bir güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=163639">MS10-004</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office PowerPoint'teki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (975416)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office PowerPoint'teki özel olarak bildirilen altı güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir PowerPoint dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179066">MS10-010</a></td>
<td style="border:1px solid black;"><strong>Windows Server 2008 Hyper-V'deki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (977894)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Server 2008 Hyper-V ve Windows Server 2008 R2 Hyper-V'deki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, Hyper-V sunucusu tarafından barındırılan konuk sanal makinelerden birinde kimliği doğrulanmış bir kullanıcı tarafından makine yönergeleri hatalı biçimlendirilmiş bir sırayla çalıştırılırsa hizmet reddine olanak verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için, geçerli oturum açma kimlik bilgilerine sahip olması ve konuk sanal makinede yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179798">MS10-011</a></td>
<td style="border:1px solid black;"><strong>Windows İstemci Sunucu Çalışma Zamanı Alt Sistemi'ndeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (978037)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows 2000, Windows XP ve Windows Server 2003'teki Microsoft Windows İstemci Sunucu Çalışma Zamanı Alt Sistemi'nde özel olarak bildirilen bir güvenlik açığını giderir. Windows'un diğer sürümleri bu açıktan etkilenmez. Bu güvenlik açığı, bir saldırgan sistemde oturum açar ve çalışmaya devam edecek şekilde özel olarak tasarlanmış bir uygulamayı başlatırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açığı anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=155976">MS10-012</a></td>
<td style="border:1px solid black;"><strong>SMB Sunucusu'ndaki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (971468)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen birkaç güvenlik açığını giderir. Bu güvenlik açıklarının önem düzeyi en yüksek olanı, bir saldırgan özel hazırlanmış bir SMB paketi oluşturup bu paketi etkilenen bir sisteme gönderirse uzaktan kod yürütülmesine olanak verebilir. Güvenlik duvarlarına yönelik en iyi uygulamalar ve standart olarak kullanılan varsayılan güvenlik duvarı yapılandırmaları, bu güvenlik açıklarından yararlanmak üzere işletme dışından gerçekleştirilen saldırılardan ağların korunmasına yardımcı olabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=181196">MS10-014</a></td>
<td style="border:1px solid black;"><strong>Kerberos Güvenlik Açığı Hizmet Reddine Olanak Verebilir (977290)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, Windows Kerberos dışındaki güvenilen bir alanda yer alan kimliği doğrulanmış bir kullanıcıdan Windows Kerberos etki alanına özel hazırlanmış bir anahtar yenileme isteği gönderilirse hizmet reddine olanak verebilir. Hizmet reddi durumu, etki alanı denetleyicisi yeniden başlatılıncaya kadar devam edebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=179062">MS10-015</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (977165)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki genel olarak duyurulan ve özel olarak bildirilen birer güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açıklarından birinden yararlanabilmesi için, geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=180620">MS10-005</a></td>
<td style="border:1px solid black;"><strong>Microsoft Paint'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (978706)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Paint'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir JPEG görüntü dosyasını Microsoft Paint kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Orta</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, yararlanılabilirlik değerlendirmesi düzeylerine ve sonra da CVE Kimliklerine göre azalan sırayla listelenmektedir.
  
**Bu tabloyu nasıl kullanacağım?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
| Bülten Kimliği                                            | Güvenlik Açığı Başlığı                                                            | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                                                                  |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------|  
| [MS10-006](http://go.microsoft.com/fwlink/?linkid=178850) | SMB İstemcisi'nde Yarış Durumu Güvenlik Açığı                                     | [CVE-2010-0017](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0017) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Uzaktan saldırı vektörü, DoS'ye yol açabilir; yerel saldırı vektörü, EoP'ye yol açabilir                       |  
| [MS10-011](http://go.microsoft.com/fwlink/?linkid=179798) | CSRSS'de Yerel Ayrıcalık Yükselmesi Güvenlik Açığı                                | [CVE-2010-0023](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0023) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Saldırganın ve kurbanın aynı konsolda oturum açmış olmaları gerekir                                            |  
| [MS10-007](http://go.microsoft.com/fwlink/?linkid=179067) | URL Doğrulaması Güvenlik Açığı                                                    | [CVE-2010-0027](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0027) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | PowerPoint LinkedSlideAtom Öbek Taşması Güvenlik Açığı                            | [CVE-2010-0030](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0030) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | PowerPoint OEPlaceholderAtom 'placementId' Geçersiz Dize Dizini Güvenlik Açığı    | [CVE-2010-0031](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0031) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | PowerPoint OEPlaceholderAtom Serbest Bırakıldıktan Sonra Kullanma Güvenlik Açığı  | [CVE-2010-0032](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0032) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | PowerPoint Viewer'daki TextBytesAtom Kaydında Yığın Taşması Güvenlik Açığı        | [CVE-2010-0033](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0033) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Güvenlik açığı yalnızca PowerPoint Viewer 2003'ü etkiler                                                       |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | Office PowerPoint Viewer'daki TextCharsAtom Kaydında Yığın Taşması Güvenlik Açığı | [CVE-2010-0034](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0034) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Güvenlik açığı yalnızca PowerPoint Viewer 2003'ü etkiler                                                       |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | SMB'de NTLM Kimlik Doğrulaması Sırasında Yetersiz Entropi Güvenlik Açığı          | [CVE-2010-0231](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0231) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-015](http://go.microsoft.com/fwlink/?linkid=179062) | Windows Çekirdeğinde Özel Durum İşleyicisi Güvenlik Açığı                         | [CVE-2010-0232](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0232) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-003](http://go.microsoft.com/fwlink/?linkid=178812) | MSO.DLL Dosyasında Arabellek Taşması Güvenlik Açığı                               | [CVE-2010-0243](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0243) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-013](http://go.microsoft.com/fwlink/?linkid=167321) | DirectShow'da Öbek Taşması Güvenlik Açığı                                         | [CVE-2010-0250](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0250) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                          |  
| [MS10-006](http://go.microsoft.com/fwlink/?linkid=178850) | SMB İstemcisi'nde Havuz Bozulması Güvenlik Açığı                                  | [CVE-2010-0016](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0016) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                          |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | SMB'de Yol Adı Taşması Güvenlik Açığı                                             | [CVE-2010-0020](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0020) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                          |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | SMB'de Bellek Bozulması Güvenlik Açığı                                            | [CVE-2010-0021](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0021) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                          |  
| [MS10-005](http://go.microsoft.com/fwlink/?linkid=180620) | MS Paint'te Tamsayı Taşması Güvenlik Açığı                                        | [CVE-2010-0028](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0028) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Yararlanma girişiminin başarılı olması için önemli ölçüde kullanıcı etkileşimi gerekmektedir                   |  
| [MS10-004](http://go.microsoft.com/fwlink/?linkid=163639) | PowerPoint'te Dosya Yolunu İşleme Sırasında Arabellek Taşması Güvenlik Açığı      | [CVE-2010-0029](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0029) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                          |  
| [MS10-015](http://go.microsoft.com/fwlink/?linkid=179062) | Windows Çekirdeğinde İki Kez Bırakma Güvenlik Açığı                               | [CVE-2010-0233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                          |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | ICMPv6 Yönlendirici Bildirisi Güvenlik Açığı                                      | [CVE-2010-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0239) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Yararlanılabilmesi için, saldırganın hedef ana bilgisayar ile aynı bağlantı üzerinde olması gerekir            |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | Üstbilgi MDL'sinde Bölünme Güvenlik Açığı                                         | [CVE-2010-0240](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0240) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenlik açığı, üçüncü taraflara ait bir ağ sürücüsü gerektirir                                                |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | ICMPv6 Yönlendirme Bilgileri Güvenlik Açığı                                       | [CVE-2010-0241](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0241) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Yararlanılabilmesi için, saldırganın hedef ana bilgisayar ile aynı bağlantı üzerinde olması gerekir            |  
| [MS10-012](http://go.microsoft.com/fwlink/?linkid=155976) | SMB'de Boş İşaretçi Güvenlik Açığı                                                | [CVE-2010-0022](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0022) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                          |  
| [MS10-010](http://go.microsoft.com/fwlink/?linkid=179066) | Hyper-V'de Yönerge Kümesi Doğrulaması Güvenlik Açığı                              | [CVE-2010-0026](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0026) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Güvenlik açığı yalnızca DoS durumuna olanak verebilir                                                          |  
| [MS10-014](http://go.microsoft.com/fwlink/?linkid=181196) | Kerberos'ta Boş İşaretçi Başvurusu Güvenlik Açığı                                 | [CVE-2010-0035](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0035) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Yalnızca DoS; yalnızca varsayılan olmayan yapılandırmaya sahip etki alanı denetleyicilerinden yararlanılabilir |  
| [MS10-009](http://go.microsoft.com/fwlink/?linkid=167190) | TCP/IP Seçmeli Onayı Güvenlik Açığı                                               | [CVE-2010-0242](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-0242) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                          |
  
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
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=80b49bab-6c2f-48a8-a901-ca3f76e4fe6b)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=92234237-a8eb-4ce4-bc5e-cd86feb7dbd3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=543dc6a7-fa76-4ba9-81e4-25fdf2013548)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=ba110440-10ce-40a0-884a-8b9afd45a3e3)  
(KB977914)  
(Kritik)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=16787c93-2c95-4c13-8492-be1db9d18146)  
(KB975560)  
(Kritik)  
[DirectX 9.0'daki Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=59a8bc19-02bb-4800-bac1-464f59e1cb7b)<sup>[1]</sup>
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=456185b5-57d1-4fa5-a4a9-5b2006ede3ad)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=267ce982-54a0-418f-ad52-e4963610f714)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=56a9afba-a6ee-4fb9-ba85-e51d9f94de27)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=ed8ac6a5-c8bb-4ed4-8994-810e9a1863c3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=e5861705-8f49-45cb-8a92-cf052ccf4134)  
(Orta)
</td>
</tr>
<tr>
<th colspan="12">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f6c4472e-385c-4412-bda9-c2e615e50713)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b8e7bf17-a037-4200-9ae2-2280b19766a4)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7bcf3945-0552-478e-b7f3-bbca97dd1b5d)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=a9beb2bd-e5f6-43f9-bbcc-a2afee5e5ceb)  
(KB977914)  
(Kritik)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7ab53be3-3f42-4e61-a2bc-3ed41d8736ff)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b9234b40-1b1c-498b-90d4-0bff347b36ee)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8f7adee3-e68e-41b3-b835-d84691774f31)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e2b348f5-ec8d-4782-bb03-5de550adea77)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b2e70df6-7728-4fc3-8df7-8ddb9ba5202f)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63e15ff0-73b3-46c9-96f8-c18977d35a10)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b8d83f30-9cd7-4d6b-b2b9-65d0a483cb9c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25ef97e8-e76e-44c2-953c-f94cbac552cf)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=dedc3010-a989-45f7-b9d4-f7079db3e572)  
(KB977914)  
(Kritik)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7543e819-cd36-4e89-9850-60f00c50999d)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1f83bf7a-e16c-404a-89bd-f65843938299)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=91ee57f2-81e5-49bd-bdfc-d3e385efc8a5)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e534d00c-6ddc-4eb3-9464-5db6e90afa3e)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8c4acc8-c2f4-41f7-9b32-e7bd791e0155)  
(Orta)
</td>
</tr>
<tr>
<th colspan="12">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=feb8c145-7c30-45fa-a6f0-8b6453ddd521)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5cb2e203-18fb-4887-a1c9-289d86b8ba11)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=29ff72f7-1663-4f35-a794-2dfe3c17b39c)  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=cc5150d7-070e-4a87-9c02-d050a8cb2204)  
(KB977914)  
(Kritik)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=983c5484-6321-4765-97ec-8d42d42d1f70)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c8c4eec-255e-41d5-b1e6-f0204edcb46f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3d18cbc4-ac48-458c-8aa3-90708fd854ff)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=738e2fda-96fc-413d-a5c7-74b1fac1d6b3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=defd8603-ed9b-42f9-a539-2b6a690e9575)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c1efbe73-fc87-4e6a-8b36-81f125a27aec)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36d88c1b-814c-4371-9ed2-d4576f419fc3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=90360537-9311-45e2-8047-9a971f90c3c3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d4a97bb7-4f74-4884-9a6e-7a4df9c540fb)  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=db13e99b-2f2a-4474-8d6e-271b025bd07f)  
(KB977914)  
(Kritik)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7dc20252-6091-407b-befc-c25e8f5d3fb0)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=de0186f6-27a2-4226-b8eb-f2912710f072)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d63c95e-311a-446f-8852-dffd217a89f6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f8ad539d-8191-4864-977b-ad4e31c04ba0)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9873c962-9d3d-46ef-b54b-2a50696fb6b2)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9143e435-f0d6-464b-9273-4d1f38f8ff3a)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=622442b0-cffe-4fc2-94a8-edff9d71ecd3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=d695ca9f-a1db-4c0f-94b6-7112861c28da)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=b84f0be4-6d11-4b07-bb3c-2c76ae9ceea8)  
(Orta)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[AVI Filtresi](http://www.microsoft.com/downloads/details.aspx?familyid=aec66173-e2c6-4c39-8d60-8fbef6d7b764)  
(KB977914)  
(Önemli)  
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=b1a7533a-913f-4054-b579-489a257bae5f)  
(KB975560)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=87732f7a-9339-43bc-a4e8-3da849f35b70)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ee7f8cc4-f7fd-4dc7-808c-436204ee80cb)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=d549c927-add7-4d83-bfc7-15dc35663dfb)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=c3c21225-8534-4c7f-96b6-20a743dcea74)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ee603435-26af-4ab9-9f22-92734346dc0a)  
(Orta)
</td>
</tr>
<tr>
<th colspan="12">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
Yok
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1902fc93-0f4b-4261-9da3-17d1931daf2e)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c897ddd-f441-41d4-b5b4-d794cfc96e6b)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=71f03946-622c-4403-b94f-f6a3de18a8c3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=7130ce0f-df38-4c96-ac54-cdbff35f03e7)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=16494dac-553a-4de9-b751-0d6b51cb43f0)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2761c7b4-d472-4f00-949b-af3ebafdc08d)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7c2f89b5-a3b3-42cd-857d-923fe8b8f1da)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f349f7aa-d020-4e0d-a35f-518a63ec92df)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=519815fd-707d-476f-9e29-7b03b7a17af5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=de7b7c8f-bd0a-4e13-bd58-d95507a6274b)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cec582b3-e37f-448e-a5c3-6abdcee9e57c)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=38b40dab-6b4d-434b-9997-12ef70d6bbcc)  
(Önemli)
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
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
<td style="border:1px solid black;">
[**Düşük**](http://go.microsoft.com/fwlink/?linkid=21140)
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
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=09e19263-18ba-495e-bcf7-719e957204a7)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9a85b1bf-7427-47d0-9e1b-21dbe824a62c)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc451228-3de4-427c-b42f-91f204c708b8)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=5ac0a948-0bdc-4c10-9b88-16a5d7092e47)\*\*  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=597b2310-2cd8-4d0f-8248-781eb8b7450a)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=75327470-0f14-4cdd-bcb7-64684c61c267)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=21e87558-9bd2-4aa9-aaa5-7fd26a5b60e6)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=180c2313-5e3e-4d84-87cd-64048f51e0f6)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fde218c3-90ab-4664-852d-25ca55835054)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3a889152-5d7c-4a3e-b4f1-c6507b739ca0)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=362fea40-649b-4471-aad7-db29edd0ac10)\*\*  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3463a63c-e88a-4036-ab60-f84d4bf4191a)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=67119fb6-e517-46f4-ab0b-2351cdc3d670)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0f8f81-fc10-450a-a653-06f89acba9fa)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b93047d-f2c6-403b-9200-c251898bc1e0)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=614eaf7e-95aa-4f8f-910c-1980e1f14d11)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b6e9451-df38-4626-bb1d-4fc160d7a40e)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1cd1882b-8e55-47ea-a82a-68bb59a500a7)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=effa638b-cfc1-4777-8219-7b433ed5e717)  
(KB975560)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f90fc0c8-babe-4224-be07-614ea7ddf102)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cd6b234b-8e96-4128-a77a-645a0882996a)  
(Önemli)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=a589431a-93dc-42cd-a74e-d9c1e3452fef)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=ec6d996f-dffa-45ad-9467-e96a4ac63e5f)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=4ec49aa2-81df-4e65-80da-6201394c4089)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=122fc003-0651-4ad2-a5c8-a21536defad8)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=66f14bb4-40fc-4ae3-9baf-429b7106cd91)  
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
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=3c1edcf8-d304-45c4-9818-1cd86383b3fe)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=b3265576-04c1-48b1-8ce9-128843c58cf5)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=a8a2519c-3b89-4987-9473-920adafc78cb)  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=3e096468-db6c-45c6-bee5-eaeaa63500b5)  
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
<th colspan="12">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-006**](http://go.microsoft.com/fwlink/?linkid=178850)
</td>
<td style="border:1px solid black;">
[**MS10-007**](http://go.microsoft.com/fwlink/?linkid=179067)
</td>
<td style="border:1px solid black;">
[**MS10-008**](http://go.microsoft.com/fwlink/?linkid=179106)
</td>
<td style="border:1px solid black;">
[**MS10-009**](http://go.microsoft.com/fwlink/?linkid=167190)
</td>
<td style="border:1px solid black;">
[**MS10-013**](http://go.microsoft.com/fwlink/?linkid=167321)
</td>
<td style="border:1px solid black;">
[**MS10-010**](http://go.microsoft.com/fwlink/?linkid=179066)
</td>
<td style="border:1px solid black;">
[**MS10-011**](http://go.microsoft.com/fwlink/?linkid=179798)
</td>
<td style="border:1px solid black;">
[**MS10-012**](http://go.microsoft.com/fwlink/?linkid=155976)
</td>
<td style="border:1px solid black;">
[**MS10-014**](http://go.microsoft.com/fwlink/?linkid=181196)
</td>
<td style="border:1px solid black;">
[**MS10-015**](http://go.microsoft.com/fwlink/?linkid=179062)
</td>
<td style="border:1px solid black;">
[**MS10-005**](http://go.microsoft.com/fwlink/?linkid=180620)
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
<td style="border:1px solid black;">
[**Düşük**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Yok
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=ecb06350-47a7-48eb-825f-3e8f89c5ca8e)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=cda31c54-8b81-4185-a623-64480ad4b73c)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=a9811baa-1500-4c73-940b-57f8c5456891)\*\*  
(KB975560)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=3214b347-d901-4aac-85ce-676e4602de87)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=dc757b6d-f0f8-4e71-ab6f-1417233eedf9)\*  
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
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=badd6cab-7738-4401-a68c-c15414388601)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=43fa4e26-160f-4aa3-a03d-b98a79666a18)  
(Düşük)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Quartz](http://www.microsoft.com/downloads/details.aspx?familyid=2ed23bf5-6217-413c-a7ba-eccc82139d68)  
(KB975560)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=d5b0b1eb-24f3-47ec-aba1-c1b95400189e)  
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
</table>
 
**MS10-013 için Not**

<sup>[1]</sup>DirectX 9.0 güncelleştirmesi, Microsoft Windows 2000 üzerinde DirectX 9.0a, DirectX 9.0b ve DirectX 9.0c için de uygulanır.

**Windows Server 2008 ve Windows Server 2008 R2 için Notlar**

**\*Sunucu Çekirdeği yüklemesi etkilenir.** Bu güncelleştirme, Sunucu Çekirdeği yükleme seçeneğinin kullanılmış olup olmadığına bakılmaksızın, Windows Server 2008 veya Windows Server 2008 R2'nin desteklenen sürümlerine aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) ve [Windows Server 2008 R2 için Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) adlı MSDN makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008 ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Sunucu Çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i veya Windows Server 2008 R2'yi belirtildiği üzere Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları bu işletim sistemlerinin desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx) ve [Windows Server 2008 R2 için Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ee391631(vs.85).aspx) adlı MSDN makalelerine bakın. Sunucu Çekirdeği yükleme seçeneği Windows Server 2008 ve Windows Server 2008 R2'nin belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS10-003**](http://go.microsoft.com/fwlink/?linkid=178812)
</td>
<td style="border:1px solid black;">
[**MS10-004**](http://go.microsoft.com/fwlink/?linkid=163639)
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
Microsoft Office XP
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=47553f45-fa10-40e5-8267-9d42ff560a62)  
(KB977896)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=cfc697b4-2ceb-4030-86c5-be9bc8bfd07c)  
(KB973143)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2291ae24-fa39-4ad8-a7d0-12726b68ad96)  
(KB976881)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="3">
Mac için Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS10-003**](http://go.microsoft.com/fwlink/?linkid=178812)
</td>
<td style="border:1px solid black;">
[**MS10-004**](http://go.microsoft.com/fwlink/?linkid=163639)
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
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=7c985595-00c5-44b8-81c3-59d9967220f8)<sup>[1]</sup>
(KB979674)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=7c985595-00c5-44b8-81c3-59d9967220f8)<sup>[1]</sup>
(KB979674)  
(Önemli)
</td>
</tr>
</table>
 
**Mac için Microsoft Office için Not**

<sup>[1]</sup>Mac için Microsoft Office 2004 toplu hizmet modeli nedeniyle bu güncelleştirmeler aynıdır.

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

-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Damian Frizza, MS10-003'te açıklanan sorunu bildirdiği için
-   [Secunia](http://secunia.com/) için çalışan Carsten Eiram, MS10-004'te açıklanan sorunu bildirdiği için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Sean Larsson, MS10-004'te açıklanan üç sorunu bildirdiği için
-   SkD, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-004'te açıklanan sorunu bildirdikleri için
-   [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) için çalışan Cody Pierce, MS10-004'te açıklanan sorunu bildirdiği için
-   ICST-ERCIS (Bilgi Güvenliği Araştırma Merkezi, Bilgisayar Bilimleri ve Teknolojisi Enstitüsü, Pekin Üniversitesi/Çin) için çalışan Tielei Wang, [Secunia](http://secunia.com/) ile birlikte çalışarak MS10-005'te açıklanan sorunu bildirdikleri için
-   [stratsec](http://www.stratsec.net/) için çalışan Laurent Gaffié, MS10-006'da açıklanan iki sorunu bildirdiği için
-   Brett Moore, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-007'de açıklanan sorunu bildirdikleri için
-   [Lostmon Lords](http://lostmon.blogspot.com/), MS10-007'de açıklanan sorunu bildirdiği için
-   [NGS Software](http://www.ngssoftware.com/) için çalışan Shaun Colley, MS10-008'de açıklanan sorunu bildirdiği için
-   [Google Security Team](http://www.google.com/) için çalışan Sumit Gwalani, Drew Hintz ve Neel Mehta, MS10-009'da açıklanan üç sorunu bildirdikleri için
-   Jan Bottorff, MS10-010'da açıklanan sorunu bildirdiği için
-   [Hispasec](http://www.hispasec.com/) için çalışan Matthew 'j00ru' Jurczyk ve Gynvael Coldwind, MS10-011'de açıklanan sorunu bildirdikleri için
-   [Codenomicon](http://www.codenomicon.com/) için çalışan Joshua Morin, MS10-012'de açıklanan sorunu bildirdiği için
-   [BSI](http://www.bsi.bund.de/) için çalışan Florian Rienhardt, MS10-012'de açıklanan sorunu bildirdiği için
-   Hernan Ochoa (Bağımsız Bilgi Güvenliği Danışmanı/Araştırmacısı), MS10-012'de açıklanan sorunu bildirdiği için
-   Anonim bir araştırmacı, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS10-013'te açıklanan sorunu bildirdikleri için
-   [Google Inc.](http://www.google.com/) için çalışan Tavis Ormandy, MS10-015'te açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (9 Şubat 2010): Bülten Özeti yayımlandı.
-   V1.1 (10 Şubat 2010): MS10-005 için yeniden başlatma gereksinimleri düzeltildi.

*Built at 2014-04-18T01:50:00Z-07:00*
