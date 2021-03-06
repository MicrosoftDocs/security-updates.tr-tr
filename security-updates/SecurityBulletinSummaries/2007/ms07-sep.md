---
TOCTitle: 'MS07-SEP'
Title: Microsoft Güvenlik Bülteni Eylül 2007 Özeti
ms:assetid: 'ms07-sep'
ms:contentKeyID: 61235799
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms07-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Eylül 2007 Özeti
===========================================

Yayım Tarihi: 11 Eylül 2007 Salı | Güncelleştirme Tarihi: 12 Eylül 2007 Çarşamba

**Sürüm:** 1.1

Bu bülten özetinde Eylül 2007'de yayımlanan güvenlik bültenleri listelenir.

Eylül 2007 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 6 Eylül 2007'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 12 Eylül 2007 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirmektedir. [Eylül Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344690&eventcategory=4&culture=en-us&countrycode=us). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (1)
----------

<span></span>
| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS07-051                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Agent'taki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (938827)**](http://go.microsoft.com/fwlink/?linkid=94667)                                                                                                                                                                                                                                                                                                                                     |
| **Yürütmeyle İlgili Özet**   | Bu kritik güvenlik güncelleştirmesi, özel olarak bildirilen bir güvenlik açığını giderir. Microsoft Agent'ta, özel hazırlanmış bazı URL'leri işleme biçimi nedeniyle bir uzaktan kod yürütme güvenlik açığı bulunmaktadır. Güvenlik açığı, saldırganın etkilenen sistemde uzaktan kod yürütmesine olanak sağlayabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                      |
| **Etkilenen Yazılımlar**     | **Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                     |

Önemli <sup>[3]</sup>
------------

