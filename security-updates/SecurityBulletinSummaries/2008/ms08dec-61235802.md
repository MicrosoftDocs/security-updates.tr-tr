---
TOCTitle: 'MS08-DEC'
Title: Microsoft Güvenlik Bülteni Aralık 2008 Özeti
ms:assetid: 'ms08-dec'
ms:contentKeyID: 61235802
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Aralık 2008 Özeti
============================================

Yayım Tarihi: 9 Aralık 2008 Salı | Güncelleştirme Tarihi: 29 Nisan 2009 Çarşamba

**Sürüm:** 6.0

Bu bülten özetinde Aralık 2008'de yayımlanan güvenlik bültenleri listelenir.

Aralık 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 4 Aralık 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 10 Aralık 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirmektedir. [Aralık Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374647). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Bu bülten özetinin Sürüm 3.0'ına eklenen bant dışı güvenlik bülteni (MS08-078) için, Microsoft bu bültenlerle ilgili müşteri sorularını yanıtlamak üzere iki web yayını sağlamaktadır: 17 Aralık 2008 saat 13:00 Pasifik Saati (ABD ve Kanada) ve 18 Aralık 2008 saat 11:00 Pasifik Saati. [17 Aralık web yayını](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032399448&culture=en-us) ve [18 Aralık web yayını](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032399449&culture=en-us) için şimdi kaydolun. Daha sonra bu web yayınları istek üzerine alınabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;"><strong>GDI'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956802)</strong><br />
<br />
Bu güvenlik güncelleştirmesi GDI'daki özel olarak bildirilen iki güvenlik açığını giderir. Bir kullanıcı özel hazırlanmış bir WMF resim dosyasını açarsa, bu güvenlik açıklarından birinden yararlanılması, uzaktan kod yürütülmesine olanak verebilir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;"><strong>Windows Arama'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959349)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows Arama'daki özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir kayıtlı arama dosyasını Windows Gezgini içinden açıp kaydederse veya özel hazırlanmış bir arama URL'sini tıklatırsa uzaktan kod yürütülmesine izin verebilir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer için Toplu Güvenlik Güncelleştirmesi (958215)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, özel olarak bildirilen dört güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=137335">MS08-078</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer için Güvenlik Güncelleştirmesi (960714)</strong><br />
<br />
Bu güvenlik güncelleştirmesi genel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;"><strong>Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları için ActiveX denetimlerindeki özel olarak bildirilen beş ve genel olarak duyurulan bir güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış içeriğe sahip bir Web sitesine gözatarsa uzaktan kod yürütülmesine izin verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Geliştirici Araçları ve Yazılımları, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Office Word ve Microsoft Office Outlook'ta bir kullanıcı özel hazırlanmış bir Word veya Zengin Metin Biçimi (RTF) dosyasını açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen sekiz güvenlik açığını giderir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959070)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Excel dosyasını Microsoft Office Excel'de açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen üç güvenlik açığını giderir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126307">MS08-077</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office SharePoint Server'daki Güvenlik Açığı Ayrıcalık Yükselmesine Neden Olabilir (957175)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan SharePoint sitesindeki bir yönetimsel URL'ye gözatarak kimlik doğrulamasını atlarsa ayrıcalık yükselmesine izin verebilir. Ayrıcalık yükselmesiyle sonuçlanan başarılı bir saldırı, hizmet reddine veya bilginin açığa çıkmasına neden olabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Server Yazılımı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;"><strong>Windows Media Bileşenlerindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959807)</strong><br />
<br />
Bu güvenlik güncelleştirmesi şu Windows Media bileşenlerindeki özel olarak bildirilen iki güvenlik açığını giderir: Windows Media Player, Windows Media Format Çalışma Zamanı Modülü ve Windows Media Hizmetleri. En ciddi güvenlik açığı uzaktan kod yürütülmesine olanak verebilir. Kullanıcı yönetimsel haklarla oturum açtıysa, bu güvenlik açığından başarıyla yararlanan bir saldırgan etkilenen sistemin denetimini tümüyle ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
**Bu tabloyu nasıl kullanacağım?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Bülten Başlığı</th>
<th style="border:1px solid black;" >CVE Kimliği</th>
<th style="border:1px solid black;" >Yararlanma Dizini Değerlendirmesi</th>
<th style="border:1px solid black;" >Önemli Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3704">CVE-2008-3704</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Tutarlı yararlanma kodu genel kullanıma açıktır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4252">CVE-2008-4252</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4256">CVE-2008-4256</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4253">CVE-2008-4253</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4254">CVE-2008-4254</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları'ndaki (ActiveX Denetimleri) Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4255">CVE-2008-4255</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">Windows 2000 çalışan sistemler en fazla risk altındadır. Windows XP SP2, Windows Server 2003 SP1 ve sonraki işletim sistemlerinin daha güçlü öbek koruması nedeniyle işlevsel yararlanma kodundan etkilenme olasılıkları düşüktür.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;">GDI'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956802)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3465">CVE-2008-3465</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;">GDI'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956802)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2249">CVE-2008-2249</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4024">CVE-2008-4024</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4025">CVE-2008-4025</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4026">CVE-2008-4026</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4027">CVE-2008-4027</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4028">CVE-2008-4028</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4030">CVE-2008-4030</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4837">CVE-2008-4837</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Microsoft Office Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4031">CVE-2008-4031</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - İşlevsel bir yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Internet Explorer için Toplu Güvenlik Güncelleştirmesi (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4258">CVE-2008-4258</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Internet Explorer için Toplu Güvenlik Güncelleştirmesi (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4259">CVE-2008-4259</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Internet Explorer için Toplu Güvenlik Güncelleştirmesi (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4261">CVE-2008-4261</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Internet Explorer için Toplu Güvenlik Güncelleştirmesi (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4260">CVE-2008-4260</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4265">CVE-2008-4265</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4266">CVE-2008-4266</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4264">CVE-2008-4264</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;">Windows Arama'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4269">CVE-2008-4269</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;">Windows Arama'daki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4268">CVE-2008-4268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> - Yararlanma kodu büyük olasılıkla tutarsız</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;">Windows Media Bileşenlerindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959807)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3009">CVE-2008-3009</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Bu sorun için tutarlı yararlanma kodu oluşturulabilir. Ancak saldırı senaryolarının sınırlı yapısı, asıl saldırıların gerçekleşme olasılığının düşük olduğu anlamına gelir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;">Windows Media Bileşenlerindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (959807)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3010">CVE-2008-3010</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Bu sorun için tutarlı yararlanma kodu oluşturulabilir. Ancak saldırı senaryolarının sınırlı yapısı, asıl saldırıların gerçekleşme olasılığının düşük olduğu anlamına gelir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126307">MS08-077</a></td>
<td style="border:1px solid black;">Microsoft Office SharePoint Server'daki Güvenlik Açığı Ayrıcalık Yükselmesine Neden Olabilir (957175)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4032">CVE-2008-4032</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı</td>
<td style="border:1px solid black;">Bu sorun için tutarlı yararlanma kodu oluşturulabilir. Ancak bu güvenlik açığından yararlanılan saldırılar büyük olasılıkla uzaktan kod yürütülmesine değil, yalnızca bilginin açığa çıkmasına neden olacaktır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=137335">MS08-078</a></td>
<td style="border:1px solid black;">Internet Explorer için Güvenlik Güncelleştirmesi (960714)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4844">CVE-2008-4844</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Yararlanma kodu büyük olasılıkla tutarlı<br />
(Bülten yayımlandığında genel olarak biliniyordu)</td>
<td style="border:1px solid black;">Etkin saldırılarda tutarlı yararlanma kodu bulunmuştur. Ancak, varsayılan Windows Vista ve Windows Server 2008 yüklemelerinde Internet Explorer Korumalı Mod'da çalıştığından yararlanma engellenmektedir.</td>
</tr>
</tbody>
</table>
  
Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları  
--------------------------------------------------
  
<span></span>
**Bu tabloyu nasıl kullanacağım?**  
  
Bu tabloyu, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip gereken güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.
  
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
</tr>
<tr>
<th colspan="6">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=3b775fb1-1077-455d-af4a-4ccb5237974f)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=c242ba42-556b-4c87-bf33-9d99166ff096)  
(Kritik)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c0583745-7e57-4265-9429-c3415cb8465f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d3e18732-47f1-40ce-999c-d1fd283bf138)  
(Kritik)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=124c14b6-9323-4f6f-902b-727aa56444bc)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=c33d558e-45f9-4e85-b48c-03bd0e8cb4bc)  
(KB954600)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 7.1 ve Windows Media Format Çalışma Zamanı Modülü 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=6a459497-0ab8-41cb-87d0-b551631d8d8a)  
(KB952069)  
(Önemli)  
[Windows Media Hizmetleri 4.1](http://www.microsoft.com/downloads/details.aspx?familyid=58b7d241-cef6-48fa-aa52-017695f71db1)  
(KB952068)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="6">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2151fbba-c464-4d1e-82d4-5b096e82bed0)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=af9a6cb0-725d-490c-9858-16ec40e98560)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1b582695-b3cc-4c65-bc4b-d673c9a6d82a)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1d83e0af-46fa-4bfc-ba57-635435a7ef2d)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0190a289-164e-41a7-8c01-fa1aaed3f531)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=99241309-e644-4088-a8f3-38837fab4037)  
(KB954600)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.0, Windows Media Format Çalışma Zamanı Modülü 9.5 ve Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=504f816c-f554-4b93-ac28-b085574d9bac)  
(Yalnızca Windows XP Service Pack 2)  
(KB952069)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.0, Windows Media Format Çalışma Zamanı Modülü 9.5 ve Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=ad76fcf3-a2f9-4e36-bd1b-c1536749173c)  
(Yalnızca Windows XP Service Pack 3)  
(KB952069)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2247f6a5-aa33-4c68-9ea8-a63488d126d3)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=60bf9851-24fe-4658-8333-d353e82063c7)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=107cf54b-29d4-4c54-b091-2b5b3ffbf49d)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a585cb73-2c1a-4fa8-862a-ad6aeaeaf2f8)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9ba71e23-8cef-4399-b215-983b0dcf5cb5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=946d47c9-b208-4fab-8ef6-774413d61bc8)  
(KB954600)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=644ef023-ee40-45b0-9c9d-c76d9fab0005)  
(KB952069)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ae9e8b07-5354-42f3-a226-ba2193244524)  
(KB952069)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=2dadc017-2be5-4240-ab8f-0291756dca6b)  
(KB952069)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c396796-0929-4cd2-99e8-3c0f7075a89e)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d53adf6f-9501-4862-a1ca-57eb4d40cd75)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9cdd4f9e-c578-405c-af9e-628f2d77fdf4)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d81e9cf9-ce0c-463a-a359-49a348cb89ae)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=388847ec-817e-45cf-8fa7-32c7e1f57f80)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=2315ce20-2f46-42c2-bb40-045f003409d7)  
(KB954600)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=d8958248-c889-499e-a6a9-3b394cdb27ea)  
(KB952069)  
(Önemli)  
[Windows Media Hizmetleri 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=e71abc2d-d60e-444a-9b7b-062c5805fe9e)  
(KB952068)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6d5c7d2f-1a82-4cdf-b3f2-b2c2390c6a64)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=5e37cb34-32be-4bbe-87f3-c4e1974e4d00)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7c36f92c-d8a0-4b70-b85f-83588a0299a0)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=015df302-d79f-43a1-b5c5-32ac04de0510)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2ae17caf-6204-470e-8480-380d3d505657)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=4c29bed9-1b88-4d2f-80a5-305c2bedd89f)  
(KB954600)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=2278022e-a716-46c0-bedf-d626933bd815)  
(KB952069)  
(Önemli)  
[Windows Media Format Çalışma Zamanı Modülü 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ae9e8b07-5354-42f3-a226-ba2193244524)  
(KB952069)  
(Önemli)  
[Windows Media Hizmetleri 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=e0030155-1a9a-46cc-bbc8-6d0d1ed65c1f)  
(KB952068)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=1edb62b4-3d0f-4891-b4b3-8f8bc4e7bdfe)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=0da4e424-4682-4401-a226-7d8f1be19d44)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3811030d-5958-4b91-b5b8-20587dc7c4d6)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=18016305-7f72-47f6-ab4c-94282289bf5f)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=97d6c093-f68d-4ddf-8e3c-f29662a1940f)  
(Kritik)
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
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cddf9cf6-bdeb-4429-823a-879387a428d7)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0dcc5373-0435-42d5-864d-298e5bb122d9)  
(KB958623)  
(Önemli)  
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5b1b65f0-6848-47c6-bdd5-be3c0621b323)  
(KB958624)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=3f62030a-9ce2-4c92-b948-143a6881921e)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7887111d-4fac-4823-bdd2-a18d9468fdf0)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=1fcdc8dd-26d9-4d1a-8b3f-7b6a21a95999)  
(KB952069)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=73dc3775-b6f0-40f1-bd36-6b5fb80eb2fa)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2112c5c8-7c9f-4491-b127-b1093085e105)  
(KB958623)  
(Önemli)  
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=eb1d0ffe-1644-457b-9e82-768bd4c7f7ab)  
(KB958624)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d8800493-fba4-41f8-bde5-a53eeaf89d54)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=69979d92-8d45-47fe-ac4c-c2f1f23cf1fb)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=8839f6cd-dfbf-448c-bf1e-1da9bb5f3f25)  
(KB952069)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="6">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-Bit Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=bbed9e8b-e75e-44ef-ba1d-fd6f852c1f67)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=90ab7e6f-5ae7-4f55-8838-868fc98d8a16)\*\*\*  
(KB958623)  
(Önemli)  
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=470d506f-77ae-4a44-8598-df645f484295)\*\*\*  
(KB958624)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=45a0de3c-c7d1-4314-a456-1f7428b7c90a)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5552e564-dd1c-4e2a-9a42-6317522c884d)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=91ec4195-bc1c-444e-a7b0-ebde46c088fa)  
(KB952069)  
(Önemli)  
[Windows Media Hizmetleri 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ffb5d945-7f98-4849-b020-ed4873fa42df)\*  
(KB952068)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 Service Pack 2
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
[Windows Media Hizmetleri 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ffb5d945-7f98-4849-b020-ed4873fa42df)\*  
(KB952068)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=48aecf4c-1296-490d-ba37-a28e3ec19bd6)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=e1deab57-ada2-4b12-9157-5615e7b0071d)\*\*\*  
(KB958623)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=e41f23e4-6a2f-4ebb-b425-d241a08da316)\*\*\*  
(KB958624)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=405b28db-47d7-4d6b-90e6-834c0a409323)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=889c6eb1-7d1f-4e60-b637-535cb6e4e443)\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Format Çalışma Zamanı Modülü 11](http://www.microsoft.com/downloads/details.aspx?familyid=8cab6fe8-161d-4d8c-9772-eb3174a2c3c3)  
(KB952069)  
(Önemli)  
[Windows Media Hizmetleri 2008](http://www.microsoft.com/downloads/details.aspx?familyid=0204a366-5641-4036-9cb0-a46d04af9d72)\*  
(KB952068)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
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
[Windows Media Hizmetleri 2008](http://www.microsoft.com/downloads/details.aspx?familyid=0204a366-5641-4036-9cb0-a46d04af9d72)\*  
(KB952068)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=9bfe15cd-02ff-45cf-85c8-5ff1e6c1a871)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=48bed90d-c243-4969-8e54-326d9a7af343)  
(KB958623)  
(Önemli)  
[Itanium Tabanlı Sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=83de2263-de2a-4c13-96ba-ecfebdaf0bb9)  
(KB958624)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f0d4f321-941e-4da7-958f-582c75542ee8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=06cb502a-6818-4599-aa24-6eddb83e4b84)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**MS08-078 için Not**

