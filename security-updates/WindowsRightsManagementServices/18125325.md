---
TOCTitle: Güvenilen Kullanıcı Etki Alanı Eklemek için
Title: Güvenilen Kullanıcı Etki Alanı Eklemek için
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18125325
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747793(v=WS.10)'
---

Güvenilen Kullanıcı Etki Alanı Eklemek için
===========================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Güvenilen Kullanıcı Etki Alanı Ekleme
-------------------------------------

#### Güvenilen Kullanıcı Etki Alanı Eklemek için

1.  **Genel Yönetim** sayfasını açın ve sonra güvenilir kullanıcı etki alanı eklemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim** bağlantıları alanında, **Güven ilkeleri**'ni tıklatın.

3.  **Güvenilen kullanıcı etki alanları** alanında **Gözat**'ı tıklatın, güven ilişkisi oluşturmak amacıyla almak istediğiniz kullanıcı etki alanının sunucu sertifikasını çift tıklatın ve ardından **Ekle**'yi tıklatın.

    Etki alanının adı **Güvenilen kullanıcı etki alanları** listesinde görünür.

4.  Güvenilen kullanıcı etki alanındaki hangi e-posta etki alanlarının güvenilir olduğunu belirtmek için, listedeki sertifika adının yanında bulunan **Güvenilen etki alanları**’nı tıklatarak **Güvenilen e-posta etki alanları** penceresini açın.

5.  Aşağıdaki güven seçeneklerinden birini seçin:

    -   Bu etki alanının üyesi olan tüm kullanıcı hesaplarına güvenmek için **Tüm e-posta etki alanlarına güven** seçeneğini seçin.
        –veya-
    -   **Yalnızca belirtilen e-posta etki alanlarına güven** seçeneğini belirleyip etki alanı adını yazın (örneğin, example.com) ve **Ekle**’yi tıklatın. Bu işlem, etki alanını Güvenilen e-posta etki alanları listesine ekler. Listeden ad kaldırmak için, adı seçin ve ardından **Kaldır**'ı tıklatın. Etki alanıyla birlikte tüm alt etki alanları listelenir.

6.  RMS'yi, grup üyeliğini ormanlar arasında genişletmeniz gereken bir ortamda kullanıyorsanız, **Bu kullanıcı etki alanı için güvenlik tanıtıcılarının (SID) RM lisansına güven** onay kutusunu işaretleyin.

7.  Tamamlandığında, **Pencereyi kapat ve Güven İlkeleri'ne geri dön**'ü tıklatın.

Bu yordamı uygulama hakkında daha fazla bilgi için, bu konuda daha önce geçen "[Güvenilen Kullanıcı Etki Alanı Ekleme ve Kaldırma](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1)" bölümüne bakın.
