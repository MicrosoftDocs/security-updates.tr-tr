---
TOCTitle: Günlüğü Açma ve Kapatma
Title: Günlüğü Açma ve Kapatma
ms:assetid: '50ccd827-2d39-41e7-a395-3d5f5836869b'
ms:contentKeyID: 18125090
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747565(v=WS.10)'
---

Günlüğü Açma ve Kapatma
=======================

**Günlük ayarları** sayfasından, geçerli küme veya sunucu için günlüğü açıp kapatırsınız. Günlüğün kapatılması, RMS Web hizmetlerinin günlük ileti sırasına günlüğe kaydedilen verileri göndermesini engeller. Ayrıca, günlük dinleyici hizmetini de durdurur. Günlüğün Windows Server 2003 Hizmetleri yönetim aracı kullanılarak kapatılması desteklenmez.

RMS günlükleri veritabanı sunucusuna Message Queuing ile gönderilir. Veritabanı sunusuyla bir bağlantı yoksa, Message Queuing günlükleri tekrar bağlantı sağlanana kadar yerel önbellekte depolayacaktır. Günlük kaydetmeyi ilk kez etkinleştiriyorsanız, RMS sunucusunun veritabanı sunucusuna bağlantısı olduğundan ve veritabanı hizmetinin başlatıldığından emin olun. Veritabanı sunucunuz olarak SQL Server kullanıyorsanız, günlüklerin veritabanına yazıldığını aşağıdaki adımları izleyerek doğrulayabilirsiniz:

-   SQL Server Enterprise Manager'da günlük veritabanına gidin, **Veritabanları**'nı genişletin ve sonra RMS günlüklerini içeren veritabanını genişletin.
-   Günlük veritabanını tıklatın, **Tablolar**'ı tıklatın, **DRMS\_log\_master**'ı sağ tıklatın ve sonra **Tablo aç - tüm satırları getir**'i tıklatın. Günlük dosyaları oluşturulmaktaysa, bir veya daha fazla günlük dosyası göreceksiniz.
