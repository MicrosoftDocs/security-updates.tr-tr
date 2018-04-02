---
TOCTitle: 'MS08-JAN'
Title: Microsoft Güvenlik Bülteni Ocak 2008 Özeti
ms:assetid: 'ms08-jan'
ms:contentKeyID: 61235804
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-jan(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Ocak 2008 Özeti
==========================================

Yayım Tarihi: 8 Ocak 2008 Salı | Güncelleştirme Tarihi: 25 Ocak 2008 Cuma

**Sürüm:** 1.2

Bu bülten özetinde Ocak 2008'de yayımlanan güvenlik bültenleri listelenir.

Ocak 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 3 Ocak 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 9 Ocak 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Ocak Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357213&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (1)
----------

<span></span>
| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-001                                                                                                                                                                                                                                                                                                                                                                                    |
|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows TCP/IP'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (941644)**](http://go.microsoft.com/fwlink/?linkid=104919)                                                                                                                                                                                                                                                                           |
| **Yürütmeyle İlgili Özet**   | Bu kritik güvenlik güncelleştirmesi İletim Denetimi Protokolü/Internet Protokolü (TCP/IP) işlemlerindeki özel olarak bildirilen iki güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                 |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                               |
| **Etkilenen Yazılımlar**     | **Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                              |

Önemli (1)
----------

<span></span>
| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-002                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**LSASS'deki Güvenlik Açığı Yerel Olarak Ayrıcalık Yükselmesine İzin Verebilir (943485)**](http://go.microsoft.com/fwlink/?linkid=104921)                                                                                                                                                                                                                                                                                                                                                                                  |
| **Yürütmeyle İlgili Özet**   | Bu önemli güncelleştirme Microsoft Windows Yerel Güvenlik Yetkilisi Alt Sistemi Hizmeti'ndeki (LSASS) özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı bir saldırganın yükseltilmiş ayrıcalıklarla rasgele kod çalıştırılmasına izin verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Güvenlik Açığının Etkisi** | Yerel Olarak Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                    |
| **Etkilenen Yazılımlar**     | **Windows. **Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                   |

Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları
--------------------------------------------------

<span></span>
**Bu tabloyu nasıl kullanacağım?**  

Bu tabloyu, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip gereken güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Bir yazılım programı veya bileşenle birlikte güvenlik açığının etkisi de listelenmiş ve kullanılabilir yazılım güncelleştirmesine köprü de sağlanmıştır.

**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.

**Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları**

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Ayrıntılar        
</th>
<th style="border:1px solid black;" >
Ayrıntılar        
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-001**](http://go.microsoft.com/fwlink/?linkid=104919)
</td>
<td style="border:1px solid black;">
[**MS08-002**](http://go.microsoft.com/fwlink/?linkid=104921)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**En Yüksek Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="3">
Windows İşletim Sistemi
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Orta](http://www.microsoft.com/downloads/details.aspx?familyid=980f5457-c7b5-421c-8643-0e57429ec156)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=7956632e-17d9-4876-8340-84fe3e43e5cc)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=0a766242-2342-4fa0-9b66-8953c54a2211)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=6a4cf182-8e36-490e-aefe-edb7b3a0df9c)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=2e8bc7d5-fe81-4ed5-9efa-360738d160ee)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=51fc657b-2b4a-4725-a744-d279e027c4a5)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=fda060a5-9a1e-4036-9899-13eb61fdd8be)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=12397b47-b18f-4d4d-b8d7-adec8ff310d5)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=19d993f9-06dd-4dc4-b0cc-c59e822eb8fa)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=f19fd790-a4e6-4a8a-8077-d1bbfe37ecca)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=2c2264f7-ebbb-40ab-9dbf-9b4e313665a7)
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=0382a195-aa3d-409b-8a79-9fe61588d8a9)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Small Business Server 2003 Service Pack 1, Windows Small Business Server 2003 R2, Windows Small Business Server 2003 R2 Service Pack 2 ve Windows Home Server
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=fda060a5-9a1e-4036-9899-13eb61fdd8be)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=23c0e03a-db66-4618-bce0-af55e5c1b067)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=5f6a37b1-c604-47c9-932f-485db2eda133)
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 

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

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Yüksek Öncelikli Güncelleştirmeler

