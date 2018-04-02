---
TOCTitle: 'MS09-JUN'
Title: Microsoft Güvenlik Bülteni Haziran 2009 Özeti
ms:assetid: 'ms09-jun'
ms:contentKeyID: 61235818
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms09-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Haziran 2009 Özeti
=============================================

Yayım Tarihi: 9 Haziran 2009 Salı

**Sürüm:** 1.0

Bu bülten özetinde Haziran 2009'da yayımlanan güvenlik bültenleri listelenir.

Haziran 2009 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 4 Haziran 2009'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 10 Haziran 2009 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Haziran Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395225). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;"><strong>Active Directory'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (971055)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows 2000 Server ve Windows Server 2003 üzerinde Active Directory ile Windows XP Professional ve Windows Server 2003 üzerinde Active Directory Uygulama Modu (ADAM) uygulamalarında özel olarak bildirilen iki güvenlik açığını giderir. Daha ciddi olan güvenlik açığı uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini uzaktan ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ yapılarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. En iyi uygulamalar, Internet'e bağlı sistemlerde olabildiğince az sayıda bağlantı noktasının açılmasını önerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;"><strong>Windows Yazdırma Biriktiricisi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (961501)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Yazdırma Biriktiricisi'ndeki özel olarak bildirilen üç güvenlik açığını giderir. En ciddi güvenlik açığı, etkilenen bir sunucu özel hazırlanmış bir RPC isteği alırsa uzaktan kod yürütülmesine olanak verebilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ yapılarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. En iyi uygulamalar, Internet'e bağlı sistemlerde olabildiğince az sayıda bağlantı noktasının açılmasını önerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen yedi ve genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açıklarından en önemlisi, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969514)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Word dosyasını açarsa uzaktan kod yürütülmesine izin verilebileceği özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıklarından birini başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı hatalı biçimlendirilmiş bir kayıt nesnesi içeren özel hazırlanmış bir Excel dosyasını açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen birkaç güvenlik açığını giderir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=128104">MS09-024</a></td>
<td style="border:1px solid black;"><strong>Microsoft Works Dönüştürücüleri'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957632)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Works dönüştürücülerindeki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Works dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, yerel kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150174">MS09-026</a></td>
<td style="border:1px solid black;"><strong>RPC'deki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (970238)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Windows uzaktan yordam çağrısı (RPC) hizmetinde RPC Düzenleme Altyapısı'nın iç durumunu düzgün şekilde güncelleştirmemesine neden olduğu genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, saldırganın rasgele kod yürütmesine ve etkilenen sistemin tüm denetimini ele geçirmesine olanak verebilir. Microsoft Windows'un desteklenen sürümleri, bu güvenlik açığından etkilenebilecek RPC sunucularıyla veya istemcileriyle birlikte gelmez. Varsayılan yapılandırmada, bu güvenlik açığından yararlanılarak kullanıcılara saldırılamaz. Ancak güvenlik açığı, Microsoft Windows RPC çalışma zamanında bulunmaktadır ve üçüncü taraf RPC uygulamalarını etkileyebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (968537)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Windows çekirdeğinde ayrıcalık yükselmesine izin verebileceği genel ve özel olarak bildirilen ikişer güvenlik açığını giderir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan rasgele kod yürütebilir ve etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Saldırganın bu güvenlik açıklarından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;"><strong>Internet Information Services'taki (IIS) Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (970483)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Internet Information Services'taki (IIS) genel olarak duyurulan ve özel olarak bildirilen birer güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı kimlik doğrulaması gerektiren bir Web sitesine özel hazırlanmış bir HTTP isteği gönderirse ayrıcalık yükselmesine izin verebilir. Bu güvenlik açıkları, saldırganın izin verilen kimlik doğrulamasını belirten IIS yapılandırmasını atlamasına izin verir; ancak bir dosyaya belirli bir kullanıcı tarafından erişime izin verilip verilmediğini doğrulayan dosya sistemi tabanlı erişim denetim listesi (ACL) denetimini atlamasına izin vermez. Saldırgan bu güvenlik açıklarından başarıyla yararlansa da, anonim kullanıcı hesabına dosya sistemi ACL'leri tarafından atanmış olan izinlerle kısıtlanmış olacaktır.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143550">MS09-023</a></td>
<td style="border:1px solid black;"><strong>Windows Search'teki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (963093)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Search'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı birinci sonuç olarak özel hazırlanmış bir dosyayı döndüren bir arama gerçekleştirirse veya arama sonuçlarındaki özel hazırlanmış bir dosyaya önizleme yaparsa bilginin açığa çıkmasına neden olabilir. Windows Search bileşeni varsayılan olarak Microsoft Windows XP ve Windows Server 2003'te önceden yüklenmiş değildir. İsteğe bağlı olarak karşıdan yüklenebilen bir bileşendir. Windows Vista'nın ve Windows Server 2008'in desteklenen sürümleri üzerine yüklendiğinde Windows Search bu güvenlik açığından etkilenmez.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Orta</a><br />
Bilginin Açığa Çıkması</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, bülten numarasına ve CVE numarasına göre listelenmektedir.
  
