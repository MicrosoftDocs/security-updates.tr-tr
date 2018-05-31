---
TOCTitle: Anahtar Yönetimi Gereksinimlerini Tanımlama
Title: Anahtar Yönetimi Gereksinimlerini Tanımlama
ms:assetid: 'f0e08fb8-bf5e-4278-a09f-daa57696e786'
ms:contentKeyID: 18125350
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747797(v=WS.10)'
---

Anahtar Yönetimi Gereksinimlerini Tanımlama
===========================================

RMS, içerik koruması ve hak uygulaması sağlamak için şifreleme anahtarları kullanır. Şifreleme anahtarları, sistemin kesintisiz ve güvenli bir şekilde çalışmasını sağlayan temel bilgi parçalarıdır. Yöneticiler, veri kaybına, sistem arızalarına ve hırsızlığa karşı koruma sağlamak için bu anahtarları düzgün bir şekilde yönetmeye özen göstermelidir.

Varsayılan yapılandırmada, RMS, sunucu anahtar çiftini ve bununla ilişkili GUID'yi yapılandırma veritabanındaki bir tabloda depolar. Sunucu anahtar çifti, sağlama işlemi sırasında seçtiğiniz parola kullanılarak şifrelenir.

Sunucu anahtar çiftinin ve bununla ilişkili GUID'nin korunmasına yardımcı olmak için, yapılandırma veritabanını bir depolama ortamına (CD gibi) yedekleyin ve bu yedek ortamını güvenli bir yerde (şirket dışında bir kasa gibi) saklayın. Yedeklerin zamanlaması, ne kadar sık yönetim değişiklikleri yaptığınıza ve ortam yıpranmasının veya ortamla ilgili başka risklerin yol açacağı veri kaybına yönelik kabul edebileceğiniz risk düzeyine bağlıdır. Yapılandırma veritabanının yedeklenmesinde kullanılan özel anahtar parolasını bilmeniz gerekir. Uygun parola olmadan, yedeği RMS sunucusuna geri yükleyemezsiniz.

Veritabanı sunucusu olarak SQL Server kullanıyorsanız, şifrelenen özel anahtar verilerinin ve GUID'nin değerini doğrudan güvenli bir diskete veya başka bir ortama kopyalamak için SQL Server Enterprise Manager'ı kullanabilirsiniz. Özel anahtar korunduğundan, yedeği güvenli bir ortamdan RMS yüklemesine geri yüklerseniz, RMS yüklemesinin yedekle aynı RMS hizmet hesabının altında çalışması gerekir.

Sunucunun özel anahtarını korumak için yazılım veya donanım CSP'si kullanıyorsanız, anahtar kapsayıcısını ve anahtarı kendiniz yedeklemelisiniz. Donanım güvenlik modülü kullandığınızda, özel anahtarların güvenliği özel anahtarları donanımda tutarak ve hiçbir zaman yazılımla karşı karşıya bırakmayarak iyileştirilir. Şifresinin çözülmesi veya imzalanması gereken veriler donanım güvenlik modülüne aktarılır, şifresi çözülür veya imzalanır ve sonra dışarıya çıkarılır.

Donanım veya yazılım için olmasına bağlı olmaksızın her CSP'nin anahtarı güvenli bir şekilde yedeklemeye yönelik özel yordamları vardır; bu yordam hakkında fazla bilginiz yoksa CSP belgelerine bakmalısınız.