Bu ay için:

-   Microsoft, Microsoft Update (MU) ve Windows Server Update Services (WSUS) hizmetinde **güvenlikle ilgili olmayan**, yüksek öncelikli beş güncelleştirme yayımladı.
-   Microsoft, Windows Update (WU) ve WSUS sitelerinde Windows için **güvenlikle ilgili olmayan**, yüksek öncelikli iki güncelleştirme yayımladı.

Bu bilgiler **yalnızca** güvenlik bülteni özetiyle aynı günde yayımlanan Microsoft Update, Windows Update ve Windows Server Update Services hizmetlerindeki **güvenlikle ilgili olmayan**, yüksek öncelikli güncelleştirmeler için geçerlidir. Diğer günlerde yayımlanan **güvenlikle ilgili olmayan** güncelleştirmeler için bilgi **sağlanmamaktadır**.

#### Güvenlik Stratejileri ve Topluluğu

**Güncelleştirme Yönetim Stratejileri**

[Security Guidance for Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) Web sitesi, güvenlik güncelleştirmelerini uygulamayla ilgili Microsoft'un en iyi uygulama önerilerini sağlar.

**Diğer Güvenlik Güncelleştirmelerini Edinme**

Diğer güvenlik sorunlarıyla ilgili güncelleştirmeler aşağıdaki konumlardan edinilebilir:

-   Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.
-   Tüketici platformlarına yönelik güncelleştirmeler [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) Web sitesinden edinilebilir.
-   Windows Update sitesinde bu ay için sunulan güvenlik güncelleştirmelerini, Yükleme Merkezi'nden Güvenlik ve Kritik Sürümler ISO CD'si Yansıması dosyaları olarak edinebilirsiniz. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Topluluğu**

Güvenliği geliştirmeyi ve BT altyapınızı en iyi duruma getirmeyi öğrenin; ayrıca [IT Pro Security Topluluğu](http://go.microsoft.com/fwlink/?linkid=21164)'nda güvenlik konularında diğer BT Uzmanlarının çalışmalarına katılın.

#### İlgili Kaynaklar

Microsoft, müşterilerimizi korumamıza yardım etmek için bizimle işbirliği yapan aşağıdaki kişi ve kuruluşlara [teşekkür eder](http://go.microsoft.com/fwlink/?linkid=21127):

-   [IBM Internet Security Systems X-Force](http://www.iss.net/) için çalışan Alex Wheeler ve Ryan Smith, [MS08-001](http://go.microsoft.com/fwlink/?linkid=104919)'de açıklanan sorunu bildirdikleri için
-   [IBM Internet Security Systems X-Force](http://www.iss.net/) için çalışan Alex Wheeler ve Ryan Smith, [MS08-001](http://go.microsoft.com/fwlink/?linkid=104919)'de açıklanan sorunu bildirdikleri için
-   [SkyRecon](http://www.skyrecon.com/) için çalışan Thomas Garnier, [MS08-002](http://go.microsoft.com/fwlink/?linkid=104921)'de açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (8 Ocak 2008): Bülten özeti yayımlandı.
-   V1.1 (23 Ocak 2008): Bülten özeti, MS08-001 numaralı bülten için etkilenen yazılım olarak Windows Small Business Server 2003 Service Pack 2 eklenerek güncelleştirildi.
-   V1.2 (25 Ocak 2008): Bülten özeti, MS08-001 numaralı bülten için etkilenen yazılım olarak Windows Small Business Server 2003 Service Pack 1, Windows Small Business Server 2003 R2, Windows Small Business Server 2003 R2 Service Pack 2 ve Windows Home Server eklenerek güncelleştirildi.

*Built at 2014-04-18T01:50:00Z-07:00*
