---
TOCTitle: 'MS08-OCT'
Title: Microsoft Güvenlik Bülteni Ekim 2008 Özeti
ms:assetid: 'ms08-oct'
ms:contentKeyID: 61235810
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms08-oct(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Ekim 2008 Özeti
==========================================

Yayım Tarihi: 14 Ekim 2008 Salı | Güncelleştirme Tarihi: 23 Ekim 2008 Perşembe

**Sürüm:** 3.0

Bu bülten özetinde Ekim 2008'de yayımlanan güvenlik bültenleri listelenir.

Ekim 2008 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 9 Ekim 2008'de özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 15 Ekim 2008 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Ekim Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374639). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

#### Yürütmeyle İlgili Özetler

Bu ayın güvenlik bültenleri önem derecelerine göre aşağıda listelenmektedir:

Kritik (5)
----------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-067                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Sunucu Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (958644)**](http://go.microsoft.com/fwlink/?linkid=130719)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Sunucu hizmetindeki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı etkilenen bir sistemde özel hazırlanmış bir RPC isteği alırsa uzaktan kod yürütülmesine izin verebilir. Microsoft Windows 2000, Windows XP ve Windows Server 2003 çalışan sistemlerde, bir saldırgan rasgele kod çalıştırmak için kimliğini doğrulamasına gerek kalmadan bu güvenlik açığından yararlanabilir. Bu güvenlik açığından solucan saldırıları düzenlemek için yararlanılabilir. En iyi güvenlik duvarı uygulamaları ve standart varsayılan güvenlik duvarı yapılandırmaları, ağ kaynaklarının kuruluş dışından gerçekleştirilen saldırılardan korunmasına yardımcı olabilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-060                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Active Directory'deki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957280)**](http://go.microsoft.com/fwlink/?linkid=128125)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Windows 2000 Server üzerine yüklendiğinde Active Directory uygulamalarında özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik güncelleştirmesi, bir saldırgan etkilenen bir ağa erişim sağlarsa uzaktan kod yürütülmesine olanak verebilir. Bu güvenlik açığı yalnızca etki alanı denetleyicileri olarak yapılandırılan Microsoft Windows 2000 sunucularını etkiler. Microsoft Windows 2000 sunucusu bir etki alanı denetleyicisi olarak yükseltilmemişse, Basit Dizin Erişim Protokolü (LDAP) veya SSL üzerinden LDAP (LDAPS) sorgularını dinlemeyeceği için bu güvenlik açığından etkilenmez. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-058                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)**](http://go.microsoft.com/fwlink/?linkid=128060)                                                                                                                                                                                                                                                                                                                                                |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, özel olarak bildirilen beş ve genel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse bilginin açığa çıkmasına veya uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                         |
| **Etkilenen Yazılımlar**     | **Microsoft Windows, Internet Explorer.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                              |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-059                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Host Integration Server RPC Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (956695)**](http://go.microsoft.com/fwlink/?linkid=125712)                                                                                                                                                                                                                                                                                                                                                                                    |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Host Integration Server'daki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir saldırgan etkilenen bir sisteme özel hazırlanmış bir Uzaktan Yordam Çağrısı (RPC) isteği gönderirse uzaktan kod yürütülmesine izin verebilir. En iyi uygulamaları kullanan ve SNA RPC hizmet hesabını sistem üzerinde daha az kullanıcı hakkı olacak şekilde yapılandıran müşteriler, SNA RPC hizmet hesabını yönetimsel kullanıcı haklarıyla yapılandıran müşterilere göre daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Güncelleştirme bir yeniden başlatma gerektirebilir.                                                                                                                                                                                                                                                                                                                                                                   |
| **Etkilenen Yazılımlar**     | **Microsoft Host Integration Server.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-057                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956416)**](http://go.microsoft.com/fwlink/?linkid=124653)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir Excel dosyasını Microsoft Office Excel'de açarsa uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen üç güvenlik açığını giderir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir. |
| **En Yüksek Önem Derecesi**  | [Kritik](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

Önemli (6)
----------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-066                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Yardımcı İşlev Sürücüsündeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (956803)**](http://go.microsoft.com/fwlink/?linkid=125709)                                                                                                                                                                                                                                            |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Microsoft Yardımcı İşlev Sürücüsü'ndeki özel olarak bildirilen bir güvenlik açığını giderir. Bu açıktan yerel olarak başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                               |
| **Güvenlik Açığının Etkisi** | Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                                                                                 |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                          |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                  |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-061                                                                                                                                                                                                                                                                                                                |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (954211)**](http://go.microsoft.com/fwlink/?linkid=121738)                                                                                                                                                                                                       |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Windows çekirdeğinde genel olarak bildirilen bir ve özel olarak bildirilen iki güvenlik açığını giderir. Bu güvenlik açıklarından yerel olarak başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Bu güvenlik açıkları uzaktan veya anonim kullanıcılar tarafından kullanılamaz. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                             |
| **Güvenlik Açığının Etkisi** | Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                               |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                        |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-062                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Windows Internet Yazdırma Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (953155)**](http://go.microsoft.com/fwlink/?linkid=120829)                                                                                                                                                                                                                              |
| **Yürütmeyle İlgili Özet**   | Bu güncelleştirme Windows Internet Yazdırma Hizmeti'nde uzaktan kod yürütülmesine izin verebileceği özel olarak bildirilen bir güvenlik açığını giderir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Böylece saldırgan program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir ya da yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                     |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                        |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                        |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-063                                                                                                                                                                                                                                                                                                                                                                                                               |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**SMB'deki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957095)**](http://go.microsoft.com/fwlink/?linkid=127994)                                                                                                                                                                                                                                                                                                                    |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Sunucu İleti Bloğu'ndaki (SMB) özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, dosya veya klasörlerin paylaşıldığı bir sunucuda uzaktan kod yürütülmesine izin verebilir. Bu güvenlik açıklarından başarıyla yararlanan bir saldırgan program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                            |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                       |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                               |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-064                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Sanal Adres Tanımlayıcısını Denetlemedeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (956841)**](http://go.microsoft.com/fwlink/?linkid=128103)                                                                                                                                                                                                                                                                                                                                                                               |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Sanal Adres Tanımlayıcısı'ndaki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir uygulama çalıştırırsa ayrıcalık yükselmesine neden olabilir. Bu güvenlik açığından başarıyla yararlanan kimliği doğrulanmış bir saldırgan etkilenen sistemde ayrıcalık yükseltmesi sağlayabilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm yönetici haklarına sahip olan yeni hesaplar oluşturabilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Güvenlik Açığının Etkisi** | Ayrıcalık Yükselmesi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                                                                                                                                                                                                                                                |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-065                                                                                                                                                                                                                                                                             |
|------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Message Queuing Hizmetindeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (951071)**](http://go.microsoft.com/fwlink/?linkid=128102)                                                                                                                                                              |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi, Microsoft Windows 2000 çalışan sistemlerdeki Message Queuing Hizmeti'nde (MSMQ) özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, MSMQ hizmetinin etkinleştirilmiş olduğu Microsoft Windows 2000 çalışan sistemlerde uzaktan kod yürütülmesine izin verebilir. |
| **En Yüksek Önem Derecesi**  | [Önemli](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                          |
| **Güvenlik Açığının Etkisi** | Uzaktan Kod Yürütme                                                                                                                                                                                                                                                                                             |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirir.                                                                                                                                     |
| **Etkilenen Yazılımlar**     | **Microsoft Windows.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                             |

Orta (1)
--------

<span></span>

| Bülten Tanımlayıcısı         | Microsoft Güvenlik Bülteni MS08-056                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Bülten Başlığı**           | [**Microsoft Office'teki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (957699)**](http://go.microsoft.com/fwlink/?linkid=128145)                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Yürütmeyle İlgili Özet**   | Bu güvenlik güncelleştirmesi Microsoft Office'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir CDO URL'sini tıklatırsa bilginin açığa çıkmasına neden olabilir. Bu güvenlik açığından başarıyla yararlanan bir saldırgan, kullanıcının tarayıcısına bir istemci tarafı komut dosyası ekleyerek içeriği sızdırabilir, bilginin açığa çıkmasına neden olabilir veya kullanıcının etkilenen Web sitesinde gerçekleştirebileceği herhangi bir eylemi kendisi de gerçekleştirebilir. |
| **En Yüksek Önem Derecesi**  | [Orta](http://go.microsoft.com/fwlink/?linkid=21140)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Güvenlik Açığının Etkisi** | Bilginin Açığa Çıkması                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Algılama**                 | Microsoft Baseline Security Analyzer, bu güncelleştirmenin bilgisayar sisteminiz için gerekli olup olmadığını algılayabilir. Bu güncelleştirme yeniden başlatma gerektirmez.                                                                                                                                                                                                                                                                                                                                                                   |
| **Etkilenen Yazılımlar**     | **Microsoft Office.** Daha fazla bilgi için, Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları bölümlerine bakın.                                                                                                                                                                                                                                                                                                                                                                                                                             |

Yararlanma Dizini
-----------------

<span></span>
**Bu tabloyu nasıl kullanabilirim?**  

Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.

| Bülten Kimliği                                            | Bülten Başlığı                                                                                                                                              | CVE Kimliği   | Yararlanma Dizini Değerlendirmesi                                                                             | Önemli Notlar                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [MS08-056](http://go.microsoft.com/fwlink/?linkid=128145) | [Microsoft Office'teki Güvenlik Açığı Bilginin Açığa Çıkmasına Neden Olabilir (957699)](http://go.microsoft.com/fwlink/?linkid=128145)                      | CVE-2008-4020 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    | İşlevsel bir yararlanma kodu oluşturulabilir. Ancak güvenlik açığı yalnızca belirli Web uygulaması senaryolarında bir iletişim kutusundan bilgi sızdırılmasına olanak verdiği için önem derecesi etkisi sınırlıdır. Bu nedenle, saldırganların ilgisini çekmeyebilir.                                                                                                                                                                                                                                                                 |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                   | CVE-2008-4019 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                   | CVE-2008-3471 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-057](http://go.microsoft.com/fwlink/?linkid=124653) | [Microsoft Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (956416)](http://go.microsoft.com/fwlink/?linkid=124653)                   | CVE-2008-3477 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-2947 | (Bülten yayımlandığında genel olarak biliniyordu)                                                             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-3472 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-3473 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-3475 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-3474 | [3 - İşlevsel bir yararlanma kodu olasılığı düşük](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-058](http://go.microsoft.com/fwlink/?linkid=128060) | [Internet Explorer için Toplu Güvenlik Güncelleştirmesi (956390)](http://go.microsoft.com/fwlink/?linkid=128060)                                            | CVE-2008-3476 | [3 - İşlevsel bir yararlanma kodu olasılığı düşük](http://technet.microsoft.com/en-us/security/cc998259.aspx) |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-059](http://go.microsoft.com/fwlink/?linkid=125712) | [Host Integration Server RPC Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (956695)](http://go.microsoft.com/fwlink/?linkid=125712) | CVE-2008-3466 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Host Integration Server yalnızca belirli türde kurumsal müşteriler tarafından yüklenecektir, ancak işlevsel bir yararlanma kodu oluşturulabilir.                                                                                                                                                                                                                                                                                                                                                                                      |
| [MS08-060](http://go.microsoft.com/fwlink/?linkid=128125) | [Active Directory'deki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957280)](http://go.microsoft.com/fwlink/?linkid=128125)                     | CVE-2008-4023 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    | Güvenlik açığı tetiklenerek hizmet reddi durumu oluşturulabilir. Ancak, gerekli bir yazma adresi denetlenemediği için, işlevsel bir yararlanma kodu oluşturularak uzaktan kod yürütülmesi zordur.                                                                                                                                                                                                                                                                                                                                     |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                    | CVE-2008-2250 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                    | CVE-2008-2252 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Birden çok işlemcili sistemler için işlevsel bir yararlanma kodu oluşturulabilir.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| [MS08-061](http://go.microsoft.com/fwlink/?linkid=121738) | [Windows Çekirdeğindeki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (954211)](http://go.microsoft.com/fwlink/?linkid=121738)                    | CVE-2008-2251 | [3 - İşlevsel bir yararlanma kodu olasılığı düşük](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Güvenlik açığı tetiklenebilir, ancak işlevsel bir yararlanma kodu oluşturulması oldukça zordur.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-062](http://go.microsoft.com/fwlink/?linkid=120829) | [Windows Internet Yazdırma Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (953155)](http://go.microsoft.com/fwlink/?linkid=120829)   | CVE-2008-1446 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Sınırlı sayıda ve hedefe yönelik saldırılarda tutarlı yararlanma kodu bulunmuştur. Internet Yazdırma Protokolü (IPP) hizmeti varsayılan olarak etkinleştirilmiştir, ancak tüm platformlarda bu hizmete IIS kullanarak erişmek için varsayılan olarak kimlik doğrulaması da gerekmektedir.                                                                                                                                                                                                                                             |
| [MS08-063](http://go.microsoft.com/fwlink/?linkid=127994) | [SMB'deki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (957095)](http://go.microsoft.com/fwlink/?linkid=127994)                                  | CVE-2008-4038 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-064](http://go.microsoft.com/fwlink/?linkid=128103) | [Sanal Adres Tanımlayıcısını Denetlemedeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (956841)](http://go.microsoft.com/fwlink/?linkid=128103)    | CVE-2008-4036 | [2 - Yararlanma kodu büyük olasılıkla tutarsız](http://technet.microsoft.com/en-us/security/cc998259.aspx)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-065](http://go.microsoft.com/fwlink/?linkid=128102) | [Message Queuing Hizmetindeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (951071)](http://go.microsoft.com/fwlink/?linkid=128102)              | CVE-2008-3479 | [3 - İşlevsel bir yararlanma kodu olasılığı düşük](http://technet.microsoft.com/en-us/security/cc998259.aspx) | Bilginin açığa çıkması söz konusu olabilir, ancak bellekten her zaman kullanışlı içerik alınamayabilir. Bellek bozulması sorunu tetiklenebilir, ancak uzaktan kod yürütülmesi zordur.                                                                                                                                                                                                                                                                                                                                                 |
| [MS08-066](http://go.microsoft.com/fwlink/?linkid=125709) | [Microsoft Yardımcı İşlev Sürücüsündeki Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (956803)](http://go.microsoft.com/fwlink/?linkid=125709)       | CVE-2008-3464 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| [MS08-067](http://go.microsoft.com/fwlink/?linkid=130719) | [Sunucu Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (958644)](http://go.microsoft.com/fwlink/?linkid=130719)                      | CVE-2008-4250 | [1 - Yararlanma kodu büyük olasılıkla tutarlı](http://technet.microsoft.com/en-us/security/cc998259.aspx)     | Sınırlı sayıda ve hedefe yönelik saldırılarda Windows XP'yi etkileyen tutarlı yararlanma kodu bulunmuştur. Bu hizmet varsayılan olarak tüm etkilenen platformlarda etkinleştirilmiş durumdadır; ancak Microsoft Windows 2000, Windows XP ve Windows Server 2003 çalışan sistemlerin bu açıktan etkilenme olasılığı daha yüksektir. Windows Vista, Windows Server 2008 ve Windows 7 Beta platformları kimlik doğrulaması gerektirir ve ASLR ve DEP geliştirmeleri nedeniyle kimlik doğrulamadan sonra da açıktan yararlanmak zorlaşır. |

Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları
--------------------------------------------------

<span></span>
**Bu tabloyu nasıl kullanabilirim?**  

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
<th colspan="10">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=e22eb3ae-1295-4fe2-9775-6f43c5c2aed3)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4 üzerinde Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=8ed7bb9a-4b26-49d7-8c14-60226d2bc20d)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=257c0478-56dd-42eb-a90e-607d01613db7)  
(Kritik)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=02390258-08e9-4b75-960d-be081b749558)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=3a6165a6-d7e7-4526-9291-290caf0639b4)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=8163d1f6-feb5-4f39-8134-3ed42326b822)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=9ed29c3a-0682-4586-bbc2-a73deaa18e4c)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=899e2728-2433-4ccb-a195-05b5d65e5469)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="10">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=0d5f9b6e-9265-44b9-a376-2067b73d6a03)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a7f0f47b-b1ee-4516-9fbf-bf8e579963d0)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4e73de2b-05e6-4901-9bac-46d8f469e635)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b16d9dac-c430-4dd8-a1e5-9a614801f1d9)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=7718bf14-c26c-43f3-be67-4c79ab5b2607)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e7ef571f-c9e8-4e14-95a3-3eeaec55b784)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2f7e5981-6eef-4f08-86c0-c6a7607ea5d0)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=25997b73-a640-49c1-b19e-768a18bbe22c)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4c16a372-7bf8-4571-b982-dac6b2992b25)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=234c05fb-988b-4e02-aab6-bb23e447df3d)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ccf7a3e3-ec30-4b95-9a86-00032301513c)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b607efc-c6fb-4079-8478-e4f3262386d3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b06d3a02-b6e4-4d40-913a-3759a31f20f3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3ae4b913-bff0-4974-b198-828ca10d2a87)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4e1675eb-6b06-48e9-9765-23a2c7737bdc)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=50fae854-0bde-46f8-9444-b9e0d9bfecad)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f26d395d-2459-4e40-8c92-3de1c52c390d)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=ae8d22d5-20aa-471d-a423-f54c9d75febe)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=feaf2adf-7892-4dbf-a147-db4d5dbe52f3)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ee88ff2d-1b12-4f4c-a081-9f27a6fba074)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6e696762-d652-4a8f-ab8f-622f9746c320)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=437a9b68-6a0c-48c8-9348-0d6fda48aa21)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=dbbebb3f-f1c7-402c-bd16-6f88da0d042c)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e8ef3d5f-dd8e-4945-92cd-9d3e30b16667)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c04d2afb-f9d0-4e42-9e1f-4b944a2de400)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=07fc88c4-2571-4a4d-b573-ae576798ab4c)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=319dba34-07ca-47f9-a1e9-20df2df7966b)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ab4d94d3-458c-4946-ab7f-03a279629d25)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=57ca28ea-e5e1-4191-a3d6-84aa90a3d668)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d3df6508-a568-449d-ac97-fbf3f97b98ef)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=989ac6f1-515c-467d-a200-2aabe66d9319)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c2e754f9-086a-494c-bc19-5feed7df8b65)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=ab590756-f11f-43c9-9dcc-a85a43077acf)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b68937af-f04a-4d1e-9d7f-ec92af5194de)  
(Orta)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=47381d91-4a14-4a09-96b3-3345155df52d)  
(Düşük)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=63234f85-6e5d-4ef6-b7cf-d1d2c78a5517)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=1e6c3f81-85bb-48e6-a5af-635a7e540c93)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=748f54f1-40b9-407c-9819-909061b53743)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=91589cfb-15ba-4dd2-9e3b-107899fbcba6)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=5a3832ec-3f8f-42c1-a603-b1330d527547)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="10">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=18fdff67-c723-42bd-ac5c-cac7d8713b21)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=4756e04b-6e1c-4d78-a3c0-17f6b4b97975)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3483b400-cedc-441f-ba8e-594e3df89190)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9b5995df-a3b8-4e81-b118-9bb057e19884)  
(Önem derecesi yok)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=72dd6015-25d1-45f4-a769-88ac43074b44)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=b4212db5-093e-497d-b999-2e3780f9f7c2)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a976999d-264f-4e6a-9bd6-3ad9d214a4bd)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=bd19c72b-4f83-47ab-93be-d2c286e732c4)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=905ab030-14a5-4a3d-aa11-e8f957f6a1ea)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4a0fcf4b-eb8e-456a-b934-400ae18248ee)  
(Önem derecesi yok)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f793af16-5464-4db1-a42b-1c5f17c538ed)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c20808cb-c30a-4b53-91e5-810eb6b4b2e3)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="10">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
32-bit sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=25c17b07-1efe-43d7-9b01-3dfdf1ce0bd7)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ec73f416-2204-42d6-8932-c96578ac819f)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=8b97114a-71aa-47a2-b9e7-f4e158c18c80)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=3d6290d8-1745-4bc0-9ca9-eeb1ad0be4a5)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=cf6744e6-b54c-40f6-a78d-7ba9453133c0)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ec9eeb82-0497-4c55-94bb-9a47cb3521b4)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=7b12018e-0cc1-4136-a68c-be4e1633c8df)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=baacd1c2-9764-4fea-bd4d-c49791974fef)\*\*  
(Düşük)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=6e641db2-90c8-458f-9795-3e46b70a5203)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=a33c833c-d5c5-4e37-8f89-7b9079f92e59)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=223236e8-7b19-4b47-8a90-bfc35eb9318a)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=0bc178b8-f8ae-4f41-8f88-fb6a75be1bca)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=2bcf89ef-6446-406c-9c53-222e0f0baf7a)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=250a45dd-7eae-4440-bd10-02a703940976)  
(Düşük)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=b6546e1c-bf7b-4354-8574-6c16fa707de0)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=31783e88-76e2-4bc6-b4ae-308443c6d223)  
(Önem derecesi yok)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=077b697c-04a0-45bd-b08c-331d5c30cb47)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=0af72663-4945-4916-8c55-090ba4d82793)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="10">
Windows 7 Beta
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-067**](http://go.microsoft.com/fwlink/?linkid=130719)
</td>
<td style="border:1px solid black;">
[**MS08-060**](http://go.microsoft.com/fwlink/?linkid=128125)
</td>
<td style="border:1px solid black;">
[**MS08-058**](http://go.microsoft.com/fwlink/?linkid=128060)
</td>
<td style="border:1px solid black;">
[**MS08-066**](http://go.microsoft.com/fwlink/?linkid=125709)
</td>
<td style="border:1px solid black;">
[**MS08-061**](http://go.microsoft.com/fwlink/?linkid=121738)
</td>
<td style="border:1px solid black;">
[**MS08-062**](http://go.microsoft.com/fwlink/?linkid=120829)
</td>
<td style="border:1px solid black;">
[**MS08-063**](http://go.microsoft.com/fwlink/?linkid=127994)
</td>
<td style="border:1px solid black;">
[**MS08-064**](http://go.microsoft.com/fwlink/?linkid=128103)
</td>
<td style="border:1px solid black;">
[**MS08-065**](http://go.microsoft.com/fwlink/?linkid=128102)
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
32-bit sistemler için Windows 7 Beta
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows 7 Beta](http://www.microsoft.com/downloads/details.aspx?familyid=e877d9c1-3e7c-4551-a899-c3fcc5175bb6)  
(Önemli)
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
</tr>
<tr>
<td style="border:1px solid black;">
x64 tabanlı sistemler için Windows 7 Beta
</td>
<td style="border:1px solid black;">
[Windows 7 Beta x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=0fa96b25-90e3-46ab-bcd5-051f4b2b881b)  
(Önemli)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows 7 Beta
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows 7 Beta](http://www.microsoft.com/downloads/details.aspx?familyid=66646156-f3e6-48d7-be22-de1772dd1884)  
(Önemli)
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
</tr>
</table>
 
**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirmeler tarafından giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

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
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=1b2740e0-ecdd-48ca-84e0-eb187c31eb16)  
(KB955461)  
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
[Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=27cedef1-c47c-472c-a343-cd9b4ebc2bba)  
(KB955464)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=b1aee2d5-bfa0-40e3-91b6-98bf65524e8c)  
(KB956464)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 ve Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Excel 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Önemli)  
[Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=4df27e8a-d803-483b-a700-0177d71bf368)  
(KB955466)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi ve 2007 Microsoft Office Sistemi Service Pack 1
</td>
<td style="border:1px solid black;">
[Excel 2007](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Önemli)  
[Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2765bbc0-ea2e-4b6e-822c-222ee8e5021f)  
(KB955470)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="3">
Mac için Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=ba4fa21a-7e01-4ef8-9b9f-9d51d00ef094)  
(KB958312)  
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
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=e70c5ae0-2858-46de-81f8-dcd1786656b7)  
(KB958267)  
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
[Mac için Açık XML Dosya Biçimi Dönüştürücüsü](http://www.microsoft.com/downloads/details.aspx?familyid=2a8d9a3b-b8a4-43b6-82a6-a2e7d16ae11d)  
(KB958304)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
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
[**MS08-057**](http://go.microsoft.com/fwlink/?linkid=124653)
</td>
<td style="border:1px solid black;">
[**MS08-056**](http://go.microsoft.com/fwlink/?linkid=128145)
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
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Önemli)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9769ce08-5207-4c63-b7b9-536266ad6b2b)  
(KB955468)  
(Önemli)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=83c88444-75b8-44d1-b280-3671394ade45)  
(KB955935)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Önemli)  
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=9a7be004-5903-4101-90c5-c0d5f8722af9)  
(KB955936)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5c29e646-504c-4455-9d35-9a1bed6d7535)\*  
(KB955937)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Önemli)  
[Microsoft Office SharePoint Server 2007 x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3c21c405-2c9e-45d0-be4d-8ccd093af31f)\*  
(KB955937)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
\*Bu güncelleştirme Microsoft Office SharePoint Server 2007 Enterprise sürümünün varsayılan yapılandırması ve Internet Siteleri için Microsoft Office SharePoint Server 2007 gibi Excel Hizmetleri'nin yüklü olduğu sunuculara uygulanır. Microsoft Office SharePoint Server 2007 Standard sürümü Excel Hizmetleri'ni içermemektedir.

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
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS08-059**](http://go.microsoft.com/fwlink/?linkid=125712)
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
Microsoft Host Integration Server 2000
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2000 Service Pack 2 (Sunucu)](http://www.microsoft.com/downloads/details.aspx?familyid=11cca58b-59a4-4e93-9eb1-19b07c290a10)  
(Kritik)  
[Microsoft Host Integration Server 2000 Administrator Client](http://www.microsoft.com/downloads/details.aspx?familyid=41b49291-1231-4e23-aef7-818207453d56)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 (Sunucu)](http://www.microsoft.com/downloads/details.aspx?familyid=9ca255ed-9334-4848-af94-49ef3078cdc0)  
(Kritik)  
[Microsoft Host Integration Server 2004 Service Pack 1 (Sunucu)](http://www.microsoft.com/downloads/details.aspx?familyid=eca756a1-ca56-4481-b23c-53c159a4e08c)  
(Kritik)  
[Microsoft Host Integration Server 2004 (İstemci)](http://www.microsoft.com/downloads/details.aspx?familyid=92cb54e7-f4ff-40a4-99cb-6257c4d8d4cd)  
(Kritik)  
[Microsoft Host Integration Server 2004 Service Pack 1 (İstemci)](http://www.microsoft.com/downloads/details.aspx?familyid=d776515c-09aa-4a04-876d-606bfc26a006)  
(Kritik)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Microsoft Host Integration Server 2006](http://www.microsoft.com/downloads/details.aspx?familyid=1ae79da3-ec17-4d4b-8011-d777a237ac93)  
(Kritik)  
[x64 tabanlı sistemler için Microsoft Host Integration Server 2006](http://www.microsoft.com/downloads/details.aspx?familyid=05da4540-4976-458a-a612-7385d78695a2)  
(Kritik)
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

-   [NetAgent Co., Ltd.](http://www.netagent.co.jp/), MS08-056'da açıklanan sorunu bildirdikleri için
-   [iDefense](http://labs.idefense.com/) için çalışan Joshua J. Drake, MS08-057'de açıklanan sorunu bildirdiği için
-   Wushi, [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-057'de açıklanan sorunu bildirdikleri için
-   [Labo Skopia](http://www.laboskopia.com/) için çalışan Lionel d'Hauenens, [iDefense VCP](http://labs.idefense.com/) ile birlikte çalışarak MS08-057'de açıklanan sorunu bildirdikleri için
-   David Bloom, MS08-058'de açıklanan sorunu bildirdiği için
-   Gregory Rubin, MS08-058'de açıklanan sorunu bildirdiği için
-   [Ivan Fratric](http://ifsec.blogspot.com/), [TippingPoint](http://www.tippingpoint.com/) ve [Zero Day Initiative](http://www.zerodayinitiative.com/) ile birlikte çalışarak MS08-058'de açıklanan sorunu bildirdikleri için
-   [n.runs](http://www.nruns.com/) için çalışan Thierry Zoller, MS08-058'de açıklanan sorunu bildirdiği için
-   [Composica](http://www.composica.com/) için çalışan Lee Dagon, MS08-058'de açıklanan sorunu bildirdiği için
-   [Harmony Security](http://www.harmonysecurity.com/) için çalışan Stephen Fewer, [iDefense VCP](http://labs.idefense.com/) ile birlikte çalışarak MS08-059'da açıklanan sorunu bildirdikleri için
-   [nCircle](http://www.ncircle.com/) için çalışan Paul Miseiko, MS08-060'da açıklanan sorunu bildirdiği için
-   [iShadow](http://www.ishadow.com/) için çalışan Paul Caton, MS08-061'de açıklanan sorunu bildirdiği için
-   [SkyRecon](http://www.skyrecon.com/) için çalışan Thomas Garnier, MS08-061'de açıklanan sorunu bildirdiği için
-   [CERT/CC](http://www.cert.org/), MS08-062'de açıklanan sorunu bildirdikleri için
-   [Codenomicon](http://www.codenomicon.com/) için çalışan Joshua Morin, MS08-063'te açıklanan sorunu bildirdiği için
-   [TippingPoint DVLabs](http://dvlabs.tippingpoint.com) için çalışan Cody Pierce ve Aaron Portnoy, MS08-065'te açıklanan sorunu bildirdikleri için
-   [SkyRecon](http://www.skyrecon.com/) için çalışan Fabien Le Mentec, MS08-066'da açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (14 Ekim 2008): Bülten özeti yayımlandı.
-   V2.0 (15 Ekim 2008): Itanium tabanlı sistemler için Windows Server 2008 (MS08-062) önem derecesi kaldırıldı.
-   V2.1 (16 Ekim 2008): Microsoft Güvenlik Bülteni MS08-062 için Yürütmeyle İlgili Özet güncelleştirildi.
-   V3.0 (23 Ekim 2008): Microsoft Güvenlik Bülteni MS08-067: Sunucu Hizmeti'ndeki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (958644) eklendi.

*Built at 2014-04-18T01:50:00Z-07:00*