MS08-08 tarafından giderilen güvenlik açığı Windows Internet Explorer 8 Beta 2'nin yayımlanmasından sonra bildirilmiştir. Windows Internet Explorer 8 Beta 2 çalıştıran müşterilerin güncelleştirmeyi karşıdan yükleyip sistemlerine uygulamaları önerilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) ve [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) sitelerinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.

**Windows Server 2008 için Notlar**

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008 çalışan bir sistem Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmişse, sistemde bu güvenlik açıklarından etkilenen dosyalar olsa da, bu güncelleştirmelerle giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Ancak, güncelleştirilmiş dosyalar sisteminizde bulunan dosyalardan daha yeni oldukları (sürüm numaraları daha büyük olduğu) için, etkilenen dosyaların bulunduğu kullanıcılara bu güncelleştirme yine de önerilir. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="5">
Microsoft Office Paketleri, Sistemleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=43e8c4d8-307b-48f6-ac99-a9617421d40a)  
(KB956328)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f39d2a49-f861-4f2d-bf91-94a8a85af40c)  
(KB958435)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3ef41412-50b3-4077-b0e3-9a3704d2f876)  
(KB956329)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=72076e21-2aa3-48e8-883a-c3cb756fc72a)  
(KB958372)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=45c81c60-4b1b-4246-839b-198ebc4eeae2)  
(KB956357)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6c0771e5-fcd4-4365-b903-1a3bd95d9e66)  
(KB958436)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007](http://www.microsoft.com/downloads/details.aspx?familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Önemli)  
[Microsoft Office Outlook 2007](http://www.microsoft.com/downloads/details.aspx?familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=68bb8d99-f28b-4efd-9314-3eee0bb00ccf)  
(KB958437)\*\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Önemli)  
[Microsoft Office Outlook 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=68bb8d99-f28b-4efd-9314-3eee0bb00ccf)  
(KB958437)\*\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office FrontPage
</td>
<td style="border:1px solid black;">
[Microsoft Office FrontPage 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0a6130ae-c5b4-43cb-afe3-ab6a55b9d9ea)\*  
(KB957797)  
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=89a44042-a629-40f3-800a-0bb45fc36591)  
(KB949045)  
(Kritik)  
[Microsoft Office Project 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2fbf6a5b-ff35-4a2d-9fa0-4e62b6486fe6)  
(KB949046)  
(Kritik)  
[Microsoft Office Project 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2fbf6a5b-ff35-4a2d-9fa0-4e62b6486fe6)  
(KB949046)  
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
</tr>
<tr>
<th colspan="5">
Mac için Microsoft Office
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=eca13ad8-62ae-41a8-b308-41e2d1773820)\*\*  
(KB960402)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=eca13ad8-62ae-41a8-b308-41e2d1773820)\*\*  
(KB960402)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ab31a564-43d2-45bd-98bf-19e9ca477b62)\*\*  
(KB960401)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ab31a564-43d2-45bd-98bf-19e9ca477b62)\*\*  
(KB960401)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=edb6cd8f-832c-4123-8982-ac0c601ea0a7)\*\*  
(KB960403)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=edb6cd8f-832c-4123-8982-ac0c601ea0a7)\*\*  
(KB960403)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="5">
Diğer Office Yazılımları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=1537d181-90d9-4bb5-b5ae-8d9990a349af)\*\*\*  
(KB959487)  
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
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=4b3989ef-02b8-4bd2-b2ab-c3716079936e)  
(KB958434)  
(Önemli)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4b3989ef-02b8-4bd2-b2ab-c3716079936e)  
(KB958434)  
(Önemli)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=9dbb35c1-aa7a-481b-a330-8ba916ddd443)  
(KB958442)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3 ve Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=70de7c3c-519f-4f4a-a03f-027f80b5415c)  
(KB956366)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=55430121-4476-48b8-9f6f-4a60fa0b2970)  
(KB956828)  
(Önemli)  
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=55430121-4476-48b8-9f6f-4a60fa0b2970)  
(KB956828)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f)  
(KB958439)  
(Önemli)  
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f)  
(KB958439)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
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
[Microsoft Office SharePoint Server 2007 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)  
(KB956716)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)  
(KB956716)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=a7fda284-273c-42ab-8188-433beaacca86)  
(KB956716)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=a7fda284-273c-42ab-8188-433beaacca86)  
(KB956716)  
(Önemli)
</td>
</tr>
</table>
 