**Bu tabloyu nasıl kullanacağım?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
| Bülten Kimliği                                            | Bülten Başlığı                                                                                            | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                                                                                                                                                                                                                              |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Active Directory'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (971055)                 | [CVE-2009-1138](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1138) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Ağ üzerinden LDAP hizmetinin (varsayılan tcp/389) kullanıldığı Windows 2000 tabanlı sunucularda uzaktan kod yürütülmesi olasılığı bulunmaktadır.                                                                                                                           |  
| [MS09-018](http://go.microsoft.com/fwlink/?linkid=151361) | Active Directory'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (971055)                 | [CVE-2009-1139](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1139) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu açığın güvenlik etkisi, hizmet reddine yol açabilecek bir bellek sızıntısıdır. Kod yürütülmesi mümkün değildir.                                                                                                                                                         |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2007-3091](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2007-3091) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1140](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1140) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu, bilginin açığa çıkmasına olanak sağlayabilecek bir etki alanları arası bilgiye erişim güvenlik açığıdır; kod yürütülmesine olanak vermez.                                                                                                                              |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1141](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1141) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1528](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1528) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1529](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1529) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1530](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1530) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1531](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1531) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-019](http://go.microsoft.com/fwlink/?linkid=150860) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (969897)                                           | [CVE-2009-1532](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1532) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Internet Information Services'taki (IIS) Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (970483) | [CVE-2009-1122](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1122) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Kod yürütülmesi olasılığı düşüktür, ancak kimlik doğrulamasının atlanması koşulları nedeniyle bilginin açığa çıkması olasılığı yüksektir.                                                                                                                                  |  
| [MS09-020](http://go.microsoft.com/fwlink/?linkid=150568) | Internet Information Services'taki (IIS) Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (970483) | [CVE-2009-1535](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1535) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Bilginin açığa çıkması için genel kod kullanıma açıktır.                                                                                                                                                                                                                   |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0549](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0549) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0557](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0557) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0558](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0558) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0559](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0559) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Kod yürütülmesi tehdidi yalnızca Office 2000 için bulunmaktadır. Office'in sonraki sürümlerine yönelik saldırıların kod yürütülmesine neden olması olasılığı düşüktür.                                                                                                     |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0560](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0560) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-0561](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0561) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-021](http://go.microsoft.com/fwlink/?linkid=147294) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969462)           | [CVE-2009-1134](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1134) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Windows Yazdırma Biriktiricisi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (961501)  | [CVE-2009-0228](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0228) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Windows Yazdırma Biriktiricisi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (961501)  | [CVE-2009-0229](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0229) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu, bir bilginin açığa çıkması güvenlik açığıdır ve kod yürütülmesi olasılığı bulunmamaktadır.                                                                                                                                                                             |  
| [MS09-022](http://go.microsoft.com/fwlink/?linkid=141786) | Windows Yazdırma Biriktiricisi'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (961501)  | [CVE-2009-0230](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0230) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-023](http://go.microsoft.com/fwlink/?linkid=143550) | Windows Search'teki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (963093)                       | [CVE-2009-0239](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0239) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-024](http://go.microsoft.com/fwlink/?linkid=128104) | Microsoft Works Dönüştürücüleri'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957632)    | [CVE-2009-1533](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1533) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (968537)                   | [CVE-2009-1123](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1123) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (968537)                   | [CVE-2009-1124](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1124) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (968537)                   | [CVE-2009-1125](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1125) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-025](http://go.microsoft.com/fwlink/?linkid=150248) | Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (968537)                   | [CVE-2009-1126](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1126) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Windows 2000 için yararlanma kodu büyük olasılıkla tutarlıdır. Bu yığın tabanlı arabellek taşması nedeniyle kod yürütülmesi olasılığı, /GS koruması nedeniyle Windows XP ve Windows Server 2003'te düşüktür.                                                               |  
| [MS09-026](http://go.microsoft.com/fwlink/?linkid=150174) | RPC'deki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (970238)                                    | [CVE-2009-0568](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0568) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Bu güvenlik açığı herhangi bir Microsoft yazılımını etkilememektedir. Ancak bağımsız yazılım satıcıları tarafından geliştirilen RPC hizmetlerinin kullanıldığı iş istasyonlarında bu güvenlik güncelleştirmesi yüklü değilse uzaktan kod yürütülmesinden şüphelenilebilir. |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969514)            | [CVE-2009-0563](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0563) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                      |  
| [MS09-027](http://go.microsoft.com/fwlink/?linkid=147416) | Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (969514)            | [CVE-2009-0565](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0565) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                      |
  
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
</tr>
<tr>
<th colspan="8">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4 üzerinde Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=bba6e20a-0345-46ae-a6f1-fd27fdee7c21)  
(KB969805)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=86378753-db24-44c2-a27d-cc0239f40ab8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d645ad82-13c3-4030-808b-834e86ed3298)  
(Kritik)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fe8b3796-a407-4f41-89eb-35b4bcc24ff6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=155a79c1-e5e4-4f62-b4b0-53aca59f20ac)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=79b0481d-a3d7-477b-928a-a98cc79374af)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=8515a294-4f25-4dc5-860a-e7ad9b6c1c01)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="8">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[Windows XP Professional Service Pack 2 ve Windows XP Professional Service Pack 3 üzerinde Active Directory Uygulama Modu (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=cb2c9b76-0c65-4754-9941-d45a7c74a29a)  
(KB970437)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f2119aca-a98e-4810-be52-f38241443baf)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=3d7f63ee-d7c3-48a5-902e-60625405e97d)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=827b735c-660b-4723-b688-3297e107153a)  
(Kritik)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d9e27ce1-4e7c-437f-9477-e7805a33da08)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f033fa78-c451-44f8-aa6c-a49622c37f40)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6349e046-a3f8-4ae5-b8c3-c9879cc99e8f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional Service Pack 2 ve Windows XP Professional Service Pack 3 üzerinde Microsoft Internet Information Services 5.1](http://www.microsoft.com/downloads/details.aspx?familyid=97da589f-4534-42f6-9f29-967b5a33c542)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=759f22cb-ea7f-49dd-a200-19cb83fffd8d)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory Uygulama Modu (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=2ef3aaf0-a2a9-4c17-99ab-a0dc3d3f7e86)  
(KB970437)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22699d09-1e68-456a-8733-bfad6667ebf5)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=088f70eb-c5c5-426a-880a-18ed386d0b56)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e5d2c81e-ffab-4e3b-a59a-a55000597213)  
(Kritik)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=a24aedf0-7a31-4ee8-a9a6-998f1160c700)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=20734b70-37f1-47dd-bc09-d56f93577a55)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3769800e-af93-4a44-8a1e-b30cc54b226f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=8982e6d2-e1f7-4208-88e3-80b159a8e21a)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=50c56dd6-c34d-4632-a779-8bcf8fdb341b)  
(Orta)
</td>
</tr>
<tr>
<th colspan="8">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
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
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=d814ce65-a193-4027-a6cd-106d388830a6)   
(KB969805)  
(Önemli)  
[Active Directory Uygulama Modu (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=f6f99957-f74f-4446-8734-a468283eebae)   
(KB970437)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=865414f8-3f77-4fee-acc6-6684a3dc0aa4)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=72a23752-86fb-4cc9-ab8e-63ffdfae5bec)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a980b867-c67f-4c61-b6db-e55c2ca68dc0)  
(Orta)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=298143f2-f37a-4a2c-86ac-9804d4ff1dad)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=62bb9e22-4f4b-4ffc-ba76-f626e94c79d5)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9356404c-d89a-4de0-b9b4-f6e1bdadf745)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=2bd4e410-dbd8-431a-b316-e1e2f1825c3a)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=e72ef31f-5161-4fe6-8ed3-6206e02cef31)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=0d1f23c8-06eb-4996-92eb-0eb635fd6a42)  
(KB969805)  
(Önemli)  
[Active Directory Uygulama Modu (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=1a2badc7-c0a5-4032-a009-73ebe9d76313)  
(KB970437)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=197a6cc7-4ba3-4d2e-b621-0ef3da645ef2)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=2a03d3c4-e39d-43a3-8d42-216e9551be96)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5e7d6372-9c8c-449d-88fd-afd4f92ad9e6)  
(Orta)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4a5401d7-ca97-4734-a0e9-d7ffe0777e34)  
(Orta)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=888b8dd8-d76c-42f5-a377-1f1750d3cf56)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5a3123af-173d-49eb-9997-14e82e764aee)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=ea363223-535d-4142-9aba-3890960c6259)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Search 4.0](http://www.microsoft.com/downloads/details.aspx?familyid=7ffc3680-f9bf-423b-96a7-102f4cc9c240)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=92e7808b-92ff-449d-bb73-ee8638e9ccd1)  
(KB969805)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=719efd62-fb33-447d-b6dd-2aaafbbad881)  
(Orta)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=58efde2c-e0b8-4259-b19e-80564b834882)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a2d2907e-67ae-44a4-a805-8670e659ea57)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=3084f46e-02b9-4d99-a7a1-033817f9bd9f)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=13b50993-410f-4e7a-a33a-6d9b48dbb4d1)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](http://www.microsoft.com/downloads/details.aspx?familyid=e6b806eb-e2c4-4436-8964-720db593055d)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="8">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ad8f037-2434-4dea-bfc3-9d3b4008b828)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e60215c3-b8b9-4e45-9d9f-b3fb0b47cce1)  
(Kritik)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=6f2730e9-b4fc-4f20-96cf-73f1be63f374)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5ca227c0-f2dd-429c-a542-e08e93527214)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 ve Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c31b36f8-330c-4a0c-9a3d-7cbe9a1ab8c8)  
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
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=85c317cd-2a14-4747-9f50-3af3ddd3ae1b)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=88185088-8c2c-4bc6-89b2-87f4d4849cf7)  
(Kritik)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=5edb14f7-11ec-4180-9f0f-b2673f1c8d83)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=188adafe-1feb-46ad-b237-a88d35104dcd)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 ve Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d70a65f-07ce-4992-8bec-28fefd7587bc)  
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
<th colspan="8">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-018**](http://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](http://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](http://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](http://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](http://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](http://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](http://go.microsoft.com/fwlink/?linkid=143550)
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
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0f18356d-9f09-4d24-8361-970c0d1ccac4)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=a0e3f975-57da-43fa-ac12-3d14fd6ce939)\*\*  
(Orta)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=aaad301c-d232-4733-a0df-8e5d41bbfde8)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=eaa26c6c-5bf7-4099-bb21-1e03de3a25ca)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 ve 32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98ba52b2-da1a-4939-a10e-d43b3a7e7ed4)\*  
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
x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7d0a6e8d-a31d-4f3d-a7d7-e61215bfebed)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=758edce7-2a82-4b2e-bd71-5b7075cc4b17)\*\*  
(Orta)  
[Windows Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=faac92d4-4a2b-4bb5-8bd1-1519a9fa8147)\*\*  
(Orta)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=447aaa4f-946b-4f23-b151-dcf46ea9f80e)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 ve x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbaa5a72-c267-4907-a207-525c2803d7b9)\*  
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
Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bbac3deb-6c93-45aa-832c-02b915ac7f44)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=67d4c189-030d-42eb-98b9-7957ccd92592)  
(Orta)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f33012b9-5d5b-4f72-8d49-a8e1c8bc1337)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 ve Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0e3ad56-a363-44ba-af4d-b7f551c88afd)  
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
 
