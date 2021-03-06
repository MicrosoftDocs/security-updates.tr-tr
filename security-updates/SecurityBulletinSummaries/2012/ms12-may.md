---
TOCTitle: 'MS12-MAY'
Title: Microsoft Güvenlik Bülteni Mayıs 2012 Özeti
ms:assetid: 'ms12-may'
ms:contentKeyID: 61235853
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms12-may(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Mayıs 2012 Özeti
===========================================

Yayım Tarihi: 8 Mayıs 2012 Salı | Güncelleştirme Tarihi: 22 Mayıs 2012 Salı

**Sürüm:** 2.1

Bu bülten özetinde Mayıs 2012'de yayımlanan güvenlik bültenleri listelenir.

Mayıs 2012 güvenlik bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 3 Mayıs 2012'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://go.microsoft.com/fwlink/?linkid=217213).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 9 Mayıs 2012 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Mayıs Güvenlik Bülteni Web Yayını için şimdi kaydolun](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032499667). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://go.microsoft.com/fwlink/?linkid=217214).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248419"><strong>MS12-029</strong></a></td>
<td style="border:1px solid black;"><strong>Microsoft Word'deki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2680352)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir RTF dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, geçerli kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;"><strong>Microsoft Office, Windows, .NET Framework ve Silverlight için Birleşik Güvenlik Güncelleştirmesi (2681578)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office, Microsoft Windows, Microsoft .NET Framework ve Microsoft Silverlight'taki genel olarak duyurulan üç ve özel olarak bildirilen yedi güvenlik açığını giderir. Bu güvenlik açıklarının önem düzeyi en yüksek olanı, bir kullanıcı özel hazırlanmış bir belgeyi açarsa veya TrueType yazı tipi dosyalarının katıştırılmış olduğu kötü amaçlı bir web sayfasını ziyaret ederse uzaktan kod yürütülmesine izin verebilir. Bir saldırganın bir kullanıcıyı kötü amaçlı bir web sitesini ziyaret etmeye zorlama yolu yoktur. Bunun yerine, saldırganın kullanıcıları bir e-posta iletisindeki veya Instant Messenger iletisindeki kendi web sitesine yönlendiren bir bağlantıyı tıklatmalarını sağlayarak onları bu web sitesini ziyaret etmeye ikna etmesi gerekir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework, Microsoft Silverlight,<br />
Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;"><strong>.NET Framework'teki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (2693777)</strong><br />
<br />
Bu güvenlik güncelleştirmesi .NET Framework'teki özel olarak bildirilen iki güvenlik açığını giderir. Güvenlik açıkları, bir kullanıcı özel hazırlanmış bir web sayfasını XAML Tarayıcı Uygulamaları (XBAP) çalıştırabilen bir web tarayıcısı kullanarak görüntülerken istemci sistemde uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;"><strong>Microsoft Office'teki</strong> <strong>Güvenlik Açıkları</strong> <strong>Uzaktan Kod Yürütülmesine İzin Verebilir (2663830)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Office'teki genel olarak duyurulan bir ve özel olarak bildirilen beş güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Office dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açıklarından başarıyla yararlanan bir saldırgan, oturum açan kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248385"><strong>MS12-031</strong></a></td>
<td style="border:1px solid black;"><strong>Microsoft Visio Viewer 2010'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (2597981)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Visio dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, geçerli kullanıcı ile aynı haklara sahip olabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;"><strong>TCP/IP'deki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2688338)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki özel olarak bildirilen ve genel olarak duyurulan birer güvenlik açığını giderir. Bu güvenlik açıklarından önem düzeyi daha yüksek olanı, bir saldırgan hedeflenen sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükseltmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=247902"><strong>MS12-033</strong></a></td>
<td style="border:1px solid black;"><strong>Windows Bölüm Yöneticisi'ndeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (2690533)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Windows'daki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan sistemde oturum açar ve özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine izin verebilir. Saldırganın bu güvenlik açığından yararlanabilmesi için geçerli oturum açma kimlik bilgilerine sahip olması ve yerel olarak oturum açabilmesi gerekir.</td>
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

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Güvenlik Açığı Başlığı</th>
<th style="border:1px solid black;" >CVE Kimliği</th>
<th style="border:1px solid black;" >En Son Yazılım Sürümü için Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Yazılımın Eski Sürümleri için Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Hizmet Reddi Yararlanma Değerlendirmesi</th>
<th style="border:1px solid black;" >Önemli Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248419"><strong>MS12-029</strong></a></td>
<td style="border:1px solid black;">RTF Uyumsuzluğu Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0183">CVE-2012-0183</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel Dosya Biçiminde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0141">CVE-2012-0141</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel Dosya Biçimindeki OBJECTLINK Kaydında Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0142">CVE-2012-0142</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel'de Çeşitli Değiştirilmiş Baytlar Kullanıldığında Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0143">CVE-2012-0143</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Yalnızca Microsoft Office 2003 etkilenir.<br />
<br />
Bu güvenlik açığı genel olarak duyurulmuştur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel SXLI Kaydında Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0184">CVE-2012-0184</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel MergeCells Kaydında Öbek Taşması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0185">CVE-2012-0185</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Yararlanma kodunun oluşturulması zor olabilir</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Yararlanma kodunun oluşturulması zor olabilir</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=238499"><strong>MS12-030</strong></a></td>
<td style="border:1px solid black;">Excel Series Kaydını Ayrıştırmada Tür Uyumsuzluğu Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1847">CVE-2012-1847</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=248385"><strong>MS12-031</strong></a></td>
<td style="border:1px solid black;">VSD Dosya Biçiminde Bellek Bozulması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0018">CVE-2012-0018</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Visio Viewer 2010 ve Visio Viewer 2010 Service Pack 1'i (Visio Viewer'ın yalnızca desteklenen sürümlerini) etkiler.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;">Windows Güvenlik Duvarı'nı Atlama Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0174">CVE-2012-0174</a></td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Bu bir güvenliği atlama güvenlik açığıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246964"><strong>MS12-032</strong></a></td>
<td style="border:1px solid black;">TCP/IP'de İki Kez Bırakma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0179">CVE-2012-0179</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=247902"><strong>MS12-033</strong></a></td>
<td style="border:1px solid black;">Tak ve Kullan (PnP) Yapılandırma Yöneticisi Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0178">CVE-2012-0178</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Geçici</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">TrueType Yazı Tipini Ayrıştırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3402">CVE-2011-3402</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">TrueType Yazı Tipini Ayrıştırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0159">CVE-2012-0159</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">.NET Framework'te Arabellek Ayırma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0162">CVE-2012-0162</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">GDI+ Uygulamasında Kayıt Türü Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0165">CVE-2012-0165</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">2</a> - Yararlanma kodunun oluşturulması zor olabilir</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">GDI+ Uygulamasında Öbek Taşması Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0167">CVE-2012-0167</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Silverlight'ta İki Kez Bırakma Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0176">CVE-2012-0176</a></td>
<td style="border:1px solid black;">Etkilenmez</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Windows ve İletiler Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0180">CVE-2012-0180</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Klavye Düzeni Dosyası Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0181">CVE-2012-0181</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">3</a> - Yararlanma kodu olasılığı düşük</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">Bu güvenlik açığı genel olarak duyurulmuştur.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=251038"><strong>MS12-034</strong></a></td>
<td style="border:1px solid black;">Kaydırma Çubuğunu Hesaplama Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-1848">CVE-2012-1848</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Kalıcı</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;">.NET Framework'te Seri Hale Getirme Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0160">CVE-2012-0160</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">(Yok)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=246970"><strong>MS12-035</strong></a></td>
<td style="border:1px solid black;">.NET Framework'te Seri Hale Getirme Güvenlik Açığı</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2012-0161">CVE-2012-0161</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx">1</a> - Yararlanma kodu olasılığı yüksek</td>
<td style="border:1px solid black;">Uygulanamaz</td>
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

 
<table style="border:1px solid black;">
<tr>
<th colspan="5">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b2ea7a8d-a537-441c-8e80-2ba4ac37e320)  
(KB2660649)  
(Yalnızca Tablet PC Edition 2005 Service Pack 3)  
(Önemli)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9a4db1b4-15b2-4fae-83c4-a86331425c9e)  
(KB2659262)  
(Önemli)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=8d341077-8fcd-4666-a27e-2141a04a321e)  
(KB2676562)  
(Kritik)  
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=954e8ae9-9247-496a-bbde-76981c49e3b3)  
(KB2686509)  
(Önemli)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b0803633-7fda-4862-a908-3450180cdaaa)  
(KB2604042)  
(Yalnızca Media Center Edition 2005 Service Pack 3 ve Tablet PC Edition 2005 Service Pack 3)  
(Kritik)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
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
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6ebaccbc-512b-4f2f-bf2a-8958f012e13f)  
(KB2659262)  
(Önemli)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e0357165-4400-40a6-a7a4-7b762a1793ba)  
(KB2676562)  
(Kritik)  
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f3b1568f-d7ad-4e6e-b45b-53b16b303d9d)  
(KB2686509)  
(Önemli)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
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
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bc7bfb79-8eaf-4c22-b1c9-e774c55eb06d)  
(KB2659262)  
(Önemli)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6287b994-041f-45b7-a230-d689bf1901a8)  
(KB2676562)  
(Kritik)  
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=167e8c49-f9f6-488b-86ad-4056d3d20213)  
(KB2686509)  
(Önemli)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b0df42a4-7444-4da6-a9b2-35a56bdc64a4)  
(KB2604078)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bf7c9aea-dc18-499f-b456-2c29e9a74a15)  
(KB2659262)  
(Önemli)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f9f49cd0-24db-4438-afde-aa7113ec2035)  
(KB2676562)  
(Kritik)  
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4614161c-ae05-43ad-8dd3-85975ec2bc4c)  
(KB2686509)  
(Önemli)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c9bf7fde-3b6f-44fe-93b3-8a4dc01c1cc5)  
(KB2656407)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=18a66b7c-f062-4236-8340-a867b1e31b78)  
(KB2604110)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
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
Itanium Tabanlı Sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=6414b607-6fb1-4527-b218-c3cb5adfd4d1)  
(KB2659262)  
(Önemli)  
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=2563425d-4f6e-4f33-b775-a8d421b0e254)  
(KB2676562)  
(Kritik)  
[Itanium Tabanlı Sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=67f659ee-0d28-40f3-ae2f-f8fceeac8bff)  
(KB2686509)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=cb5afeaf-a500-4b71-a91b-a300884b040e)  
(KB2604092)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
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
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e11d8738-379a-4dfe-b21c-495041d9523a)  
(KB2658846)  
(Önemli)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d8068e95-ac4d-45e8-84b7-b12d633c70b5)  
(KB2659262)  
(Önemli)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=02c857c6-5dfa-46fb-adef-35eac2bf5f41)  
(KB2660649)  
(Önemli)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=292d1f3b-a065-4d7d-9046-f35ab7f0591b)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b1dc6e10-34eb-45ea-92b3-9983c00f6cb5)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d9d5e290-dc57-4587-b31d-706b541924ec)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=838f588b-2a0d-4dae-b54d-782e6985fd83)  
(KB2658846)  
(Önemli)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3bde7f59-163c-4491-abc9-a822daa8142f)  
(KB2659262)  
(Önemli)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9f97c5a4-62ee-4e4f-8811-a43545d76327)  
(KB2660649)  
(Önemli)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8f90c09c-a2cb-4adb-ace7-a8bc38d78ba6)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d65565d4-d865-438a-bfb7-d71af9dd884e)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=827b9f15-b67d-4dd4-a39b-7c148bae5041)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=360adbed-a451-44ed-8675-ca5624ef1cf3)  
(KB2658846)  
(Önemli)  
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47a0df29-f42e-463b-9c15-a93385ff8705)  
(KB2659262)  
(Önemli)  
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=278c378b-6ee4-4f80-b9c3-ede885f4bbda)<sup>[3]</sup>
(KB2660649)  
(Önemli)  
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=728a84b9-c1b8-46e2-8365-1b542963508a)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ef72aab-7fd2-4330-bb6a-0c77c3943345)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46e6e960-b700-4154-b91d-aca74ea9e5df)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d5a6d617-8ef6-42fa-a325-c15fa7ece7aa)  
(KB2658846)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e6d29e1-17fc-4670-9e69-988c040f06e2)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=98c4ac87-eec2-4e02-b0e1-00626bcb0ffd)<sup>[3]</sup>
(KB2660649)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab897da8-a927-42eb-87da-1e5cd820f4c0)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0511303a-79f6-4bd9-8f50-b5836c9c476f)  
(KB2656409)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritik)  
[Microsoft .NET Framework 3.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=06273728-7f22-40db-be11-8fb03e7e0bfb)  
(KB2604105)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9569d980-766d-4825-bd1c-f30c93d4b035)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e4ab05ae-3a1c-4d6b-8c84-1165ed741356)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c65df271-8b7d-46d3-81b3-87c0ad05e8d0)  
(KB2659262)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=11da5031-1733-43ea-9204-294eb483c858)  
(KB2676562)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=88501ecb-dcf6-4956-8eab-e1076a975846)  
(KB2656353)  
(Kritik)  
[Microsoft .NET Framework 2.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=8b504a01-1e6b-42c0-b974-811350302ace)  
(KB2604094)  
(Kritik)  
[Microsoft .NET Framework 3.5 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d6f0ccd6-c8ec-45a0-beba-155989ca19b3)  
(KB2604111)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5f7ee25-2fc1-44c7-b3e6-e2c969ecf1bc)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c081b058-b95e-4467-a2fc-fb1a68345c8f)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="5">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=f4d52649-4afc-4c01-b275-93818152f6b7)  
(KB2658846)  
(Önemli)  
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=31607fd8-fae8-47a0-971e-0e68be67fb5a)  
(KB2659262)  
(Önemli)  
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=35443cfc-0f51-412a-a9d9-91bfb19d805e)  
(KB2660649)  
(Önemli)  
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=572af8d4-effb-41a6-8448-7576b03f18fd)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=46b8749e-3d8f-472f-a1ea-419f44c6bc00)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=2a4433e4-7f3f-4083-b3e1-eff2d18483af)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
32-bit sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f4d52649-4afc-4c01-b275-93818152f6b7)  
(KB2658846)  
(Önemli)  
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=31607fd8-fae8-47a0-971e-0e68be67fb5a)  
(KB2659262)  
(Önemli)  
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=35443cfc-0f51-412a-a9d9-91bfb19d805e)  
(KB2660649)  
(Önemli)  
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=572af8d4-effb-41a6-8448-7576b03f18fd)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=46b8749e-3d8f-472f-a1ea-419f44c6bc00)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2a4433e4-7f3f-4083-b3e1-eff2d18483af)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=7aa0b61b-b42c-4d60-8a7f-c61cbd25d6d9)  
(KB2658846)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=fa38b001-eef8-4153-b077-ea524e8a1e18)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=7e551e0f-3f02-49ee-a5a1-8a7480722a6b)  
(KB2660649)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=c09cbb73-7814-4946-8c0a-323d304dd633)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=e89fb3f1-44cb-4fc0-bbc2-8e94d6933322)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7](http://www.microsoft.com/downloads/details.aspx?familyid=dfa13df5-9e4e-4cf6-b56d-af7db0a0f5ea)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7aa0b61b-b42c-4d60-8a7f-c61cbd25d6d9)  
(KB2658846)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fa38b001-eef8-4153-b077-ea524e8a1e18)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7e551e0f-3f02-49ee-a5a1-8a7480722a6b)  
(KB2660649)  
(Önemli)  
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c09cbb73-7814-4946-8c0a-323d304dd633)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e89fb3f1-44cb-4fc0-bbc2-8e94d6933322)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows 7 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dfa13df5-9e4e-4cf6-b56d-af7db0a0f5ea)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="5">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=6f815b10-c60d-4e9b-8283-494036985e93)  
(KB2658846)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=6dab7283-81ba-4362-adb1-0db25e1f055e)\[4\]  
(KB2660649)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6f815b10-c60d-4e9b-8283-494036985e93)  
(KB2658846)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6dab7283-81ba-4362-adb1-0db25e1f055e)\[4\]  
(KB2660649)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Kritik)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)<sup>[1]</sup>
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=b9172218-8a3f-4b0f-a14d-64db3778f4cc)  
(KB2658846)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=d9abec73-150e-40cf-a108-1d8ee89aac92)  
(KB2659262)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=e075c03e-91db-4974-a6ea-8edeba583293)  
(KB2676562)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=34643abe-2905-4ac1-a5f3-3f6ea8724b7a)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=9b66a74a-7022-49ac-89da-8c9ab8105812)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b9172218-8a3f-4b0f-a14d-64db3778f4cc)  
(KB2658846)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d9abec73-150e-40cf-a108-1d8ee89aac92)  
(KB2659262)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=e075c03e-91db-4974-a6ea-8edeba583293)  
(KB2676562)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34643abe-2905-4ac1-a5f3-3f6ea8724b7a)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9b66a74a-7022-49ac-89da-8c9ab8105812)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="5">
Sunucu Çekirdeği yükleme seçeneği
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-035**](http://go.microsoft.com/fwlink/?linkid=246970)
</td>
<td style="border:1px solid black;">
[**MS12-032**](http://go.microsoft.com/fwlink/?linkid=246964)
</td>
<td style="border:1px solid black;">
[**MS12-033**](http://go.microsoft.com/fwlink/?linkid=247902)
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
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-bit sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=47a0df29-f42e-463b-9c15-a93385ff8705)  
(KB2659262)  
(Önemli)  
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=728a84b9-c1b8-46e2-8365-1b542963508a)  
(KB2676562)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7ef72aab-7fd2-4330-bb6a-0c77c3943345)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46e6e960-b700-4154-b91d-aca74ea9e5df)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 Service Pack 2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e6d29e1-17fc-4670-9e69-988c040f06e2)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab897da8-a927-42eb-87da-1e5cd820f4c0)  
(KB2676562)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=9569d980-766d-4825-bd1c-f30c93d4b035)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e4ab05ae-3a1c-4d6b-8c84-1165ed741356)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Önemli)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=d04bfc77-d05f-4890-9175-27ad00e84c4a)  
(KB2656410)  
(Önem derecesi yok<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=cd42511f-788c-4473-84cc-19bb1623e337)  
(KB2604114)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=34824de4-0f26-4627-8ddb-23d6b9d6671a)  
(KB2659262)  
(Önemli)  
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1a179bf7-17fa-4dc7-b0c1-af6d911373cd)  
(KB2676562)  
(Önemli)  
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=c06506e6-5838-4bba-9b12-b54dfa30a944)  
(KB2656411)  
(Önem derecesi yok<sup>[2]</sup>)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=4ee3cb61-542e-4e42-aa0e-0cbf8dd89648)  
(KB2656405)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](http://www.microsoft.com/downloads/details.aspx?familyid=85e0f8be-cdc7-464b-be43-da23d82b3486)  
(KB2604115)  
(Kritik)  
[Microsoft .NET Framework 4](http://www.microsoft.com/downloads/details.aspx?familyid=38b389d8-d534-4b0a-8dd4-b72a5ce7c4e8)<sup>[1]</sup>
(KB2604121)  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=08ba4320-6c47-4f82-a54f-61a32629b985)  
(KB2688338)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 R2 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=095c20b3-8e6c-4846-9ba1-6ce0af5e9850)  
(KB2690533)  
(Önemli)
</td>
</tr>
</table>
 
