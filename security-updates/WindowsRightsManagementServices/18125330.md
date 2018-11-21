---
TOCTitle: Kök Sertifika Sunucusu Kaydı
Title: Kök Sertifika Sunucusu Kaydı
ms:assetid: 'f08bc919-f090-4843-b2ce-b40d558012ce'
ms:contentKeyID: 18125330
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747734(v=WS.10)'
---

Kök Sertifika Sunucusu Kaydı
============================

RMS dağıtımındaki ilk sunucunun Microsoft Kayıt Hizmeti'ne kaydolması gerekir. Kök sertifika sunucusu olan bu sunucu, Internet bağlantısı varsa sağlama sırasında otomatik olarak kaydettirilebilir veya sunucu kapalı bir ağda yer alıyorsa kayıt işlemi el ile yapılabilir. El ile sunucu kaydı hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Kök Sertifika Sunucusunu El İle Kaydettirmek İçin" konusuna bakın.

Kayıt isteği aşağıdaki giriş parametrelerini içerir:

-   1024 bit ortak anahtar. Bu ortak anahtar, RMS ortak anahtarıdır.
-   Kaydettirilecek RMS sunucusunun sürümü, adı ve URL'si.

Microsoft Kayıt Hizmeti, bilgileri yalnızca sunucu lisans sertifikası oluşturmak için kullanır ve bunları yalnızca iptal işlemlerinde kullanma amacıyla depolar.

Microsoft Kayıt Hizmeti, kayıt sunucusunun imzaladığı bir sertifikanın yanı sıra, kayıt sunucusunun lisans sertifika zincirini içeren bir sertifika zinciri döndürür. Sertifika, kayıt özel anahtarıyla imzalanan sunucu ortak anahtarını, kayıtlı sunucunun sürümünü ve URL'sini içerir. Bu sertifika kök sertifika sunucusuna, lisans sunucularına sunucu lisans sertifikaları verme hakkıyla birlikte hak hesabı sertifikaları, istemci lisans sertifikaları, yayımlama ve kullanım lisansları verme hakkı da verir.

Sunucu lisans sertifikası bir yıl süreyle geçerlidir. Geçerlilik süresi sertifikanın verildiği tarihte başlar. Geçerlilik süresi sonunda sertifika yenilenebilir. Sunucu tarafından verilen sertifikalar ve lisanslar yedi yıl süreyle geçerlidir. Geçerlilik süresi sertifikanın veya lisansın verildiği tarihte başlar.

Sertifikanın iptaliyle ilgili bilgiler, sunucu lisans sertifikasına, kayıt isteğinde belirtilen şekilde eklenir. Microsoft Kayıt Hizmeti ortak anahtarı sertifikaya bir iptal anahtarı olarak eklenir. Ayrıca, üçüncü taraf iptal anahtarı belirtildiyse, bu da iptal anahtarı olarak sertifikaya eklenir.
