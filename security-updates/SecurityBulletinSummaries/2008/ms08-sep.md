---
TOCTitle: 'MS08-SEP'
Title: Microsoft Güvenlik Bülteni Eylül 2008 Özeti
ms:assetid: 'ms08-sep'
ms:contentKeyID: 61235811
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Eylül 2008 Özeti
===========================================

Yayım Tarihi: 9 Eylül 2008 Salı | Güncelleştirme Tarihi: 9 Aralık 2008 Salı

**Sürüm:** 3.0

Bu bülten özetinde Eylül 2008'de yayımlanan güvenlik bültenleri listelenir.

Eylül 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 4 Eylül 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 10 Eylül 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirmektedir. [Eylül Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374633&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (4)
----------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows Media Player'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (954154)**](http://go.microsoft.com/fwlink/?linkid=121739)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Windows Media Player'da özel hazırlanmış bir ses dosyası için Windows Media sunucusundan akış sağlandığında uzaktan kod yürütülmesine neden olabileceği özel olarak bildirilen bir güvenlik açığını giderir. Kullanıcı yönetimsel haklarla oturum açtıysa, bu güvenlik açığından başarıyla yararlanan bir saldırgan etkilenen sistemin denetimini tümüyle ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-052                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**GDI+ Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (954593)**](http://go.microsoft.com/fwlink/?linkid=125468)                                                                                                                                                                                                                                                                                                                                                                                         |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Windows GDI+ uygulamasındaki özel olarak bildirilen birkaç güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir resim dosyasını etkilenen yazılımlardan birini kullanarak açarsa veya özel hazırlanmış içeriğe sahip bir Web sitesine gözatarsa uzaktan kod yürütülmesine izin verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                           |
| **Etkilenen Yazılımlar**     | **Microsoft Windows, Internet Explorer, .NET Framework, Office, SQL Server, Visual Studio.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                             |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-053                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows Media Encoder 9'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (954156)**](http://go.microsoft.com/fwlink/?linkid=123091)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Windows Media Encoder 9 Series'deki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel olarak hazırlanmış bir Web sayfasını görüntülerse uzaktan kod yürütülmesine olanak verebilir. Kullanıcı yönetimsel haklarla oturum açtıysa, bu güvenlik açığından başarıyla yararlanan bir saldırgan etkilenen sistemin denetimini tümüyle ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-055                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Office'teki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (955047)**](http://go.microsoft.com/fwlink/?linkid=125229)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir OneNote URL'sini tıklatırsa uzaktan kod yürütülmesine izin verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme genelde yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

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
</tr>
<tr>
<th colspan="4">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a860d2d9-653d-4ddb-bbff-323d3ccdb866)  
(KB938464)  
(Kritik)  
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c7cbcd19-acc1-4a89-adfa-99b2f431510d)  
(KB947739)  
(Önem derecesi yok)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6013f866-3ea1-4672-b1bf-e516204c3a7a)  
(KB947742)  
(Önem derecesi yok)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?familyid=7f1cd013-2c4b-4582-9114-cb840a96124a)  
(KB947746)  
(Önem derecesi yok)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=215b73a3-46ab-44a8-a0fb-6d37bd1c39b8)  
(KB947748)  
(Önem derecesi yok)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=0cabfbc0-db5d-4a6a-a4cd-e6df89ac2b25)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=d5891180-5dd1-49ec-bcc6-3030a544202c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e0bd6fbe-f46e-4961-9a79-49ec77d39439)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=57bcb3c2-49d3-4f18-8d03-36abd03d7403)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=caf8a45e-a9f8-4e91-98fd-87eddbeae64c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5d26771-1f49-4bbf-902c-bf92e527cadb)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=18efea9e-b103-46de-90d9-5e295854cec3)  
(Kritik)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ebc1737c-6e78-4244-a1b2-a56d031f16e9)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ac03f138-eca4-46e1-9782-e811820e547f)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=54ce1080-94cf-4e4f-8e09-a7dbab2757c5)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=93f1451b-5b62-47e5-8f0c-b720b957999a)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=c83011cd-90b8-494c-9cad-fa055e101992)  
(Orta)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=d8f1b782-136b-443f-b5f2-63aa4d1fd94a)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=14e99f8a-cdd4-40d7-8cfc-73ae6bd6dfad)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=2f4118fd-1ffb-46da-b922-cd4ca4f9d84e)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=16f3ad21-ed77-4c32-93df-3b650b2b32a5)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=334352e7-d41f-494f-866d-f1f1745ffd17)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=aa47d016-f5c9-4586-8876-f1f4f255f54d)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Kritik)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=54d1279a-7f26-4727-a39d-5505bcd4fc53)  
(Kritik)
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://go.microsoft.com/fwlink/?linkid=121739)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
32-bit sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=72fc6028-6af4-44ec-8d2a-28c53807d6bc)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=23bd3be5-cc66-46f8-9420-49d65d8afe1d)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=3906512b-26db-473e-b522-3883ff34a21c)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=7f1e0f05-6c9d-4ad1-9b19-50ee4fa7bd7e)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9 Series](http://www.microsoft.com/downloads/details.aspx?familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Orta)  
[Windows Media Encoder 9 Series x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=e30f9427-26d0-4e86-b9b8-bc637c3b5734)\*  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=5159bdba-3825-4816-a2be-ab035332b9e2)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008 çalışan bir sistem Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmişse, sistemde bu güvenlik açıklarından etkilenen dosyalar olsa da, bu güncelleştirmelerle giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Ancak, güncelleştirilmiş dosyalar sisteminizde bulunan dosyalardan daha yeni oldukları (sürüm numaraları daha büyük olduğu) için, etkilenen dosyaların bulunduğu kullanıcılara bu güncelleştirme yine de önerilir. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 ve Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Önemli)  
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Önemli)  
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi ve 2007 Microsoft Office Sistemi Service Pack 1
</td>
<td style="border:1px solid black;">
[2007 Microsoft Office Sistemi](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Önemli)  
[2007 Microsoft Office Sistemi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Önemli)
</td>
<td style="border:1px solid black;">
[2007 Microsoft Office Sistemi](http://www.microsoft.com/downloads/details.aspx?familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Önemli)  
[2007 Microsoft Office Sistemi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Önemli)
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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
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
Microsoft Office Project 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a6d9d3ef-f087-4f61-9ec1-522b7d4b9c48)  
(KB954479)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Word Viewer 2003, Microsoft Word Viewer 2003 Service Pack 3, Microsoft Office Excel Viewer 2003, Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer, Microsoft Word Viewer 2003, Microsoft Word Viewer 2003 Service Pack 3, Microsoft Office Excel Viewer 2003, Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office PowerPoint Viewer 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=cd503f08-1831-45ff-bdf4-dd918ca40505)  
(KB956500)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer, Microsoft Office PowerPoint Viewer 2007, Microsoft Office PowerPoint Viewer 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer, Microsoft Office PowerPoint Viewer 2007, Microsoft Office PowerPoint Viewer 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Web ve Microsoft Expression Web 2
</td>
<td style="border:1px solid black;">
[Microsoft Expression Web ve Microsoft Expression Web 2](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Groove 2007 ve Microsoft Office Groove 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Groove 2007 ve Microsoft Office Groove 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?familyid=eb0d224e-a517-40d9-9fc6-2345fa12a841)  
(KB956483)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Digital Image Suite 2006
</td>
<td style="border:1px solid black;">
[Microsoft Digital Image Suite 2006](http://www.microsoft.com/downloads/details.aspx?familyid=04afd760-8173-4069-9e82-d3bf053d9eae)  
(KB955992)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office OneNote 2007
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office OneNote 2007](http://www.microsoft.com/downloads/details.aspx?familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Kritik)  
[Microsoft Office OneNote 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Kritik)
</td>
</tr>
</table>
 
\*Bu etkilenen yazılımlara yönelik güncelleştirme, Microsoft Office XP Service Pack 3 güncelleştirmesiyle aynıdır.

\*\*Bu etkilenen yazılımlara yönelik güncelleştirme, Microsoft Office 2003 Service Pack 2 ve Microsoft Office 2003 Service Pack 3 güncelleştirmesiyle aynıdır.

\*\*\*\*Bu etkilenen yazılımlara yönelik güncelleştirme, 2007 Microsoft Office Sistemi ve 2007 Microsoft Office Sistemi Service Pack 1 güncelleştirmesiyle aynıdır.

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
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2000 Reporting Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
Uygulanamaz  
QFE güncelleştirmesi:  
[SQL Server 2000 Reporting Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5f9e7f78-7439-414b-a9dc-a779b89427db)  
(KB954609)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritik)  
QFE güncelleştirmesi:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritik)  
QFE güncelleştirmesi:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritik)  
QFE güncelleştirmesi:  
[Itanium tabanlı sistemler için SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritik)
</td>
</tr>
</table>
 

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
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7848a652-4025-44bb-9c98-37a078b56d01)  
(KB947736)  
(Önem derecesi yok)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9bc1e8f8-6c30-4aa0-90f5-fbb0ad5fd90e)  
(KB947737)  
(Önem derecesi yok)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a7bf790b-3249-4ee8-9440-fa911ebbc08a)  
(KB947738)  
(Önem derecesi yok)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?familyid=a8c80b29-6d00-4949-a005-5d706122919a)  
(KB952241)  
(Önem derecesi yok)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=82833f27-081d-4b72-83ef-2836360a904d)  
(KB954765)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?familyid=6ae0aa19-3e6c-474c-9d57-05b2347456b1)  
(KB954766)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerine yüklendiğinde [Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1f4371b9-b8be-4455-94d2-2304ee340543)  
(KB955368)  
(Önem derecesi yok)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerine yüklendiğinde [Microsoft Visual FoxPro 9.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=49b21e30-722d-446e-9020-aceb3870db69)  
(KB955369)  
(Önem derecesi yok)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerine yüklendiğinde [Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36957f47-9d8b-477d-bd60-5959e5a2eafa)  
(KB955370)  
(Önem derecesi yok)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Platform SDK Redistributable: GDI+
</td>
<td style="border:1px solid black;">
[Microsoft Platform SDK Redistributable: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(Önem derecesi yok)
</td>
</tr>
</table>
 

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
Microsoft Forefront Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bültenin En Yüksek Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerine yüklendiğinde [Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?familyid=1eb1a79f-44ca-499e-90bb-ac51894e9d1e)  
(KB957177)  
(Önemli)
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

-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Greg MacManus, MS08-052'de açıklanan sorunu bildirdiği için
-   Fortinet bünyesindeki [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) için çalışan Bing Liu, MS08-052'de açıklanan sorunu bildirdiği için
-   [NGSSoftware](http://www.ngssoftware.com/) için çalışan Peter Winter-Smith ve Ivan Fratric, [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-052'de açıklanan sorunu bildirdikleri için
-   [Vulnerability Research Team, Assurent Secure Technologies](http://www.assurent.com/), MS08-052'de açıklanan sorunu bildirdikleri için
-   [Zero Day Initiative](http://www.zerodayinitiative.com/) için çalışan anonim bir araştırmacı, MS08-052'de açıklanan sorunu bildirdiği için
-   [Bach Khoa Internetwork Security Center (BKIS) Hanoi University of Technology (Vietnam)](http://security.bkis.vn/) için çalışan Nguyen Minh Duc ve Le Manh Tung, MS08-053'te açıklanan sorunu bildirdikleri için
-   [Insomnia Security](http://www.insomniasec.com/) için çalışan Brett Moore, MS08-055'te açıklanan sorunu bildirdikleri için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (9 Eylül 2008): Bülten özeti yayımlandı.
-   V2.0 (9 Eylül 2008): Bülten özeti, MS08-052 için Etkilenen Yazılımlar bölümüne Microsoft Office Project 2002 Service Pack 2, Microsoft Office 2003 için tüm Office Viewer yazılımları ve 2007 Microsoft Office Sistemi için tüm Office Viewer yazılımları eklenerek güncelleştirildi.
-   V2.1 (17 Eylül 2008): Bülten özeti, Etkilenen Yazılımlar tablosundaki Microsoft Office Project 2002 Service Pack 2 girdisi Microsoft Office Project 2002 Service Pack 1 olarak değiştirilerek güncelleştirildi. Bu yalnızca bir ad değişikliğidir. İkili dosyalarda veya algılamada değişiklik yapılmamıştır.
-   V2.2 (29 Ekim 2008): Bülten özeti, MS08-052 için etkilenen yazılım olarak listelenen Microsoft Visio 2003 Viewer, Microsoft Visio 2007 Viewer ve Microsoft Visio 2007 Viewer Service Pack 1 kaldırılarak güncelleştirildi.
-   V3.0 (9 Aralık 2008): Bülten özeti Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi ve Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1, Microsoft Expression Web ve Microsoft Expression Web 2 ve Microsoft Office Groove 2007 ve Microsoft Office Groove 2007 Service Pack 1 yazılımlarını MS08-052 için etkilenen yazılımlar olarak eklemek amacıyla güncelleştirildi.

*Built at 2014-04-18T01:50:00Z-07:00*
