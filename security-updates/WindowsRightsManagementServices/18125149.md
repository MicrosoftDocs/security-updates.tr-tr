---
TOCTitle: Güvenilen Yayımlama Etki Alanı Eklemek için
Title: Güvenilen Yayımlama Etki Alanı Eklemek için
ms:assetid: '731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c'
ms:contentKeyID: 18125149
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747624(v=WS.10)'
---

Güvenilen Yayımlama Etki Alanı Eklemek için
===========================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

RMS özel anahtarınızı korumak için bir donanım güvenlik modülü kullanıyorsanız ve yazılım tabanlı özel anahtar koruması kullanan bir RMS yüklemesinden sunucu lisans sertifikası alıyorsanız, sertifikayı alma girişiminde bulunmadan önce kümedeki her sunucunun **Güvenlik ayarları** sayfasında bir özel anahtar parolası belirtmeniz gerekir.

Güvenilen Yayımlama Etki Alanı Ekleme
-------------------------------------

#### Güvenilen Yayımlama Etki Alanı Eklemek için

1.  **Genel Yönetim** sayfasını açın ve sonra güvenilen yayımlama etki alanı eklemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Güven ilkeleri**'ni tıklatın.

3.  **Güvenilen yayımlama etki alanları** alanında, **Gözat**'ı tıklatın. Eklemek istediğiniz yayımlama etki alanının sertifikasını bulun ve çift tıklatın. **Alınan dosyanın şifresini çözmek için kullanılacak parola**'da, bu dosyanın şifresini çözmek için gereken parolayı yazın ve ardından **Al**'ı tıklatın.

    Parolayla şifrelenmiş dosya; lisans sertifikasını, özel anahtarı (anahtar yazılımda depolanıyorsa) ve hak ilkesi şablonlarını içerir.

4.  Etki alanının adı **Güvenilen yayımlama etki alanları** listesinde görünür.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Güvenilen Yayımlama Etki Alanı Ekleme ve Kaldırma](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee)" bölümüne bakın.