**MS08-070 için Not**
Diğer güncelleştirme dosyaları için **Microsoft Geliştirici Araçları ve Yazılımları** adlı sonraki bölüme de bakın. Bu bülten hem Microsoft Office hem de Microsoft Geliştirici Araçları ve Yazılımları içindir.

**MS08-077 için Not**
Diğer güncelleştirme dosyaları için **Microsoft Server Yazılımı** bölümüne de bakın. Bu bülten hem Microsoft Office Paketleri hem de Microsoft Server Yazılımı içindir.

**MS08-070'te Microsoft Office FrontPage için Not**
\*Bu güncelleştirme FrontPage 2002 Service Pack 3'ün yalnızca Basitleştirilmiş Çince (Çin), Çince Pan (Hong Kong), Geleneksel Çince (Tayvan) ve Kore dili sürümlerine uygulanır.

**MS08-072 ve MS08-074'te Mac için Microsoft Office için Not**
\*\*MS08-072 ve MS08-074'te karşılık gelen güncelleştirmeler aynıdır. Güvenlik açıkları aynı dosyalarda bulunduğu için, bu güncelleştirmeler her iki bülten için de aynıdır.

**MS08-072'de Works 8 için Not**
\*\*\*Microsoft Works 8.0 çalıştıran müşterilere bu güvenlik güncelleştirmesinin sunulması için, önce [Microsoft Works Güncelleştirmesi](http://www.microsoft.com/products/works/international/update_1001.mspx) makalesinde açıklandığı şekilde Works 8.5 sürümüne güncelleştirmeleri gerekir. Bu durum Microsoft Works 8.0, Works Suite 2004 ve Works Suite 2005 kullanan tüm müşteriler için geçerlidir. Works Suite 2006 çalıştıran müşteriler için Works 8.5 zaten bulunmaktadır.

**MS08-074'te Microsoft Office Excel 2007 ve Microsoft Office Excel 2007 Service Pack 1 için Not**
\*\*\*\*Microsoft Office Excel 2007 ve Microsoft Office Excel 2007 Service Pack 1 için, müşterilerin MS08-074'te açıklanan güvenlik açıklarına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB958437'nin yanı sıra, [Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f)'ne yönelik güvenlik güncelleştirmesini (KB958439) de yüklemeleri gerekmektedir. KB958437 ve KB958439 güncelleştirme paketlerini daha önce başarıyla yüklemiş olan müşterilerin yeniden yüklemeleri gerekmez.

#### Microsoft Geliştirici Araçları ve Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
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
Microsoft Visual Basic
</td>
<td style="border:1px solid black;">
[Microsoft Visual Basic 6.0 Çalışma Zamanı Modülü Ek Dosyaları](http://www.microsoft.com/downloads/details.aspx?familyid=e27eebcb-095d-43ec-a19e-4a46e591715c)  
(KB926857)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=afad980d-7f27-49d9-aa23-b762c7b94cd6)  
(KB958392)  
(Kritik)  
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6ac7cf8f-d046-43a8-b4ef-253153d65aed)  
(KB958393)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a6977f81-f7f6-486b-96ad-8d296d79f205)  
(KB958369)  
(Kritik)  
[Microsoft Visual FoxPro 9.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=386d27a6-b2c7-4acc-bf3e-edcbc7358172)  
(KB958370)  
(Kritik)  
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b1f28a9-da8d-463a-8ae4-dfc8fcc6c41a)  
(KB958371)  
(Kritik)
</td>
</tr>
</table>
 
