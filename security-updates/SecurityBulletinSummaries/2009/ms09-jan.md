---
TOCTitle: 'MS09-JAN'
Title: Microsoft Güvenlik Bülteni Ocak 2009 Özeti
ms:assetid: 'ms09-jan'
ms:contentKeyID: 61235816
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms09-jan(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Ocak 2009 Özeti
==========================================

Yayım Tarihi: 13 Ocak 2009 Salı

**Sürüm:** 1.0

Bu bülten özetinde Ocak 2009'da yayımlanan güvenlik bültenleri listelenir.

Ocak 2009 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 8 Ocak 2009'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 14 Ocak 2009 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Ocak Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395120). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132991">MS09-001</a></td>
<td style="border:1px solid black;"><strong>SMB'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958687)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft Sunucu İleti Bloğu'ndaki (SMB) özel olarak bildirilen birkaç güvenlik açığını giderir. Güvenlik açıkları, etkilenen sistemlerde uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açıklarından başarıyla yararlanan bir saldırgan program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ yapılarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. En iyi uygulamalar, Internet'e bağlı sistemlerde olabildiğince az sayıda bağlantı noktasının açılmasını önerir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
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
  
| Bülten Kimliği                                            | Bülten Başlığı                                                               | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                                                                                                                                                                                                                                                                                                                     |  
|-----------------------------------------------------------|------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-001](http://go.microsoft.com/fwlink/?linkid=132991) | SMB'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958687) | [CVE-2008-4114](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4114) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu yalnızca bir hizmet reddi güvenlik açığıdır.                                                                                                                                                                                                                                                                                                                   |  
| [MS09-001](http://go.microsoft.com/fwlink/?linkid=132991) | SMB'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958687) | [CVE-2008-4834](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4834) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu bir uzaktan kod yürütme güvenlik açığı olmakla birlikte çalışır durumda yararlanma kodu bulunma olasılığı düşüktür. Daha fazla bilgi için, bkz. Microsoft Güvenlik Açığı Araştırma ve Savunma blogu, [SMB bülteninin dağıtımına öncelik verme](http://blogs.technet.com/swi/archive/2009/01/09/ms09-001-prioritizing-the-deployment-of-the-smb-bulletin.aspx). |  
| [MS09-001](http://go.microsoft.com/fwlink/?linkid=132991) | SMB'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958687) | [CVE-2008-4835](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4835) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bu bir uzaktan kod yürütme güvenlik açığı olmakla birlikte çalışır durumda yararlanma kodu bulunma olasılığı düşüktür. Daha fazla bilgi için, bkz. Microsoft Güvenlik Açığı Araştırma ve Savunma blogu, [SMB bülteninin dağıtımına öncelik verme](http://blogs.technet.com/swi/archive/2009/01/09/ms09-001-prioritizing-the-deployment-of-the-smb-bulletin.aspx). |
  
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
</tr>
<tr>
<th colspan="2">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-001**](http://go.microsoft.com/fwlink/?linkid=132991)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=e0678d14-c1b5-457a-8222-8e7682760ed4)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-001**](http://go.microsoft.com/fwlink/?linkid=132991)
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
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=eeafcdc5-df39-4b29-b6f1-7d32b64761e1)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=26898401-f669-4542-ad93-199ed1fe9a2a)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-001**](http://go.microsoft.com/fwlink/?linkid=132991)
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
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=588ca8e8-38a9-47ed-9c41-09aaf1022e49)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ee59441c-1e8f-4425-ae8d-dec14e7f13fb)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=caec9321-fa5b-42f0-9f26-61f673fe6eef)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="2">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-001**](http://go.microsoft.com/fwlink/?linkid=132991)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9179c463-c10a-452a-990f-b7e37cdd889b)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6b26952e-b59d-4b0f-a52d-025e45ecd233)  
(Orta)
</td>
</tr>
<tr>
<th colspan="2">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-001**](http://go.microsoft.com/fwlink/?linkid=132991)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-Bit Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=7245b411-7c9e-41e5-9841-4c586336086c)\*  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=a241eaad-95a0-442b-978f-f21a6f0c7db4)\*  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ab7c7015-20bb-4a0c-977a-969f4e2a5189)  
(Orta)
</td>
</tr>
</table>
 
**Windows Server 2008 için Notlar**

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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

-   Anonim bir araştırmacı, [Tipping Point](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS09-001'de açıklanan sorunu bildirdikleri için
-   Anonim bir araştırmacı, [Tipping Point](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS09-001'de açıklanan başka bir sorunu bildirdikleri için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (13 Ocak 2009): Bülten özeti yayımlandı.

*Built at 2014-04-18T01:50:00Z-07:00*
