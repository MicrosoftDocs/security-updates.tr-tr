---
TOCTitle: 'MS08-JUN'
Title: Microsoft Güvenlik Bülteni Haziran 2008 Özeti
ms:assetid: 'ms08-jun'
ms:contentKeyID: 61235806
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Haziran 2008 Özeti
=============================================

Yayım Tarihi: 10 Haziran 2008 Salı | Güncelleştirme Tarihi: 1 Nisan 2009 Çarşamba

**Sürüm:** 2.1

Bu bülten özetinde Haziran 2008'de yayımlanan güvenlik bültenleri listelenir.

Haziran 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 5 Haziran 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 11 Haziran 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Haziran Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357225&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (3)
----------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-030                                                                                                                                                                                                                                                                                                                                                                                     |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Bluetooth Yığınındaki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (951376)**](http://go.microsoft.com/fwlink/?linkid=119619)                                                                                                                                                                                                                                                                             |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Windows'daki Bluetooth yığınında uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen bir güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                  |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                     |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-031                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Internet Explorer için Toplu Güvenlik Güncelleştirmesi (950759)**](http://go.microsoft.com/fwlink/?linkid=116367)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, özel ve genel olarak bildirilen birer güvenlik açığını giderir. Özel olarak bildirilen güvenlik açığı, Internet Explorer kullanan bir kullanıcı özel hazırlanmış bir Web sayfasını görüntülerse uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Genel olarak bildirilen güvenlik açığı, Internet Explorer kullanan bir kullanıcı özel hazırlanmış bir Web sayfasını görüntülerse uzaktan bilginin açığa çıkmasına neden olabilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Microsoft Windows, Internet Explorer.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-033                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**DirectX'teki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (951698)**](http://go.microsoft.com/fwlink/?linkid=118655)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir medya dosyasını açarsa Microsoft DirectX'te uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

Önemli <sup>[3]</sup>
------------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-034                                                                                                                                                                                                                                                                                                                                                                                   |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**WINS'deki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (948745)**](http://go.microsoft.com/fwlink/?linkid=111957)                                                                                                                                                                                                                                                                                          |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Windows Internet Ad Hizmeti'nde (WINS) ayrıcalık yükselmesine neden olabileceği özel olarak bildirilen bir güvenlik açığını giderir. Bu açıktan yerel olarak başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Böylece saldırgan program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir ya da yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                |
| **Güvenlik Açığının Etkisi** | Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                           |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                   |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-035                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Active Directory'deki Güvenlik Açığı Hizmet Reddine Olanak Verebilir (953235)**](http://go.microsoft.com/fwlink/?linkid=111953)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Windows 2000 Server, Windows Server 2003 ve Windows Server 2008 üzerinde Active Directory; Windows XP Professional ve Windows Server 2003 üzerine yüklendiğinde Active Directory Uygulama Modu (ADAM) ve Windows Server 2008 üzerine yüklendiğinde Active Directory Basit Dizin Hizmeti (AD LDS) uygulamalarında özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığından yararlanan bir saldırgan, hizmet reddi durumunun oluşmasına neden olabilir. Windows XP Professional, Windows Server 2003 ve Windows Server 2008'de bir saldırganın bu açıktan yararlanabilmesi için, geçerli oturum açma kimlik bilgilerine sahip olması gerekir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, sistemin yanıt vermemesine veya otomatik olarak yeniden başlatılmasına neden olabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Güvenlik Açığının Etkisi** | Hizmet Reddi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-036                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Kolay Genel Çok Noktaya Yayın Protokolü'ndeki (PGM) Güvenlik Açıkları Hizmet Reddine Olanak Verebilir (950762)**](http://go.microsoft.com/fwlink/?linkid=117297)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Kolay Genel Çok Noktaya Yayın Protokolü'nde (PGM) hatalı biçimlendirilmiş PGM paketleri etkilenen bir sistem tarafından alınırsa hizmet reddine olanak verebileceği özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, bir kullanıcının sisteminin yanıt vermemesine ve işlevselliğin geri yüklenebilmesi için yeniden başlatılması gerekmesine neden olabilir. Hizmet reddi güvenlik açığının, bir saldırganın kod yürütmesine veya kullanıcı haklarını yükseltmesine izin vermeyeceğini, ancak etkilenen sistemin istekleri kabul etmeyi durdurmasına neden olabileceğini unutmayın. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Güvenlik Açığının Etkisi** | Hizmet Reddi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

Orta (1)
--------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-032                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**ActiveX Kill Bitlerine Yönelik Toplu Güvenlik Güncelleştirmesi (950760)**](http://go.microsoft.com/fwlink/?linkid=116368)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Microsoft Konuşma API'sinde genel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse ve Windows'daki Konuşma Tanıma özelliği etkinleştirilmiş durumdaysa uzaktan kod yürütülmesine izin verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Güncelleştirme ayrıca BackWeb tarafından geliştirilen yazılım için bir kill biti içerir. |
| **En Yüksek Önem Derecesi**  | [Orta](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları
--------------------------------------------------

<span></span>
**Bu tabloyu nasıl kullanacağım?**  

Bu tabloyu, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip gereken güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.

**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.

#### Windows İşletim Sistemi ve Sunucuları

 
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bültenin En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=88990b23-d37f-4d02-a5a3-2ee389ade53c">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Önemli)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4c47cf8a-8100-4d43-855a-f225a3492b19">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=65640123-a9e4-455c-a51a-9df28bd2d412">DirectX 7.0</a><br />
(Kritik)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=c6a28d45-13cf-48c4-8f89-3417d552e90b">DirectX 8.1</a><br />
(Kritik)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=4dc47e04-5e95-4636-a814-3f912d961461">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cedfd988-232c-4cba-ac65-beb54b8946e0">Microsoft Windows 2000 Service Pack 4</a><br />
(Orta)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Windows 2000 Server Service Pack 4</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=aa8aa79f-c2cc-440c-9e5c-089143e6f814">Microsoft Windows 2000 Server Service Pack 4</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=53438880-9ea9-4975-9b85-2a1d3d232793">Active Directory</a><br />
(KB949014)<br />
(Önemli)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
</tr>
</tbody>
</table>

 
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bültenin En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2 ve Windows XP Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=980bb421-950f-4825-8039-44cc961a47b8">Windows XP Service Pack 2 ve Windows XP Service Pack 3</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=cc325017-3a48-4475-90e4-0c79a002fce3">Microsoft Internet Explorer 6</a><br />
(Kritik)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fbc31bde-0bf5-490c-96a8-071310d9464a">Windows Internet Explorer 7</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7aaa6427-1e22-4566-960c-836a3b9e5f36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=36b14a81-5979-4e38-9ba3-ed83dfc17adf">Windows XP Service Pack 2 ve Windows XP Service Pack 3</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2d8957c2-e473-4dca-8d68-19fdaea36e26">Windows XP Service Pack 2 ve Windows XP Service Pack 3</a><br />
(Orta)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional Service Pack 2 ve Windows XP Professional Service Pack 3</td>
<td style="border:1px solid black;">(Windows XP Service Pack 2 ve Windows XP Service Pack 3 satırına bakın)</td>
<td style="border:1px solid black;">(Windows XP Service Pack 2 ve Windows XP Service Pack 3 satırına bakın)</td>
<td style="border:1px solid black;">(Windows XP Service Pack 2 ve Windows XP Service Pack 3 satırına bakın)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=7d6aec31-cfb4-470c-983e-78c6a3ebabfe">ADAM</a><br />
(KB949269)<br />
(Orta)</td>
<td style="border:1px solid black;">(Windows XP Service Pack 2 ve Windows XP Service Pack 3 satırına bakın)</td>
<td style="border:1px solid black;">(Windows XP Service Pack 2 ve Windows XP Service Pack 3 satırına bakın)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=81ab56ca-933f-4974-a393-290a54c30a78">Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c8783cfe-9da5-4842-ab3a-1e2be4fafc47">Microsoft Internet Explorer 6</a><br />
(Kritik)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=19c0ccdc-95c9-4151-96b6-4f49b594ebe0">Windows Internet Explorer 7</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5e8e7e9d-828d-442c-acac-8d91e80dfb36">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2e0b48-1bde-4ccc-8f40-2918c2568b2b">ADAM</a><br />
(KB949269)<br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9e9d24ee-8183-428c-8067-168a8d85eaa1">Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=62874096-7d17-4116-9795-4756e2fb6dae">Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2</a><br />
(Orta)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bültenin En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=286aada6-a358-41f1-b81a-8de39b9f908a">Microsoft Internet Explorer 6</a><br />
(Orta)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=a1ae9ad2-8329-4c96-b950-7534b3287eaa">Windows Internet Explorer 7</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2274ecb2-2802-47e2-84fd-6621fcb17758">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=08fc90d5-23aa-4327-8aef-16bc5170769d">Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a4aed117-3c76-4d80-b50e-8e07e2ef2f7d">Active Directory</a><br />
(KB949014)<br />
(Orta)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=0a983ffb-4f5a-4b78-9bf5-813dcc5df8d3">ADAM</a><br />
(KB949269)<br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1e8e2faf-009f-403b-a5fe-a47cf014db3a">Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=dadead99-09cb-4f2b-850d-e98a627cb9f8">Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2</a><br />
(Düşük)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6604569a-3db0-47e7-bd30-7dfba8145386">Microsoft Internet Explorer 6</a><br />
(Orta)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=fb0c70b4-ce9f-43d6-875a-3cfd0d3a2681">Windows Internet Explorer 7</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5ba63bb7-ed6d-4c59-88b3-456eda07e190">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=71675ae8-d60a-4834-b358-2d8e761e62fc">Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8298a6e4-d3e2-48ea-ac29-aa4dc5a8ec77">Active Directory</a><br />
(KB949014)<br />
(Orta)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=334252db-4a7a-4161-bb71-2a20c0b5bd93">ADAM</a><br />
(KB949269)<br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=78bf92d8-63c4-4596-8425-8fcfea7f5582">Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=84f9b533-b0cb-46d1-b4a8-5c9469abbd22">Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Düşük)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0262beb8-1eb5-4c2d-a50a-0c6c6e0c1f61">Microsoft Internet Explorer 6</a><br />
(Orta)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=28d2913c-1c6b-4671-9892-de08698cd5a6">Windows Internet Explorer 7</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=be71c002-2f64-49e9-9f4b-ba99c4f3caf6">DirectX 9.0, DirectX 9.0a, DirectX 9.0b veya DirectX 9.0c</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=87affdc9-d9fe-413c-af30-f3d3b671ec72">Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=f6bf4b85-b91d-4378-a356-cd11f12cbbfd">Active Directory</a><br />
(KB949014)<br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5b7e94fa-22ed-4f7c-b452-647b2e620113">Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2</a><br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ac35ce19-d761-4529-9f55-1e1b5b2447ad">Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2</a><br />
(Düşük)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bültenin En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista ve Windows Vista Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6524debe-be50-44d1-8543-af0bfaf086ad">Windows Vista ve Windows Vista Service Pack 1</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6d68b39d-157f-4c3d-ac76-bc5a9386db59">Windows Internet Explorer 7</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4d4b305b-57f8-448d-92fa-3dcdd1f42ed7">DirectX 10.0</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=ef2d2a4b-4831-41be-b5d0-8df5b01fd205">Windows Vista ve Windows Vista Service Pack 1</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4af6575e-b061-45a6-b3d8-ecb32d76b2d3">Windows Vista ve Windows Vista Service Pack 1</a><br />
(Orta)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=6adee8b9-3455-4f3b-8bdd-2585c8ff83b8">Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4cf92235-861e-4b74-bee3-8e977c8688d9">Windows Internet Explorer 7</a><br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b040cfad-2290-44f4-8f5a-5d1ed98a7265">DirectX 10.0</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0839fcf4-85ca-445e-896b-f634b10b6700">Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=67576acb-9cb6-4c76-9a72-dc5e5556b658">Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1</a><br />
(Orta)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=119619"><strong>MS08-030</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116367"><strong>MS08-031</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=118655"><strong>MS08-033</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111957"><strong>MS08-034</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111953"><strong>MS08-035</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117297"><strong>MS08-036</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=116368"><strong>MS08-032</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bültenin En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Önemli</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">32-Bit Sistemler için Windows Server 2008</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=a8922e7e-9264-4e09-b8ad-c5420fed8690">Windows Internet Explorer 7</a><br />
(Orta)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c0c495f8-2a35-4638-a635-1e55dd15e062">DirectX 10.0</a><br />
(Kritik)<strong>**</strong></td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">Active Directory</a><br />
(KB949014)<br />
(Orta)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=2981156e-2e2f-469e-91be-da127d50f3fc">AD LDS</a><br />
(KB949014)<br />
(Orta)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0466a6e7-fdca-4647-af62-449e5f20d1e4">32-bit sistemler için Windows Server 2008</a><br />
(Orta)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8a507fba-8c93-4952-91e4-98e9e7affbd2">32-bit sistemler için Windows Server 2008</a><br />
(Düşük)<strong>***</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">x64 Tabanlı Sistemler için Windows Server 2008</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=05b0e838-24d7-4387-b069-2604bbcc43b9">Windows Internet Explorer 7</a><br />
(Orta)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0b70fc2e-4e80-4ae8-8682-41ea04c24e4e">DirectX 10.0</a><br />
(Kritik)<strong>**</strong></td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">Active Directory</a><br />
(KB949014)<br />
(Orta)<strong>*</strong><br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=b5cfe6f4-c5ba-4be9-a6b8-9381c40c85aa">AD LDS</a><br />
(KB949014)<br />
(Orta)<strong>*</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=304898e6-21a7-476f-b9ed-7ac0d88a91e2">x64 tabanlı sistemler için Windows Server 2008</a><br />
(Orta)<strong>**</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=1a11499d-a008-407f-9084-a5189fa27015">x64 tabanlı sistemler için Windows Server 2008</a><br />
(Düşük)<strong>***</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Itanium Tabanlı Sistemler için Windows Server 2008</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=640e1865-ebcc-4d69-a770-fd360020da1e">Windows Internet Explorer 7</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=80ec83e0-cfb8-4a5e-9254-6679a7225b83">DirectX 10.0</a><br />
(Kritik)</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;">Uygulanamaz</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8907783b-e3fe-40b2-9fc8-4937e7d58b7e">Itanium tabanlı sistemler için Windows Server 2008</a><br />
(Orta)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=59b1689c-e723-4d87-973e-4beac107a6f7">Itanium tabanlı sistemler için Windows Server 2008</a><br />
(Düşük)</td>
</tr>
</tbody>
</table>
 

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez, ancak bu güncelleştirme yine de sunulacaktır.** Windows Server 2008 çalışan bir sistem Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmişse, sistemde bu güvenlik açıklarından etkilenen dosyalar olsa da, bu güncelleştirme ile giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Ancak, güncelleştirilmiş dosyalar sisteminizde bulunan dosyalardan daha yeni oldukları (sürüm numaraları daha büyük olduğu) için, etkilenen dosyaların bulunduğu kullanıcılara bu güncelleştirme yine de önerilir. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): 2008 yılındaki Software Update Services ve Windows Server Update Services içerik değişikliklerinin açıklaması. Tüm Windows içeriği yer alır.
-   [Microsoft Windows Dışındaki Microsoft Ürünleri için Yeni, Yeniden Düzenlenen ve Yayımlanan Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

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

-   [Tipping Point](http://www.tippingpoint.com/) için çalışan Sebastian Apelt, Peter Vreugdenhil ve anonim bir araştırmacı ile [Zero Day Initiative](http://www.zerodayinitiative.com/), MS08-031'de açıklanan sorunu bildirdikleri için.
-   [IBM Internet Security Systems X-Force](http://xforce.iss.net/) araştırmacısı olan Mark Dowd, MS08-033'te açıklanan sorunu bildirdiği için.
-   [Tipping Point](http://www.tippingpoint.com/) için çalışan anonim bir araştırmacı ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS08-033'te açıklanan sorunu bildirdikleri için.
-   [Securify](http://www.securify.com/) için çalışan Alex Matthews ve John Guzik, MS08-035'te açıklanan sorunu bildirdiği için.

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (10 Haziran 2008): Bülten özeti yayımlandı.
-   V1.1 (11 Haziran 2008): Windows XP için Etkilenen Yazılımlar tablosu, MS08-030, MS08-031, MS08-032, MS08-033 ve MS08-036 için Windows XP Service Pack 2 ve Windows XP Service Pack 3 girdilerini açıklığa kavuşturmak üzere düzeltildi.
-   V2.0 (16 Temmuz 2008): MS08-033 için etkilenen yazılım olarak DirectX 9.0a eklendi.
-   V2.1 (1 Nisan 2009): MS08-032 için, Windows Server 2008 sunucu çekirdeği yüklemelerinin açıklanan güvenlik açığından etkilenmediği halde güncelleştirmenin yine de önerileceği açıklığa kavuşturuldu. Bu yalnızca bilgilendirme amaçlı bir değişikliktir. Bu tür yüklemeleri kullananların bu güncelleştirmeyi yüklemeleri gerekmemektedir.

*Built at 2014-04-18T01:50:00Z-07:00*
