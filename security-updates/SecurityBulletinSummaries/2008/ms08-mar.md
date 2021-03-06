---
TOCTitle: 'MS08-MAR'
Title: Microsoft Güvenlik Bülteni Mart 2008 Özeti
ms:assetid: 'ms08-mar'
ms:contentKeyID: 61235807
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Mart 2008 Özeti
==========================================

Yayım Tarihi: 11 Mart 2008 Salı | Güncelleştirme Tarihi: 16 Nisan 2008 Çarşamba

**Sürüm:** 2.0

Bu bülten özetinde Mart 2008'de yayımlanan güvenlik bültenleri listelenir.

Mart 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 6 Mart 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 12 Mart 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Mart Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357217&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (4)
----------

<span></span>
| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-014                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (949029)**](http://go.microsoft.com/fwlink/?linkid=112111)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Excel dosyasını Microsoft Office Excel'de açarsa uzaktan kod yürütülmesine izin verebileceği genel ve özel olarak bildirilen birkaç güvenlik açığını giderir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-015                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Outlook'taki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (949031)**](http://go.microsoft.com/fwlink/?linkid=112113)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Office Outlook'taki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, Outlook özel hazırlanmış bir mailto URI'sı geçirirse uzaktan kod yürütülmesine olanak verebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. Bu güvenlik açığından Outlook önizleme bölmesi aracılığıyla bir e-posta görüntülenerek yararlanılamaz. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Etkilenen Yazılımlar**     | **Microsoft Office. **Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-016                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Office'teki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (949030)**](http://go.microsoft.com/fwlink/?linkid=112112)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı hatalı biçimlendirilmiş bir Office dosyasını Microsoft Office'te açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen iki güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-017                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Office Web Bileşenleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (933103)**](http://go.microsoft.com/fwlink/?linkid=112114)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Yürütmeyle İlgili Özet**   | Bu kritik güncelleştirme Microsoft Office Web Bileşenleri'ndeki özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel olarak hazırlanmış bir Web sayfasını görüntülerse uzaktan kod yürütülmesine olanak verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Etkilenen Yazılımlar**     | **Microsoft Office Web Bileşenleri.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları
--------------------------------------------------

<span></span>
**Bu tabloyu nasıl kullanabilirim?**  

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
[**MS08-014**](http://go.microsoft.com/fwlink/?linkid=112111)
</td>
<td style="border:1px solid black;">
[**MS08-015**](http://go.microsoft.com/fwlink/?linkid=112113)
</td>
<td style="border:1px solid black;">
[**MS08-016**](http://go.microsoft.com/fwlink/?linkid=112112)
</td>
<td style="border:1px solid black;">
[**MS08-017**](http://go.microsoft.com/fwlink/?linkid=112114)
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
<th colspan="5">
Office Paketleri ve Yazılımları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=72735aa1-e22c-40ed-8c79-38fba89979aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9cf8aafa-71a5-4017-b53c-4e80ef6e1188)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=f7f90c30-1bfd-406b-a77f-612443e30185)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=907f96d5-d1e9-4471-b41c-3ac811e63038)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=296e5f2c-f594-41c8-a20a-3e4c40ae3948)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=280bb2ac-b21a-46b5-8751-5a50fbebf107)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=9f25922c-d3c2-4ef1-b164-8a21a77d29aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel 2007
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=e7634cb5-9531-4284-9554-4168fc488e0c)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=e9251d71-9098-4125-ae91-7d4c83ea58ad)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=714a49cd-5bca-4719-96a1-e1077f279533)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2002 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=59853687-d885-4059-9460-ee403855dbd8)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Outlook 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=fccc7c4c-8496-4682-bd46-6590503c1bf2)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Outlook 2007
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=4e2baf00-88eb-4eb6-961a-54245b363c21)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=95dceb37-b35f-46db-b280-db0f3b298aa9)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2008
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=8fe8c32a-6d7a-482b-97c6-42562f089ee4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Diğer Yazılımlar
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB931660)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=806c654a-35e3-4385-855a-4b803249bfcf)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB932031)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=f54d2a5e-c0ed-4f70-9746-38dd61c8e9d7)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=d71b23fa-a873-406d-bad7-e38e565dee39)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=2fe10ccd-40cb-4090-b83d-eae3d4eca174)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)   
**<sup>[2]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=5fddd54f-7a33-4ea3-b68d-b96a9bae509d)   
**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=71de76ba-b62c-4a7a-a78a-9317f5255b13)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Bileşenleri 2000  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=526d87bd-c3da-412e-8765-c15987ae9b01)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2002 Service Pack 1  
(KB933367)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 Service Pack 1  
(KB933369)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft BizTalk Server 2000  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft BizTalk Server 2002  
(KB939714)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Commerce Server 2000  
(KB941305)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Security and Acceleration Server 2000 Service Pack 2  
(KB948257)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
</table>
 