<span></span>
| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS07-052                                                                                                                                                                                                                                                                                                                                   |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Crystal Reports for Visual Studio'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (941522)**](http://go.microsoft.com/fwlink/?linkid=98460)                                                                                                                                                                                                           |
| **Yürütmeyle İlgili Özet**   | Bu önemli güvenlik güncelleştirmesi genel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir RPT dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                   |
| **Algılama**                 | Microsoft Baseline Security Analyzer ve Kuruluş Güncelleştirme Tarama Aracı bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                |
| **Etkilenen Yazılımlar**     | **Visual Studio.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                       |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS07-053                                                                                                                                                                                                                                                                                                                             |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows Services for UNIX'teki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (939778)**](http://go.microsoft.com/fwlink/?linkid=94467)                                                                                                                                                                                                                |
| **Yürütmeyle İlgili Özet**   | Bu önemli güvenlik güncelleştirmesi, genel olarak bildirilen bir güvenlik açığını giderir. Windows Services for UNIX 3.0, Windows Services for UNIX 3.5 ve UNIX Tabanlı Uygulamalar için Alt Sistem'de, belirli setuid ikili dosyaları çalıştırıldığında bir saldırganın ayrıcalık yükseltmesi sağlamasına olanak verebilecek bir güvenlik açığı bulunmaktadır. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                          |
| **Güvenlik Açığının Etkisi** | Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                                            |
| **Algılama**                 | Microsoft Baseline Security Analyzer ve Kuruluş Güncelleştirme Tarama Aracı bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                  |
| **Etkilenen Yazılımlar**     | **Windows Services for UNIX, UNIX Tabanlı Uygulamalar için Alt Sistem.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                           |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS07-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**MSN Messenger ve Windows Live Messenger'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (942099)**](http://go.microsoft.com/fwlink/?linkid=100148)                                                                                                                                                                                                                                                                                                                                                                                 |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi MSN Messenger ve Windows Live Messenger'daki genel olarak duyurulan bir güvenlik açığını giderir. Güvenlik açığı, bir kullanıcı saldırganın gönderdiği bir web kamerası veya videolu sohbet davetini kabul ettiğinde uzaktan kod yürütülmesine olanak verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Algılama**                 | Bu ürünler, güncelleştirmelerin otomatik algılanması ve dağıtımı için yerleşik düzenekler sağlar. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                                              |
| **Etkilenen Yazılımlar**     | **MSN Messenger, Windows Live Messenger.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                            |

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
[**MS07-051**](http://go.microsoft.com/fwlink/?linkid=94667)
</td>
<td style="border:1px solid black;">
[**MS07-052**](http://go.microsoft.com/fwlink/?linkid=98460)
</td>
<td style="border:1px solid black;">
[**MS07-053**](http://go.microsoft.com/fwlink/?linkid=94467)
</td>
<td style="border:1px solid black;">
[**MS07-054**](http://go.microsoft.com/fwlink/?linkid=100148)
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
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<th colspan="5">
Windows İşletim Sistemi
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Kritik](http://www.microsoft.com/downloads/details.aspx?familyid=7cd248ed-d154-4dce-89ef-ceefd2700965)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Windows İşletim Sistemi Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 2000 Service Pack 4 üzerinde Windows Services for UNIX 3.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 2000 Service Pack 4 üzerinde Windows Services for UNIX 3.5
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2 üzerinde Windows Services for UNIX 3.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 üzerinde Windows Services for UNIX 3.5
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2 üzerinde Windows Services for UNIX 3.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2 üzerinde Windows Services for UNIX 3.5
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2 üzerinde UNIX Tabanlı Uygulamalar için Alt Sistem
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=8ab5cc43-0b9c-45eb-aa51-47568ab6ce3f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2 üzerinde UNIX Tabanlı Uygulamalar için Alt Sistem
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=1d21e3e8-b5f6-4044-9db6-054af836492b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista üzerinde UNIX Tabanlı Uygulamalar için Alt Sistem
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=4d52e4f4-2888-42df-8163-85c648e65b29)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition üzerinde UNIX Tabanlı Uygulamalar için Alt Sistem
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=4be667cc-c239-480b-a9a0-939bcd27f0de)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Geliştirme Araçları ve Platformları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2002 Service Pack 1  
(KB937057)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=2608c83b-e1b2-4449-9a0e-1e566aac3d76)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2003  
(KB937058)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=d612ad41-5a0d-4e13-99ea-d6a5589786d6)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 Service Pack 1  
(KB937059)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=0b10b04b-932c-4bff-9cbc-b3eeb15064b1)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio 2005  
(KB937060)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=21073cc2-919c-40df-8ebb-aa3db06050d2)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio 2005 Service Pack 1  
(KB937061)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=967d43c8-efba-4221-beb0-981e7deef33a)**<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5">
Diğer Etkilenen Yazılımlar
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerinde MSN Messenger 6.2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4 üzerinde MSN Messenger 7.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista ve Windows Vista x64 Edition üzerinde MSN Messenger 6.2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista ve Windows Vista x64 Edition üzerinde MSN Messenger 7.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista ve Windows Vista x64 Edition üzerinde MSN Messenger 7.5
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista ve Windows Vista x64 Edition üzerinde Windows Live Messenger 8.0
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Önemli](http://www.microsoft.com/downloads/details.aspx?familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc&displaylang=tr)**<sup>[3]</sup>**
</td>
</tr>
</table>
 
**Notlar**

**<sup>[1]</sup>** Bu işletim sistemi için kullanılabilen bir güvenlik güncelleştirmesi bulunmaktadır. Ayrıntılı bilgi için, etkilenen yazılım veya bileşene ve uygun güvenlik bültenine tablodan bakın.** **

**<sup>[2]</sup>** Visual Studio'nun tüm sürümleri etkilenmez. Etkilenen sürümlerin tam listesi için ilgili güvenlik bültenine bakın.** **

**<sup>[3]</sup>** Bu yazılım için MSN Messenger veya Windows Live Messenger hizmetinden çevrimiçi yükseltme gerçekleştirme seçeneği de kullanılabilir. Ayrıntılı bilgi için ilgili güvenlik bültenine bakın.

Algılama ve Dağıtım Araçları ve Kılavuzu
----------------------------------------

<span></span>
**Güvenlik Merkezi**

Kuruluşunuzdaki sunuculara, masaüstü bilgisayarlara ve taşınabilir bilgisayarlara dağıtmanız gereken yazılımları ve güvenlik güncelleştirmelerini yönetin. Daha fazla bilgi için, bkz: [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171), Microsoft ürünlerinde güvenlik konusunda ek bilgi sağlar. Müşteriler, bu bilgilerin "En Son Güvenlik Güncelleştirmeleri" tıklatılarak da edinilebileceği [Evde Güvenlik](http://go.microsoft.com/fwlink/?linkid=85102) sitesini de ziyaret edebilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) ve [Office Update](http://go.microsoft.com/fwlink/?linkid=21135) sitesinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik\_düzeltme\_eki" anahtar sözcüğünü aratarak kolayca bulabilirsiniz. Son olarak, güvenlik güncelleştirmeleri Windows Update Kataloğu'ndan karşıdan yüklenebilir. Windows Update Kataloğu hakkında daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 323166](http://support.microsoft.com/kb/323166).

**Algılama ve Dağıtım Kılavuzu**

Microsoft bu ayın güvenlik güncelleştirmeleri için algılama ve dağıtım kılavuzu sağlamıştır. Bu kılavuz, ayrıca BT uzmanlarının güvenlik güncelleştirmesini dağıtmak amacıyla Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Algılama Aracı, Microsoft Systems Management Server (SMS), Genişletilmiş Güvenlik Güncelleştirmesi Envanter Aracı ve Kuruluş Güncelleştirme Tarama Aracı (EST) gibi çeşitli araçları nasıl kullanabileceklerini anlamalarına yardımcı olur. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer ve** **Kuruluş** **Güncelleştirme Tarama Aracı**

Microsoft Baseline Security Analyzer (MBSA), yöneticilerin eksik güvenlik güncelleştirmeleri ve ayrıca sık rastlanan güvenlik yapılandırması hataları için yerel ve uzak sistemleri taramasına olanak sağlar. MBSA hakkında daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

MBSA 1.2.1 belirli bir güvenlik güncelleştirmesi için algılama desteği sağlayamazsa, Microsoft ilgili güvenlik güncelleştirmesi için Kuruluş Güncelleştirme Tarama Aracı'nın (EST) özel bir sürümünü yayımlar. EST hakkında daha fazla bilgi için, [Kuruluş Güncelleştirme Tarama Aracı](http://support.microsoft.com/default.aspx?id=894193) Web sitesini ziyaret edin.

**Not** 9 Ekim 2007'den itibaren, MBSA 1.2.1 tarafından kullanılan MSSecure.XML dosyası güncelleştirilmeyecektir. Bu tarihten sonra, MBSA 1.2.1 tarafından kullanılan MSSecure.XML dosyasına yeni güvenlik güncelleştirmeleri eklenmeyecektir ve Kuruluş Tarama Aracı'nın yeni sürümleri yayımlanmayacaktır. Daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

**Windows Server Update Services**

Windows Server Update Services'ı (WSUS) kullanarak, yöneticiler en son kritik güncelleştirmeleri ve güvenlik güncelleştirmelerini Windows 2000 işletim sistemlerine ve sonrasına, Office XP'ye ve sonrasına, Exchange Server 2003'e, SQL Server 2000'e, Windows 2000 ve sonraki işletim sistemi sürümlerine hızla ve güvenle dağıtabilir.

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) Web sitesini ziyaret edin.

**Systems Management Server**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir. Yöneticilerin güvenlik güncelleştirmelerini dağıtmak için SMS 2003'ü nasıl kullanacakları hakkında daha fazla bilgi için, [SMS 2003 Güvenlik Düzeltme Eki Yönetimi](http://go.microsoft.com/fwlink/?linkid=22939) Web sitesini ziyaret edin. SMS 2.0 kullanıcıları, güvenlik güncelleştirmelerinin dağıtılmasına yardımcı olması için [Software Update Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340)'i de kullanabilir. SMS hakkında daha fazla bilgi için, [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) Web sitesini ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı ve Microsoft Office Algılama Aracı'nı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler, bu güncelleştirmeleri yüklemek için Elevated Rights Deployment Tool'u kullanabilir ([SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) ve [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) içinde bulunur).

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Yüksek Öncelikli Güncelleştirmeler

Bu ay için:

-   Microsoft, Microsoft Update (MU) ve Windows Server Update Services (WSUS) hizmetinde **güvenlikle ilgili olmayan**, yüksek öncelikli hiçbir güncelleştirme yayımlamadı.
-   Microsoft, Windows Update (WU) sitesinde Windows için **güvenlikle ilgili olmayan**, yüksek öncelikli herhangi bir güncelleştirme yayımlamadı.

Bu bilgiler **yalnızca** güvenlik bülteni özetiyle aynı günde yayımlanan Microsoft Update, Windows Update ve Windows Server Update Services hizmetlerindeki **güvenlikle ilgili olmayan**, yüksek öncelikli güncelleştirmeler için geçerlidir. Diğer günlerde yayımlanan **güvenlikle ilgili olmayan** güncelleştirmeler için bilgi **sağlanmamaktadır**.

#### Güvenlik Stratejileri ve Topluluğu

**Güncelleştirme Yönetim Stratejileri**

[Security Guidance for Patch Management](http://go.microsoft.com/fwlink/?linkid=21168) Web sitesi, güvenlik güncelleştirmelerini uygulamayla ilgili Microsoft'un en iyi uygulama önerilerini sağlar.

**Diğer Güvenlik Güncelleştirmelerini Edinme**

Diğer güvenlik sorunlarıyla ilgili güncelleştirmeler aşağıdaki konumlardan edinilebilir:

-   Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden edinilebilir. "güvenlik\_düzeltme\_eki" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.
-   Tüketici platformlarına yönelik güncelleştirmeler [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) Web sitesinden edinilebilir.
-   Windows Update sitesinde bu ay için sunulan güvenlik güncelleştirmelerini, Yükleme Merkezi'nden Güvenlik ve Kritik Sürümler ISO CD'si Yansıması dosyaları olarak edinebilirsiniz. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Topluluğu**

Güvenliği geliştirmeyi ve BT altyapınızı en iyi duruma getirmeyi öğrenin; ayrıca [IT Pro Security Topluluğu](http://go.microsoft.com/fwlink/?linkid=21164)'nda güvenlik konularında diğer BT Uzmanlarının çalışmalarına katılın.

#### İlgili Kaynaklar

Microsoft, müşterilerimizi korumamıza yardım etmek için bizimle işbirliği yapan aşağıdaki kişi ve kuruluşlara [teşekkür eder](http://go.microsoft.com/fwlink/?linkid=21127):

-   [Assurent Secure Technologies](http://www.assurent.com/) şirketinin Vulnerability Research ekibi, [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667)'de açıklanan sorunu bildirdikleri için
-   [Palo Alto Networks](http://www.paloaltonetworks.com/) için çalışan Yamata Li, [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667)'de açıklanan sorunu bildirdiği için
-   [iDefense VCP](http://labs.idefense.com/) için çalışan anonim bir araştırmacı, [MS07-051](http://go.microsoft.com/fwlink/?linkid=94667)'de açıklanan sorunu bildirdiği için
-   WolfeReiter için çalışan Brian A. Reiter, [MS07-053](http://go.microsoft.com/fwlink/?linkid=94467)'te açıklanan bir sorun konusunda bizimle çalıştığı için
-   [team 509](http://www.team509.com/) için çalışan Woo Shi, [MS07-054](http://go.microsoft.com/fwlink/?linkid=100148)'te açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (11 Eylül 2007): Bülten özeti yayımlandı.
-   V1.1 (12 Eylül 2007): Yeniden başlatma gereksinimi yeniden açıklandı ve MS07-045 için karşıdan yükleme bağlantıları eklendi.

*Built at 2014-04-18T01:50:00Z-07:00*
