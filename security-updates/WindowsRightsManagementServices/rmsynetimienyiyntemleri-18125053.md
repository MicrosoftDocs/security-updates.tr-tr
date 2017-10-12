---
TOCTitle: RMS Yönetimi En İyi Yöntemleri
Title: RMS Yönetimi En İyi Yöntemleri
ms:assetid: '385f8112-da00-417f-a2b8-42dc1e06b717'
ms:contentKeyID: 18125053
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720245(v=WS.10)'
---

RMS Yönetimi En İyi Yöntemleri
==============================

RMS yönetiminde, aşağıda belirtilen en iyi yöntemleri göz önüne alın.

-   **RMS Sunucularında Ek Hizmetler Dağıtmama**
    Sunucularınızda RMS hizmetleri dışında başka hizmetler çalıştırıyorsanız, güvenlik sorunlarına neden olabilecek çakışmalar oluşabilir. Hizmet performansındaki azalma veya çakışmayı izlemek için performans sayaçları kullanın.
-   **Yapılandırma Veritabanlarını Sık Aralıklarla Yedekleme**
    Yapılandırma veritabanları, RMS'nin çalışması için gerekli olan bilgileri depolar. Ayrıca, kök sertifika kümesi yapılandırma veritabanı da tüm yüklemeye yönelik anahtar çiftlerini depolar. Düzenli olarak yedekleme yapıyorsanız, veritabanı sunucusu hatasında RMS işlevselliğini hızlı bir şekilde yeniden sağlayabilirsiniz. Düzenli yedekleme yapmanın yanı sıra, ayrı bir sınama ortamında geri yüklemeleri tek tek kendiniz gerçekleştirerek, bu yedeklerin geçerliliğini de düzenli olarak sınamalısınız. Daha fazla bilgi için bu belge grubunun "RMS Dağıtımı Planlama" bölümündeki "RMS Sistemini Yedekleme ve Geri Yükleme" konusuna bakın.
-   **Günlük Veritabanını Düzenli Olarak Küçültme**
-   **RMS Sunucusunu İzlemek için Microsoft Operations Manager (MOM) Kullanma**
    Önemli olayları izlemek veya performanstaki azalmayı algılamak ve söz konusu olaylara ilişkin bildirim göndermek için MOM ve RMS MOM Paketi kullanın.