**Notlar**

**<sup>[1]</sup>** Bu yazılım için kullanılabilen bir güvenlik güncelleştirmesi bulunmaktadır. Ayrıntılı bilgi için, etkilenen yazılım veya bileşene ve uygun güvenlik bültenine tablodan bakın.** **

**<sup>[2]</sup>** Bu güvenlik güncelleştirmesi Microsoft BizTalk Server 2000 ile ilişkilidir. Ayrıntılı bilgi için ilgili güvenlik bültenine bakın.

**<sup>[3]</sup>** Bu güvenlik güncelleştirmesi Microsoft BizTalk Server 2002 ile ilişkilidir. Ayrıntılı bilgi için ilgili güvenlik bültenine bakın.

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

-   Microsoft, Microsoft Update (MU) ve Windows Server Update Services (WSUS) hizmetinde **güvenlikle ilgili olmayan**, yüksek öncelikli iki güncelleştirme yayımladı.
-   Microsoft, Windows Update (WU) ve WSUS sitelerinde Windows için **güvenlikle ilgili olmayan**, yüksek öncelikli üç güncelleştirme yayımladı.

Bu bilgiler **yalnızca** güvenlik bülteni özetiyle aynı günde yayımlanan Microsoft Update, Windows Update ve Windows Server Update Services hizmetlerindeki **güvenlikle ilgili olmayan**, yüksek öncelikli güncelleştirmeler için geçerlidir. Diğer günlerde yayımlanan **güvenlikle ilgili olmayan** güncelleştirmeler için bilgi **sağlanmamaktadır**.

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

-   [SAIC](http://www.saic.com/) için çalışan Mike Scott, MS08-014'te açıklanan sorunu bildirdiği için
-   [VeriSign](http://www.verisign.com/) için çalışan Matt Richard, MS08-014'te açıklanan sorunu bildirdiği için
-   [IDefense Labs](http://labs.idefense.com/) için çalışan Greg MacManus, MS08-014'te açıklanan sorunu bildirdiği için
-   [JFE Systems](http://www.jfe-systems.com/) için çalışan Yoshiya Sasaki, MS08-014'te açıklanan sorunu bildirdiği için
-   [Fortinet](http://www.fortinet.com/) için çalışan Bing Liu, MS08-014'te açıklanan sorunu bildirdiği için
-   [iDefense Labs](http://labs.idefense.com/), MS08-014'te açıklanan sorunu bildirdikleri için
-   [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) için çalışan Cody Pierce, MS08-014'te açıklanan sorunu bildirdiği için
-   [Websense Security Labs](http://www.websense.com/) için çalışan Moti Joseph ve Dan Hubbard, MS08-014'te açıklanan sorunu bildirdikleri için
-   [IDefense Labs](http://labs.idefense.com/) için çalışan Greg MacManus, MS08-015'te açıklanan sorunu bildirdiği için
-   [Zero Day Initiative (ZDI)](http://www.zerodayinitiative.com/) için çalışan Arnaud Dovi, MS08-016'da açıklanan sorunu bildirdiği için
-   Anonim bir kullanıcı, MS08-016'da açıklanan sorunu bildirdiği için
-   [VigilantMinds Inc.](http://www.vigilantminds.com/) için çalışan Chris Ries, MS08-017'de açıklanan sorunu bildirdiği için
-   [NCNIPC](http://www.nipc.org.cn/) için çalışan Xiao Hui, MS08-017'de açıklanan sorunu bildirdiği için
-   [Finjan](http://www.finjan.com/) için çalışan Golan Yosef, MS08-017'de açıklanan bir sorunu bildirdiği için
-   [Finjan](http://www.finjan.com/) için çalışan Yuval Ben-Itzhak, MS08-017'de açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (11 Mart 2008): Bülten özeti yayımlandı.
-   V1.1 (12 Mart 2008): Bülten özeti, BizTalk Server 2000 ve 2002 için Microsoft Office Web Bileşenleri 2000'e yönelik yeni karşıdan yükleme bağlantılarını yansıtacak biçimde güncelleştirildi.
-   V1.2 (26 Mart 2008): Bülten özeti, MS08-017 için bir bulucu eklenerek güncelleştirildi.
-   V2.0 (16 Nisan 2008): Bülten özeti, MS08-016 için Etkilenen Yazılımlar bölümüne Microsoft Office Word Viewer 2003 ve Microsoft Office Word Viewer 2003 Service Pack 3 eklenerek güncelleştirildi.

*Built at 2014-04-18T01:50:00Z-07:00*