**Windows Server 2008 için Notlar**

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

#### Microsoft Office Paketleri ve Yazılımları

 
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
</tr>
<tr>
<th colspan="4">
Microsoft Office Paketleri, Sistemleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3663e9f2-a952-4238-b902-90b5b09feb38)  
(KB969600)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd16e243-b8e2-4afb-86b6-4d60214598eb)  
(KB969683)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4bf95806-3d32-411b-9779-a81aebad45e9)  
(KB957838)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f1323be1-15f2-491b-abae-c03ba1394398)  
(KB969602)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=dd80ce95-0aec-4493-b9d1-c3dad95c3415)  
(KB969680)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0ba8c9e-75ee-46bd-9e92-d4e6599309ad)  
(KB957646)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7cbc2587-2c8c-49b4-9f40-e4cdccb61ecd)  
(KB969603)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=10156044-a5a4-4312-98a7-1b1ced625ddb)  
(KB969681)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Works 6–9 Dosya Dönüştürücüsü yüklü olarak Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a7ba3ea7-d06a-4c14-9107-9b92ef68fcae)\*\*\*  
(KB968326)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi Service Pack 1 ve 2007 Microsoft Office Sistemi Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1 ve Microsoft Office Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7e205108-4c28-4cab-a4d0-4ed3fd696473)  
(KB969604)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 ve Microsoft Office Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2bcd565a-6acb-407d-80da-0398526ddf99)\*  
(KB969682)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=bd47e1e5-cd2e-4c08-9864-471e97f38ca3)  
(KB969559)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="4">
Mac için Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2008
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
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
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="4">
Diğer Office Yazılımları
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-027**](http://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](http://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](http://go.microsoft.com/fwlink/?linkid=128104)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=20e6933d-85f8-4cec-9534-893789cd053e)  
(KB969685)  
(Önemli)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=ac0530dc-7f63-4ad0-85c1-784ad28156cf)  
(KB969686)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Önemli)  
[Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
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
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1 ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63bd8f14-e736-46ce-af66-d30f17461e5a)  
(KB969613)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1 ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2)  
(KB969679)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](http://www.microsoft.com/downloads/details.aspx?familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](http://www.microsoft.com/downloads/details.aspx?familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 ve Microsoft Office SharePoint Server 2007 Service Pack 2 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=862e6ad1-8124-4060-93b1-2b882ef5ce3d)\*\*  
(KB969737)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 ve Microsoft Office SharePoint Server 2007 Service Pack 2 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=b7b6e611-2c5d-4639-add9-972055789ecd)\*\*  
(KB969737)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**MS09-021 için Notlar**