**MS12-034** **için** **Notlar**

<sup>[1]</sup>**.NET Framework 4 ve .NET Framework 4 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4 ve .NET Framework 4 İstemci Profili. .NET Framework 4 İstemci Profili, .NET Framework 4'ün bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4'ü hem de .NET Framework 4 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

<sup>[2]</sup>Bu bültende açıklanan güvenlik açığıyla ilgili olduğu bilinen saldırı vektörü olmadığı için, önem dereceleri bu güncelleştirmeye uygulanmamıştır. Ancak Microsoft kapsamlı bir savunma önlemi olarak, bu yazılımı kullanan müşterilerin bu güvenlik güncelleştirmesini uygulamalarını önerir.

<sup>[3]</sup>Bu güncelleştirme yalnızca isteğe bağlı Masaüstü Deneyimi özelliğinin yüklü ve etkinleştirilmiş olduğu Windows Server 2008 tabanlı sistemlere uygulanır. Ayrıntılar için MS12-034'teki Güncelleştirme Hakkında SSS bölümüne bakın.

\[4\]Bu güncelleştirme yalnızca isteğe bağlı Mürekkep ve El Yazısı Hizmetleri özelliğinin Mürekkep Desteği bileşeninin yüklü ve etkinleştirilmiş olduğu Windows Server 2008 R2 tabanlı sistemlere uygulanır. Ayrıntılar için MS12-034'teki Güncelleştirme Hakkında SSS bölümüne bakın.

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

