---
TOCTitle: Günlüğü Açmak veya Kapatmak için
Title: Günlüğü Açmak veya Kapatmak için
ms:assetid: '8e672f95-566f-4070-9a2a-2f70f087148f'
ms:contentKeyID: 18125177
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747674(v=WS.10)'
---

Günlüğü Açmak veya Kapatmak için
================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

RMS sunucusunun veritabanı sunucusuna bağlı olduğundan ve veritabanının günlük almanın etkinleştirilmesinden önce başlatıldığından emin olun. Message Queuing günlükleri günlük veritabanına aktaramıyorsa verileri RMS sunucusunun sabit diskinde sırada tutacaktır. Sunucunun depolama alanı dolana kadar bu işleme devam edecektir. Bu özellik SQL sunucusuyla olan bağlantıda kesinti olduğu zaman günlük kaydetmeyi desteklediği için RMS bu durumda bir hata mesajı görüntülemez.

Günlüğü Açma veya Kapatma
-------------------------

#### Günlüğü Açmak veya Kapatmak için

1.  **Genel Yönetim** sayfasını açın ve sonra günlüğe kaydetme hizmetini açmak veya kapatmak istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Günlük ayarları**'nı tıklatın.

3.  **Günlük sunucusu ve veritabanı** alanında, **Günlüğü etkinleştir** onay kutusunu seçin ve sonra **Güncelleştir**'i tıklatın.

    Günlüğe kaydetmeyi etkinleştirmek için, onay kutusunu temizleyin ve sonra **Güncelleştir**'i tıklatın.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Günlüğü Açma ve Kapatma](https://technet.microsoft.com/50ccd827-2d39-41e7-a395-3d5f5836869b)" bölümüne bakın.
