---
TOCTitle: Hizmet Bağlantı Noktası Kaydettirmek için
Title: Hizmet Bağlantı Noktası Kaydettirmek için
ms:assetid: '630cc3c3-9ed9-4423-8874-cbaceb43b353'
ms:contentKeyID: 18125118
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720283(v=WS.10)'
---

Hizmet Bağlantı Noktası Kaydettirmek için
=========================================

Hizmet Bağlantı Noktasını Kaydetme
----------------------------------

Bir alt etki alanındaki RMS sunucusundan hizmet bağlantı noktası kaydettiriyorsanız, SCP kaydının başarısız olduğunu belirten bir hata iletisi alabilirsiniz. Çoğu durumda kayıt başarılı olur, ancak kayıt ilk olarak üst düzey etki alanında gerçekleşir ve RMS sunucusu SCP nesnesini denetlediği için alt etki alanını kopyalamak zaman alır SCP ormandaki tüm genel katalog sunucularına kopyalandığında ileti artık görünmez. Bu iletiyi almaya devam ediyorsanız, bu sorunu gidermeyi denemeden önce sorunun çözülüp çözülmediğini görmek için bir süre beklemeniz gerekir.

#### Hizmet Bağlantı Noktası Kaydettirmek için

1.  Active Directory ormanı Yapılandırma kapsayıcısındaki Hizmetler kapsayıcısı altında kapsayıcı nesnesi oluşturmak için yeterli ayrıcalıklara sahip bir etki alanı hesabını kullanarak hizmet bağlantı noktasını kaydetmeniz gereken sunucuya oturum açın. Önceden tanımlanmış güvenlik grubu olan **Enterprise Admins** gerekli ayrıcalıklara sahip hesaba bir örnektir.

2.  **Genel Yönetim** sayfasını açın ve ardından **RMS'yi bu Web sitesinde yönet** bağlantısını tıklatın.

3.  **Yönetim** Giriş sayfasında **RMS hizmeti bağlantı noktası** bağlantısını tıklatın.

4.  **RMS hizmet bağlantı noktası** sayfasında, **URL'yi Kaydet** düğmesini tıklatın.
