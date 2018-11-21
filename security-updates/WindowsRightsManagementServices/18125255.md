---
TOCTitle: RMS için Sistem Yedekleri
Title: RMS için Sistem Yedekleri
ms:assetid: 'c29894da-ee00-428c-8d48-80d8e5a83678'
ms:contentKeyID: 18125255
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747746(v=WS.10)'
---

RMS için Sistem Yedekleri
=========================

Altyapıyı kurup RMS'yi yüklemeden önce, aşağıdaki ilgili bileşenleri yedekleyin:

-   Yapılandırma ve günlük veritabanlarını barındırmak için varolan bir SQL Server veritabanını kullanacaksanız, tüm veritabanlarını ve sunucu ayarlarını yedekleyin. RMS'nin önceki sürümünü yükseltiyor veya RMS'yi yeniden yüklüyorsanız, önceki yapılandırma ve günlük veritabanlarını yedeklediğinizden emin olun.
-   RMS'yi yüklemeyi planladığınız sunucunun sistem durumunu yedekleyin. Bu yedek, sunucunun geri yüklenmesine ihtiyaç duyulduğunda gereken bilgileri içeren kayıt defteri anahtarlarını ve değerleri depolar.
-   Sertifikalarınızı bir dosyaya vermek için Sertifikalar ek bileşenini kullanın. Sertifikalar ek bileşeni, RMS özel anahtar verilerini parola ile şifrelenen PKCS \#12 dosyasında yedeklemek için de kullanılır. RMS'yi yükseltiyor veya yeniden yüklüyorsanız ve RMS özel anahtarını korumak için varsayılan yazılım tabanlı şifrelemeyi kullandıysanız, özel anahtar şifrelenmiş ve yapılandırma veritabanı yedeğiyle birlikte depolanmıştır.
-   Özel anahtarın güvenliğini sağlamak için donanım güvenlik modülü kullandıysanız, yapılandırmasını üretici tarafından önerilen yöntemleri kullanarak yedeklemelisiniz.

Yedek dosyalar, özel anahtarları şifrelemek için kullanılan parolayla birlikte güvenli bir depolama alanında tutulmalıdır.