**MS08-070 için Not**
Diğer güncelleştirme dosyaları için **Microsoft Office Paketleri ve Yazılımları** adlı önceki bölüme de bakın. Bu bülten hem Microsoft Office Paketleri ve Yazılımları hem de Microsoft Geliştirici Araçları ve Yazılımları içindir.

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
Arama Sunucusu
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
Microsoft Search Server
</td>
<td style="border:1px solid black;">
[Microsoft Search Server 2008 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)\*  
(KB956716)  
(Önemli)  
[Microsoft Search Server 2008 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=a7fda284-273c-42ab-8188-433beaacca86)\*\*  
(KB956716)  
(Önemli)
</td>
</tr>
</table>
 
**MS08-077 için Notlar**

\*Microsoft Search Server 2008 Express (32-bit) sürümünü içerir

\*\*Microsoft Search Server 2008 Express (64-bit) sürümünü içerir

Diğer güncelleştirme dosyaları için **Microsoft Office Paketleri ve Yazılımları** adlı bölüme de bakın. Bu bülten hem Microsoft Office Paketleri hem de Microsoft Server Yazılımı içindir.

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

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): 2008 yılındaki Software Update Services ve Windows Server Update Services içerik değişikliklerinin açıklaması. Tüm Windows içeriği yer alır.
-   [Microsoft Windows Dışındaki Microsoft Ürünleri için Yeni, Yeniden Düzenlenen ve Yayımlanan Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   [VenusTech](http://www.venustech.com.cn/) için çalışan ADLab, MS08-070'te açıklanan sorunları bildirdiği için
-   [Affiliated Computer Services](http://www.acs-inc.com/) için çalışan Jason Medeiros, MS08-070'te açıklanan sorunu bildirdiği için
-   [Secunia Research](http://secunia.com/) için çalışan Carsten Eiram, MS08-070'te açıklanan sorunu bildirdiği için
-   [McAfee Avert Labs](http://www.avertlabs.com/) için çalışan Mark Dowd, MS08-070'te açıklanan sorunu bildirdiği için
-   [Insomnia Security](http://www.insomniasec.com/) için çalışan Brett Moore, MS08-070'te açıklanan sorunu bildirdikleri için
-   CHkr\_D591, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-070'te açıklanan sorunu bildirdikleri için
-   [CERT/CC](http://www.cert.org/) için çalışan Michal Bucko, MS08-070'te açıklanan sorunu bildirdiği için
-   Symantec bünyesindeki [Security Intelligence Analysis Team](http://www.symantec.com/), MS08-070'te açıklanan sorun konusunda bizimle birlikte çalıştıkları için
-   [Verisign iDefense Labs](http://labs.idefense.com/) için çalışan Jun Mao, MS08-071'de açıklanan sorunu bildirdiği için
-   Juan Caballero, [Carnegie Mellon University'deki Bitblaze grubu ve UC Berkeley](http://bitblaze.cs.berkeley.edu/) birlikte çalışarak MS08-071'de açıklanan sorunu bildirdikleri için
-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Ricardo Narvaja, MS08-072'de açıklanan sorunu bildirdiği için
-   [Secunia Research](http://secunia.com/) için çalışan Dyon Balding, MS08-072'de açıklanan sorunu bildirdiği için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, MS08-072'de açıklanan sorunu bildirdiği için
-   Wushi, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-072'de açıklanan sorunu bildirdikleri için
-   [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) için çalışan Aaron Portnoy, MS08-072'de açıklanan sorunları bildirdiği için
-   [team509](http://www.team509.com/) için çalışan Wushi ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS08-072'de açıklanan sorunu bildirdiği için
-   Wushi ve Ling, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-072'de açıklanan sorunları bildirdikleri için
-   Carlo Di Dato (diğer adıyla shinnai), MS08-073'te açıklanan sorunu bildirdiği için
-   Brett Moore, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-073'te açıklanan sorunu bildirdikleri için
-   [Casaba Security](http://www.casabasecurity.com/) için çalışan Chris Weber, MS08-073'te açıklanan sorunu bildirdiği için
-   [Verisign iDefense Labs](http://labs.idefense.com/) için çalışan Jun Mao, MS08-073'te açıklanan sorunu bildirdiği için
-   [Verisign iDefense Labs](http://labs.idefense.com/) için çalışan Joshua J. Drake, MS08-074'te açıklanan sorunu bildirdiği için
-   [signedness.org](http://www.signedness.org/) için çalışan Claes M Nyberg, MS08-074'te açıklanan sorunu bildirdiği için
-   [Secunia](http://secunia.com/) için çalışan Dyon Balding, MS08-074'te açıklanan sorunu bildirdiği için
-   [eEye Digital Security](http://www.eeye.com/) için çalışan Andre Protas, MS08-075'te açıklanan sorunu bildirdiği için
-   Nate McFeters, MS08-075'te açıklanan sorunu bildirdiği için
-   Anonim bir kullanıcı, MS08-077'de açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (9 Aralık 2008): Bülten özeti yayımlandı.
-   V2.0 (10 Aralık 2008): MS08-076 için etkilenen yazılımlar, Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2 üzerinde Windows Media Format Çalışma Zamanı 9.5 ve Windows Media Format Çalışma Zamanı 11 ayrı güncelleştirmeler olarak listelenecek şekilde düzeltildi. Ayrıca, MS08-076 için Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2 üzerinde Windows Media Format Çalışma Zamanı 11 x64 Edition'a yönelik hatalı başvurular kaldırıldı.
-   V3.0 (17 Aralık 2008): Microsoft Güvenlik Bülteni MS08-078 eklendi, Internet Explorer için Güvenlik Güncelleştirmesi (960714). Bu bant dışı güvenlik bülteni için bülten web yayını bağlantıları da eklendi.
-   V3.1 (18 Aralık 2008): MS08-078 için, 32-Bit Sistemler için Windows Server 2008 ve x64 Tabanlı Sistemler için Windows Server 2008 üzerinde Windows Internet Explorer 7 için sunucu çekirdeğinin etkilenmediği bildirimi eklendi.
-   V3.2 (7 Ocak 2009): MS08-072'deki Etkilenen Yazılımlar tablosundan Microsoft Office Word Viewer 2003 kaldırıldı.
-   V4.0 (13 Ocak 2009): Microsoft, Windows XP Service Pack 2 (KB952069) ve Windows XP Service Pack 3 (KB952069) üzerinde Windows Media Çalışma Zamanı 9.5 için yeni güncelleştirme paketleri sunmak amacıyla MS08-076'yı yeniden yayımladı. Windows Media bileşenlerinin desteklenen ve etkilenen diğer tüm sürümlerini çalıştıran ve özgün MS08-076 güvenlik güncelleştirmesi paketlerini yüklemiş olan müşterilerin başka bir işlem yapmaları gerekmez. Ayrıca, MS08-076 için, Windows Media Player 6.4 ve Windows Media Hizmetleri 4.1'in tüm Microsoft Windows 2000 Service Pack 4 sürümlerinde etkilendiği belirtilmiştir. Bu güncelleştirmenin (Windows Media Player 6.4 için KB954600 veya Windows Media Hizmetleri 4.1 için KB952068) önerildiği ancak güncelleştirmeyi uygulamamış olan müşterilerin, uygulamaları gerekir. Son olarak, MS08-072 için Microsoft Office Word Viewer'ın etkilendiği belirtilmiştir; KB956366 güvenlik güncelleştirmesini başarıyla yüklemiş olan müşterilerin yeniden yüklemesi gerekmemektedir.
-   V5.0 (28 Ocak 2009): Microsoft Office Excel 2007'nin desteklenen sürümleri için güvenlik güncelleştirmesi KB958437 ve KB958439 ile ilgili olarak, **Etkilenen Yazılımlar** tablosuna bir dipnot eklendi. Güvenlik güncelleştirmesinin ikili dosyalarında veya algılamada herhangi bir değişiklik yapılmadı. Microsoft Office Excel 2007 veya Microsoft Office Excel 2007 Service Pack 1 kullanan ve KB958437'yi ve KB958439'u zaten yüklemiş olan müşterilerin yeniden yüklemeleri gerekmez.
-   V6.0 (29 Nisan 2009): MS08-076 için etkilenen yazılım olarak Windows Server 2008 Service Pack 2'nin 32-bit ve x64 tabanlı sürümleri üzerinde Windows Media Services 2008 (KB952068) eklendi. Bu, yalnızca bir algılama değişikliğidir; ikili dosyalarda değişiklik yapılmamıştır. KB952068'i başarıyla yüklemiş olan müşterilerin yeniden yüklemeleri gerekmez.

*Built at 2014-04-18T01:50:00Z-07:00*