**MS12-035** **için** **Not**

<sup>[1]</sup>**.NET Framework 4 ve .NET Framework 4 İstemci Profili etkilenir.** .NET Framework sürüm 4 yeniden dağıtılabilir paketleri iki profil olarak kullanıma sunulmuştur: .NET Framework 4 ve .NET Framework 4 İstemci Profili. .NET Framework 4 İstemci Profili, .NET Framework 4'ün bir alt kümesidir. Bu güncelleştirmeyle giderilen güvenlik açığı hem .NET Framework 4'ü hem de .NET Framework 4 İstemci Profili'ni etkiler. Daha fazla bilgi için, [.NET Framework'ü Yükleme](http://msdn.microsoft.com/en-us/library/5a4x27ek.aspx) adlı MSDN makalesine bakın.

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<tr>
<th colspan="5">
Microsoft Office Paketleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9819899d-7f7f-4ddd-9fc8-816a57d2979e)  
(KB2598332)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0abbf09c-8828-4524-8b38-e34faefa2ae4)  
(KB2598253)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=162901b1-4c1d-476f-99e9-218780897f92)  
(KB2597086)  
(Önemli)
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
[Microsoft Word 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c6f79d01-8735-4b0f-a50b-90cde3fba4ee)<sup>[1]</sup>
(KB2596917)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b9a27671-883a-4ab7-b86f-99730a9af729)  
(KB2596672)  
(Önemli)  
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fa054591-b202-47f2-9610-f3cd288d34c0)  
(KB2596792)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=22b9b3a6-ad09-4397-892c-2190a86baf3e)<sup>[1]</sup>
(KB2597161)  
(Önemli)  
[Microsoft Office 2007 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6ff6650c-eaf4-4c7d-986c-c4d9e5324dac)  
(KB2597969)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Word 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c6f79d01-8735-4b0f-a50b-90cde3fba4ee)<sup>[1]</sup>
(KB2596917)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b9a27671-883a-4ab7-b86f-99730a9af729)  
(KB2596672)  
(Önemli)  
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=fa054591-b202-47f2-9610-f3cd288d34c0)  
(KB2596792)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=22b9b3a6-ad09-4397-892c-2190a86baf3e)<sup>[1]</sup>
(KB2597161)  
(Önemli)  
[Microsoft Office 2007 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=6ff6650c-eaf4-4c7d-986c-c4d9e5324dac)  
(KB2597969)  
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=c355d598-ff4d-4cac-afa9-2de3236a7d71)  
(KB2589337)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f537f6d0-be63-42af-8b39-fa6f38715f84)  
(KB2597166)  
(Önemli)  
[Microsoft Office 2010 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=2e1060fa-c43d-42df-be5f-f536d9b39ba4)  
(KB2553371)  
(Önemli)
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
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=c355d598-ff4d-4cac-afa9-2de3236a7d71)  
(KB2589337)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=f537f6d0-be63-42af-8b39-fa6f38715f84)  
(KB2597166)  
(Önemli)  
[Microsoft Office 2010 Service Pack 1 (32-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=2e1060fa-c43d-42df-be5f-f536d9b39ba4)  
(KB2553371)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=91619bcc-9d5d-4011-a185-c405758782be)  
(KB2589337)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=123b96d9-de3f-4aab-bcf8-bf9089fef400)  
(KB2597166)  
(Önemli)  
[Microsoft Office 2010 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=ec4371f6-644d-430d-880f-12425f1b36d4)  
(KB2553371)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64-bit sürümler)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 Service Pack 1 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=91619bcc-9d5d-4011-a185-c405758782be)  
(KB2589337)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 Service Pack 1 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=123b96d9-de3f-4aab-bcf8-bf9089fef400)  
(KB2597166)  
(Önemli)  
[Microsoft Office 2010 Service Pack 1 (64-bit sürümler)](http://www.microsoft.com/downloads/details.aspx?familyid=ec4371f6-644d-430d-880f-12425f1b36d4)  
(KB2553371)  
(Önemli)
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
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2008
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=8f85fc23-480e-4835-9ce5-0aa56702ef59)  
(KB2665346)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=8f85fc23-480e-4835-9ce5-0aa56702ef59)  
(KB2665346)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2011
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2011](http://www.microsoft.com/downloads/details.aspx?familyid=5d88d3d4-89bd-44c3-9e5a-657998223e2f)  
(KB2665351)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2011](http://www.microsoft.com/downloads/details.aspx?familyid=5d88d3d4-89bd-44c3-9e5a-657998223e2f)  
(KB2665351)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="5">
Diğer Microsoft Office Yazılımları
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-029**](http://go.microsoft.com/fwlink/?linkid=248419)
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
</td>
<td style="border:1px solid black;">
[**MS12-030**](http://go.microsoft.com/fwlink/?linkid=238499)
</td>
<td style="border:1px solid black;">
[**MS12-031**](http://go.microsoft.com/fwlink/?linkid=248385)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=9dedfb18-a651-49f7-b1fc-78f7b6cb234a)<sup>[2]</sup>
(KB2596842)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio Viewer 2010
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
[Microsoft Visio Viewer 2010 (32-bit Edition)](http://www.microsoft.com/downloads/details.aspx?familyid=0d21d110-c787-49b6-8384-6eaf9da5a38f)  
(KB2597981)  
(Önemli)  
[Microsoft Visio Viewer 2010 Service Pack 1 (32-bit Edition)](http://www.microsoft.com/downloads/details.aspx?familyid=0d21d110-c787-49b6-8384-6eaf9da5a38f)  
(KB2597981)  
(Önemli)  
[Microsoft Visio Viewer 2010 (64-bit Edition)](http://www.microsoft.com/downloads/details.aspx?familyid=331d8247-559c-4040-bdea-84cb6fd5dee2)  
(KB2597981)  
(Önemli)  
[Microsoft Visio Viewer 2010 Service Pack 1 (64-bit Edition)](http://www.microsoft.com/downloads/details.aspx?familyid=331d8247-559c-4040-bdea-84cb6fd5dee2)  
(KB2597981)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Uyumluluk Paketi Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=80d5a86a-33b0-4464-af76-0fe13bd07a5c)  
(KB2596880)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Uyumluluk Paketi Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a8386ad9-635f-45a7-b33e-ac9a3ca55f82)  
(KB2597162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Uyumluluk Paketi Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Uyumluluk Paketi Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=80d5a86a-33b0-4464-af76-0fe13bd07a5c)  
(KB2596880)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Uyumluluk Paketi Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=a8386ad9-635f-45a7-b33e-ac9a3ca55f82)  
(KB2597162)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**MS12-029** **için Not**

<sup>[1]</sup>Microsoft Word 2007 için, müşterilerin bu bültende açıklanan güvenlik açığına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB2596917'nin yanı sıra Microsoft Office Uyumluluk Paketi (KB2596880) güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

**MS12-030** **için** **Notlar**

<sup>[1]</sup>Microsoft Excel 2007 için, müşterilerin bu bültende açıklanan güvenlik açıklarına karşı korunmak üzere güvenlik güncelleştirmesi paketi KB2597161'in yanı sıra Microsoft Office Uyumluluk Paketi (KB2597162) güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

<sup>[2]</sup>Bu güncelleştirme yüklenmeden önce, Microsoft Excel Viewer desteklenen bir hizmet paketi düzeyine (Excel Viewer 2007 Service Pack 2 veya Excel Viewer 2007 Service Pack 3) yükseltilmelidir. Desteklenen Office görüntüleyicileri hakkında bilgi için, bkz. [Microsoft Bilgi Bankası makalesi 979860](http://support.microsoft.com/kb/979860).

**MS12-034** **için** **Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

#### Microsoft Geliştirici Araçları ve Yazılımları

 
<table style="border:1px solid black;">
<tr>
<th colspan="2">
Microsoft Silverlight 4
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
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
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
Mac üzerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b)  
(KB2690729)  
(Kritik)  
Tüm desteklenen Microsoft Windows istemci sürümleri üzerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b)  
(KB2690729)  
(Kritik)  
Tüm desteklenen Microsoft Windows sunucu sürümleri üzerine yüklendiğinde [Microsoft Silverlight 4](http://www.microsoft.com/downloads/details.aspx?familyid=8ea4fc68-7b03-43f6-bc41-af47e7aa8c7b)  
(KB2690729)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Microsoft Silverlight 5
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS12-034**](http://go.microsoft.com/fwlink/?linkid=251038)
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
Microsoft Silverlight 5
</td>
<td style="border:1px solid black;">
Mac üzerine yüklendiğinde [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63)  
(KB2636927)  
(Kritik)  
Tüm desteklenen Microsoft Windows istemci sürümleri üzerine yüklendiğinde [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63)  
(KB2636927)  
(Kritik)  
Tüm desteklenen Microsoft Windows sunucu sürümleri üzerine yüklendiğinde [Microsoft Silverlight 5](http://www.microsoft.com/downloads/details.aspx?familyid=fb1258e2-f3df-4a3d-b809-abec619a0c63)  
(KB2636927)  
(Kritik)
</td>
</tr>
</table>
 
**MS12-034** **için** **Not**

Aynı bülten tanımlayıcısı altındaki diğer güncelleştirme dosyaları için, **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı bu bölümdeki diğer yazılım kategorilerine de bakın. Bu bülten birden çok yazılım kategorisini kapsar.

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

-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-029'da açıklanan sorunu bildirdikleri için
-   [Omair](http://krash.in/), MS12-030'da açıklanan iki sorunu bildirdiği için
-   Omair, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-030'da açıklanan sorunu bildirdikleri için
-   Sean Larsson ve Jun Mao, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-030'da açıklanan iki sorunu bildirdikleri için
-   [TippingPoint](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışan anonim bir araştırmacı, MS12-030'da açıklanan sorunu bildirdikleri için
-   Luigi Auriemma, [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-031'de açıklanan sorunu bildirdikleri için
-   [INFIGO IS](http://www.infigo.hr/) için çalışan Bojan Zdrnja, MS12-032'de açıklanan sorunu bildirdiği için
-   [Genesys Telecommunications](http://www.genesyslab.com/) için çalışan Anatoliy Glagolev, MS12-032'de açıklanan sorunu bildirdiği için
-   Alin Rad Pop, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS12-034'te açıklanan sorunu bildirdikleri için
-   Vitaliy Toropov, [Tipping Point](http://www.tippingpoint.com/) bünyesindeki [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS12-034'te açıklanan sorunu bildirdikleri için
-   [Omair](http://krash.in/), MS12-034'te açıklanan sorunu bildirdiği için
-   Anonim bir araştırmacı, [Verisign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-034'te açıklanan sorunu bildirdikleri için
-   Anonim bir araştırmacı, [Verisign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışarak MS12-034'te açıklanan sorunu bildirdikleri için
-   [MWR InfoSecurity](http://www.mwrinfosecurity.com/) için çalışan Alex Plaskett, MS12-034'te açıklanan sorunu bildirdiği için
-   [Azimuth Security](http://www.azimuthsecurity.com/) için çalışan Tarjei Mandt, MS12-034'te açıklanan sorunu bildirdiği için
-   [Core Security Technologies](http://www.coresecurity.com/) için çalışan Nicolas Economou, MS12-034'te açıklanan sorunu bildirdiği için
-   Symantec için çalışan Geoff McDonald, MS12-034'te açıklanan sorunu bildirdiği için
-   h4ckmp, MS12-034'te açıklanan sorunu bildirdiği için
-   [Context Information Security](http://www.contextis.co.uk/) için çalışan James Forshaw, MS12-035'te açıklanan iki sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   BT uzmanları için güvenlik çözümleri: [TechNet Security Sitesinin Sorun Giderme ve Destek Bölümü](http://technet.microsoft.com/security/bb980617.aspx)
-   Windows çalışan bilgisayarınızın virüslere ve kötü amaçlı yazılımlara karşı korunmasına yardım edin: [Virüs ve Güvenlik Çözüm Merkezi](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Ülkenize göre yerel destek: [Uluslararası Destek](http://support.microsoft.com/common/international.aspx)

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (8 Mayıs 2012): Bülten Özeti yayımlandı.
-   V1.1 (9 Mayıs 2012): **Yararlanma Dizini**'ndeki CVE-2012-1847 başlığı düzeltildi.
-   V2.0 (11 Mayıs 2012): MS12-035'te, Windows Server 2003 Service Pack 2 dışında Microsoft .NET Framework 1.1 Service Pack 1'in çalıştığı tüm desteklenen sistemler için güvenlik güncelleştirmesi numarası KB2656353 olarak düzeltildi. Güvenlik güncelleştirmesinin dosyalarında değişiklik yapılmamıştır. Bu güncelleştirmeyi başarıyla yüklemiş olan müşterilerin herhangi bir işlem gerçekleştirmeleri gerekmez.
-   V2.1 (22 Mayıs 2012): MS12-034'te, Windows Server 2008 ve Windows Server 2008 R2 için güvenlik güncelleştirmesi KB2660649'a yönelik dipnotlar eklendi. Güvenlik güncelleştirmesinin dosyalarında değişiklik yapılmamıştır. Bu güncelleştirmeyi başarıyla yüklemiş olan müşterilerin herhangi bir işlem gerçekleştirmeleri gerekmez.

*Built at 2014-04-18T01:50:00Z-07:00*