\*Microsoft Office Excel 2007 Service Pack 1 ve Microsoft Office Excel 2007 Service Pack 2 için, müşterilerin bu bültende açıklanan güvenlik açıklarına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB969682'nin yanı sıra [Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1 ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2) (KB969679) güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

\*\*Bu güncelleştirme Microsoft Office SharePoint Server 2007 Enterprise sürümünün varsayılan yapılandırması ve Internet Siteleri için Microsoft Office SharePoint Server 2007 gibi Excel Hizmetleri'nin yüklü olduğu sunuculara uygulanır. Microsoft Office SharePoint Server 2007 Standard sürümü Excel Hizmetleri'ni içermemektedir.

**MS09-024 için Not**

\*\*\*Güvenlik açığından etkilenen bir Works dönüştürücüsü yüklüyse Microsoft Office Word 2003 bu sorundan etkilenir. Microsoft Office Word 2003 için Works dönüştürücüleri karşıdan yükleme olarak [Microsoft Works 6–9 Dosya Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=bf41401e-70fa-465d-ae2e-cf44dbf05297&displaylang=tr) sitesinden edinilebilir.

Algılama ve Dağıtım Araçları ve Kılavuzu
----------------------------------------

<span></span>
**Güvenlik Merkezi**

Kuruluşunuzdaki sunuculara, masaüstü bilgisayarlara ve taşınabilir bilgisayarlara dağıtmanız gereken yazılımları ve güvenlik güncelleştirmelerini yönetin. Daha fazla bilgi için, bkz: [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171), Microsoft ürünlerinde güvenlik konusunda ek bilgi sağlar. Müşteriler, bu bilgilerin "En Son Güvenlik Güncelleştirmeleri" tıklatılarak da edinilebileceği [Evde Güvenlik](http://go.microsoft.com/fwlink/?linkid=85102) sitesini de ziyaret edebilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) ve [Office Update](http://go.microsoft.com/fwlink/?linkid=21135) sitesinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.

Son olarak, güvenlik güncelleştirmeleri [Microsoft Update Kataloğu](http://go.microsoft.com/fwlink/?linkid=96155)'ndan karşıdan yüklenebilir. Microsoft Update Kataloğu, Windows Update ve Microsoft Update aracılığıyla sunulan güvenlik güncelleştirmeleri, sürücüler ve hizmet paketleri gibi içeriğin arama yapılabilen bir kataloğunu sunar. Güvenlik bülteni numarasını kullanarak arama yaptığınızda (“MS07-036” gibi), uygulanabilen tüm güncelleştirmeleri sepete ekleyebilir (bir güncelleştirmenin farklı dilleri de dahil) ve istediğiniz klasöre karşıdan yükleyebilirsiniz. Microsoft Update Kataloğu hakkında daha fazla bilgi için, bkz: [Microsoft Update Kataloğu Hakkında SSS](http://go.microsoft.com/fwlink/?linkid=97900).

**Algılama ve Dağıtım Kılavuzu**

Microsoft bu ayın güvenlik güncelleştirmeleri için algılama ve dağıtım kılavuzu sağlamıştır. Bu kılavuz, ayrıca BT uzmanlarının güvenlik güncelleştirmesini dağıtmak amacıyla Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Algılama Aracı, Microsoft Systems Management Server (SMS) ve Genişletilmiş Güvenlik Güncelleştirmesi Envanter Aracı (ESUIT) gibi çeşitli araçları nasıl kullanabileceklerini anlamalarına yardımcı olur. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Microsoft Baseline Security Analyzer (MBSA), yöneticilerin eksik güvenlik güncelleştirmeleri ve ayrıca sık rastlanan güvenlik yapılandırması hataları için yerel ve uzak sistemleri taramasına olanak sağlar. MBSA hakkında daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

**Windows Server Update Services**

Windows Server Update Services'ı (WSUS) kullanarak, yöneticiler en son kritik güncelleştirmeleri ve güvenlik güncelleştirmelerini Windows 2000 işletim sistemlerine ve sonrasına, Office XP'ye ve sonrasına, Exchange Server 2003'e, SQL Server 2000'e, Windows 2000 ve sonraki işletim sistemi sürümlerine hızla ve güvenle dağıtabilir.

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) Web sitesini ziyaret edin.

**Systems Management Server**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; ayrıca bkz. [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Yöneticilerin güvenlik güncelleştirmelerini dağıtmak için SMS 2003'ü nasıl kullanacakları hakkında daha fazla bilgi için, bkz. [SMS 2003 Güvenlik Düzeltme Eki Yönetimi](http://go.microsoft.com/fwlink/?linkid=22939). SMS 2.0 kullanıcıları, güvenlik güncelleştirmelerinin dağıtılmasına yardımcı olması için [Software Update Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340)'i de kullanabilir. SMS hakkında daha fazla bilgi için, [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) Web sitesini ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı ve Microsoft Office Algılama Aracı'nı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler, bu güncelleştirmeleri yüklemek için Elevated Rights Deployment Tool'u kullanabilir ([SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) ve [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) içinde bulunur).

**Güncelleştirme Uyumluluğu Değerlendiricisi ve Uygulama Uyumluluğu Araç Takımı**

Güncelleştirmeler genelde uygulamalarınızın çalışması için gerekli olan aynı dosyalara ve kayıt defteri ayarlarına yazar. Bu durum da uyumsuzlukları tetikleyebilir ve güvenlik güncelleştirmelerinin dağıtılması için gereken zamanı artırabilir. [Uygulama Uyumluluğu Araç Takımı 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) ile birlikte gelen [Güncelleştirme Uyumluluğu Değerlendiricisi](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) bileşenlerini kullanarak, Windows güncelleştirmelerinin yüklü uygulamalara göre sınanması ve doğrulanması sürecini hızlandırabilirsiniz.

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Microsoft Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Yüksek Öncelikli Güncelleştirmeler

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): Yazılım Güncelleştirme Hizmetleri ve Windows Server Güncelleştirme Hizmetleri'nin tanımı içeriğe bağlı olarak değişir. Tüm Windows içeriğini içerir.
-   [Microsoft Windows Dışındaki Microsoft Ürünleri için Yeni, Yeniden Düzenlenen ve Yayımlanan Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

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

-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Joshua J. Drake, MS09-018'de açıklanan sorunu bildirdiği için
-   [Beaverton School District](http://www.beaverton.k12.or.us/home/) için çalışan Justin Wyatt, MS09-018'de açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan David Bloom, MS09-019'da açıklanan sorun konusunda bizimle çalıştığı için
-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Jorge Luis Alvarez Medina, MS09-019'da açıklanan sorunu bildirdiği için
-   [Fortinet](http://www.fortinet.com/) için çalışan Haifei Li, MS09-019'da açıklanan sorunu bildirdiği için
-   [Tippingpoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS09-019'da açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) için çalışan Peter Vreugdenhil ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS09-019'da açıklanan sorunu bildirdikleri için
-   Wushi, [Tippingpoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS09-019'da açıklanan iki sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) için çalışan Nils ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS09-019'da açıklanan sorunu bildirdikleri için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, MS09-020'de açıklanan sorunu bildirdiği için
-   Fortinet bünyesindeki [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) için çalışan Bing Liu, MS09-021'de açıklanan üç sorunu bildirdiği için
-   [Secunia](http://secunia.com/) için çalışan Carsten H. Eiram, MS09-021'de açıklanan iki sorunu bildirdiği için
-   [TELUS Security Labs Vulnerability Research Team](http://telussecuritylabs.com/), MS09-021'de açıklanan sorunu bildirdikleri için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Sean Larsson ve Joshua Drake, MS09-021'de açıklanan sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS09-021'de açıklanan sorunu bildirdikleri için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Jun Mao, MS09-022'de açıklanan sorunu bildirdiği için
-   [IBM Rational Application Security](http://blog.watchfire.com/) için çalışan Yair Amit, MS09-023'te açıklanan sorunu bildirdiği için
-   [NGS Software](http://www.ngssoftware.com/) için çalışan Shaun Colley, MS09-024'te açıklanan sorunu bildirdiği için
-   Thomas Garnier, MS09-025'te açıklanan iki sorunu bildirdiği için
-   [team509](http://www.team509.com/) için çalışan Wushi, [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS09-027'de açıklanan sorunu bildirdikleri için
-   [VUPEN Security](http://www.vupen.com/) için çalışan Nicolas Joly, MS09-027'de açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (9 Haziran 2009): Bülten Özeti yayımlandı.

*Built at 2014-04-18T01:50:00Z-07:00*
