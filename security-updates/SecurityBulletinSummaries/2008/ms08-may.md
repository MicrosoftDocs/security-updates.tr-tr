---
TOCTitle: 'MS08-MAY'
Title: Microsoft Güvenlik Bülteni Mayıs 2008 Özeti
ms:assetid: 'ms08-may'
ms:contentKeyID: 61235808
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-may(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Mayıs 2008 Özeti
===========================================

Yayım Tarihi: 13 Mayıs 2008 Salı

**Sürüm:** 1.0

Bu bülten özetinde Mayıs 2008'de yayımlanan güvenlik bültenleri listelenir.

Mayıs 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 8 Mayıs 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 14 Mayıs 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Mayıs Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357221&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (3)
----------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-026                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Word'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (951207)**](http://go.microsoft.com/fwlink/?linkid=117295)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Word dosyasını Microsoft Word'de açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen birkaç güvenlik açığını giderir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-027                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Publisher'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (951208)**](http://go.microsoft.com/fwlink/?linkid=117907)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Publisher dosyasını Microsoft Publisher'da açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen bir güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-028                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Jet Veritabanı Altyapısındaki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (950749)**](http://go.microsoft.com/fwlink/?linkid=114750)                                                                                                                                                                                                                                                                                                                                                                                    |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Windows'da bulunan Microsoft Jet Veritabanı Altyapısı'ndaki (Jet) bir güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                 |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                              |

Orta (1)
--------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-029                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Zararlı Yazılımlara Karşı Koruma Altyapısı'ndaki Güvenlik Açıkları Hizmet Reddine Olanak Verebilir (952044)**](http://go.microsoft.com/fwlink/?linkid=117943)                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Microsoft Zararlı Yazılımlara Karşı Koruma Altyapısı'ndaki özel olarak bildirilen iki güvenlik açığını giderir. Saldırgan, hedeflenen bilgisayar sistemi tarafından alınıp Microsoft Zararlı Yazılımlara Karşı Koruma Altyapısı tarafından tarandığında hizmet reddine olanak verebilecek özel hazırlanmış bir dosya oluşturmak yoluyla bu güvenlik açıklarından yararlanabilir. Bu güvenlik açıklarından birinden başarıyla yararlanan bir saldırgan, Microsoft Zararlı Yazılımlara Karşı Koruma Altyapısı'nın yanıt vermemesine ve otomatik olarak yeniden başlatılmasına neden olabilir. |
| **En Yüksek Önem Derecesi**  | [Orta](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Güvenlik Açığının Etkisi** | Hizmet Reddi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Algılama**                 | Etkilenen yazılımlarda, güncelleştirmelerin otomatik olarak algılanmasını ve dağıtılmasını sağlayan yerleşik mekanizmalar bulunur. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Windows Live OneCare, Microsoft Antigen, Microsoft Windows Defender, Microsoft Forefront Security.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                       |

Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları
--------------------------------------------------

<span></span>
**Bu tabloyu nasıl kullanabilirim?**  

Bu tabloyu, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip gereken güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.

**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.

#### Windows İşletim Sistemi ve Sunucuları

 
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=114750"><strong>MS08-028</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=0de12d09-e675-4cf0-bc6f-e42eeb4784a1">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=114750"><strong>MS08-028</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3247433f-0aa9-49b8-9e40-c5463a95bcff">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=4915ebc4-5e7b-493e-b8c4-321d40d9a701">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=114750"><strong>MS08-028</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=86e3ed62-98f7-46ec-96ab-5e8c123b1288">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=5dfc867b-74b7-4818-9fc2-d71e7c9d2e38">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Itanium tabanlı sistemler için Windows Server 2003 SP1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=3452119b-ba4c-4272-82ec-97396b2c2c3d">Microsoft Jet 4.0 Veritabanı Altyapısı</a><br />
(Kritik)</td>
</tr>
</tbody>
</table>
 

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<caption>Microsoft Office Paketleri, Sistemleri ve Bileşenleri</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117295"><strong>MS08-026</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117907"><strong>MS08-027</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Office 2000 Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=9215ff71-38c0-416a-b89a-fe3474160f41">Microsoft Word 2000 Service Pack 3</a><br />
(KB950250)<br />
(Kritik)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=8675b9b6-fbf0-4ad2-9210-285e2cc10556">Microsoft Publisher 2000 Service Pack 3</a><br />
(KB950682)<br />
(Kritik)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Office XP Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=b348a518-221e-4567-a797-999715a8b2ef">Microsoft Word 2002 Service Pack 3</a><br />
(KB950243)<br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=df623784-6e26-42c0-9e21-e7960b849e1e">Microsoft Publisher 2002 Service Pack 3</a><br />
(KB950129)<br />
(Önemli)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Office 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bc33d144-f917-47b8-961f-744ca847e14c">Microsoft Word 2003 Service Pack 2</a><br />
(KB950241)<br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c18b060b-9828-4952-8e80-5328c0832d83">Microsoft Publisher 2003 Service Pack 2</a><br />
(KB950213)<br />
(Önemli)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Office 2003 Service Pack 3</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bc33d144-f917-47b8-961f-744ca847e14c">Microsoft Word 2003 Service Pack 3</a><br />
(KB950241)<br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=c18b060b-9828-4952-8e80-5328c0832d83">Microsoft Publisher 2003 Service Pack 3</a><br />
(KB950213)<br />
(Önemli)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">2007 Microsoft Office Sistemi</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=071ceaa2-12e3-4401-9331-2a54a93e2550">Microsoft Word 2007</a><br />
(KB950113)<br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e4b647c2-79a3-49e0-9b1d-741667fdbcca">Microsoft Publisher 2007</a><br />
(KB950114)<br />
(Önemli)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=071ceaa2-12e3-4401-9331-2a54a93e2550">Microsoft Outlook 2007</a><br />
(KB950113)<br />
(Kritik)</td>
<td style="border:1px solid black;">Yok</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">2007 Microsoft Office Sistemi Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=071ceaa2-12e3-4401-9331-2a54a93e2550">Microsoft Word 2007 Service Pack 1</a><br />
(KB950113)<br />
(Önemli)</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=e4b647c2-79a3-49e0-9b1d-741667fdbcca">Microsoft Publisher 2007 Service Pack 1</a><br />
(KB950114)<br />
(Önemli)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=071ceaa2-12e3-4401-9331-2a54a93e2550">Microsoft Outlook 2007 Service Pack 1</a><br />
(KB950113)<br />
(Kritik)</td>
<td style="border:1px solid black;">Yok</td>
</tr>
</tbody>
</table>

 
<table style="border:1px solid black;">
<caption>Mac için Microsoft Office</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117295"><strong>MS08-026</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Mac için Microsoft Office 2004</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=99f54471-ccf9-4d94-a882-a05ecd128adc">Mac için Microsoft Office 2004</a><br />
(KB952332)<br />
(Önemli)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Mac için Microsoft Office 2008</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=395d1487-a3a6-4106-a0f8-4d6e1d6d89d2">Mac için Microsoft Office 2008</a><br />
(KB952331)<br />
(Önemli)</td>
</tr>
</tbody>
</table>
 

 
<table style="border:1px solid black;">
<caption>Diğer Microsoft Office Yazılımları</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117295"><strong>MS08-026</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Kritik</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Word Viewer</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=bce7ea31-2bf0-4930-aff9-837bcc82a682">Microsoft Word Viewer 2003</a><br />
(KB950625)<br />
(Önemli)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=bce7ea31-2bf0-4930-aff9-837bcc82a682">Microsoft Word Viewer 2003 Service Pack 3</a><br />
(KB950625)<br />
(Önemli)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Office Uyumluluk Paketi</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/downloads/details.aspx?familyid=2d718f37-c5d1-4e15-a7e1-5a15fedef52f">Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi</a><br />
(KB951808)<br />
(Önemli)<br />
<br />
<a href="http://www.microsoft.com/downloads/details.aspx?familyid=2d718f37-c5d1-4e15-a7e1-5a15fedef52f">Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1</a><br />
(KB951808)<br />
(Önemli)</td>
</tr>
</tbody>
</table>
 

#### Diğer Microsoft Yazılımları

**Not** Belirtilen yazılımlarda güncelleştirmelerin otomatik olarak algılanmasını ve dağıtılmasını sağlayan yerleşik mekanizmalar bulunduğu için aşağıdaki girdilerle ilişkili karşıdan yükleme bağlantıları yoktur.

 
<table style="border:1px solid black;">
<caption>Microsoft Zararlı Yazılımlara Karşı Koruma</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Bülten Tanımlayıcısı</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=117943"><strong>MS08-029</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>En Yüksek Önem Derecesi</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140"><strong>Orta</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Live OneCare</td>
<td style="border:1px solid black;">Windows Live OneCare<br />
(Orta)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Antigen</td>
<td style="border:1px solid black;">Microsoft Antigen for Exchange<br />
(Orta)<br />
<br />
Microsoft Antigen for SMTP Gateway<br />
(Orta)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows Defender</td>
<td style="border:1px solid black;">Microsoft Windows Defender<br />
(Orta)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Forefront Security</td>
<td style="border:1px solid black;">Microsoft Forefront Client Security<br />
(Orta)<br />
<br />
Microsoft Forefront Security for Exchange Server<br />
(Orta)<br />
<br />
Microsoft Forefront Security for SharePoint<br />
(Orta)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Standalone System Sweeper</td>
<td style="border:1px solid black;">Diagnostics and Recovery Toolset 6.0 içinde bulunan Standalone System Sweeper<br />
(Düşük)</td>
</tr>
</tbody>
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

-   [iDefense Labs](http://labs.idefense.com/) için çalışan Jun Mao, MS08-026'da açıklanan sorunu bildirdiği için
-   [team509](http://www.team509.com/) için çalışan wushi ve [Zero Day Initiative](http://www.zerodayinitiative.com/), MS08-026'da açıklanan sorunu bildirdiği için
-   [Fortinet Security Research](http://www.fortinet.com/) için çalışan Cocoruder, MS08-027'de açıklanan sorunu bildirdiği için
-   [CERT/CC](http://www.cert.org/), MS08-028'de açıklanan sorunu bildirdikleri için
-   [ISC/SANS](http://isc.sans.org/), MS08-028'de açıklanan sorunu bildirdikleri için
-   [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) için çalışan Aaron Portnoy, MS08-028'de açıklanan sorunu bildirdiği için
-   [Nevis Labs](http://www.nevisnetworks.com) için çalışan SoWhat, MS08-029'da açıklanan iki sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (13 Mayıs 2008): Bülten özeti yayımlandı.

*Built at 2014-04-18T01:50:00Z-07:00*
