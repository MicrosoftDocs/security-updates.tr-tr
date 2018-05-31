---
TOCTitle: Geçiş Gereksinimlerini Değerlendirme
Title: Geçiş Gereksinimlerini Değerlendirme
ms:assetid: 'cec07f45-dc52-4004-860b-5cc33e5fc209'
ms:contentKeyID: 18125320
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747759(v=WS.10)'
---

Geçiş Gereksinimlerini Değerlendirme
====================================

RMS dağıtımı yapan kuruluşların, sunucunun hizmet dışı kalma süresini en aza indiren bir geçiş planı oluşturması gerekir, böylece kullanıcıların RMS korumalı içeriğe erişimlerini kesintiye uğratmadan sunucu bakım ve yükseltme senaryolarını destekleyebilirler. Önceki yapılandırma ve günlük veritabanları RMS tarafından kullanılabildiğinden, RMS'yi bir sunucudan diğerine geçirmenin kuruluşa etkisi, uygun yordamların kullanılması durumunda en düşük düzeyde olmalıdır. Geçiş senaryosu, varolan veritabanlarını kullanmak istediğinizi, tersi durumda da yeni bir RMS yüklemesi gerçekleştireceğinizi varsayar.

Değiştirdiğiniz RMS sunucusu, nCipher gibi bir donanım güvenlik modülü (HSM) kullanıyorsa, RMS'yi sunucuya yükleme ve sağlama işlemlerini yapmadan önce HSM yapılandırmasını yeni sunucuya aktarmanız gerekir. Yönergeler için donanım güvenlik modülüyle birlikte verilen belgelere bakın.

Geçiş yapmadan önce:

-   Veritabanlarının kullanılabilir olduğundan emin olun.
-   Yeni yüklemede hangi bilgisayarların kullanılacağına karar verin.

RMS yüklemenize geçiş yaptırmak için aşağıdaki adımları kullanın:

1.  Geçiş işlemini başlatmadan önce, veritabanlarını, özel anahtarları ve sistem durumunu da içerecek şekilde tüm bileşenleri yedekleyin.
2.  Önceki RMS yüklemesindeki veritabanlarının, yeni dağıtımda kullanılacak veritabanı sunucusunda bulunduğundan emin olun.
3.  RMS'yi uygun sunuculara yükleyin ve sağlayın ve veritabanlarının konumunu belirleyin.

RMS sunucusuna geçiş işlemi yaptırılmasına neden olan en sık rastlanan senaryo, pilot RMS dağıtımının üretim ortamına taşınmasıdır. Bu kullanım senaryosu hakkında daha fazla bilgi için bu belge grubundaki “RMS Dağıtma" bölümünde bulunan "Pilot Dağıtımı Üretim Dağıtımına Taşıma” konusuna bakın.
