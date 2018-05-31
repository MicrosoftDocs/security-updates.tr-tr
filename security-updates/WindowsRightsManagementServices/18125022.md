---
TOCTitle: Hak İlkesi Şablonu Eklemek için
Title: Hak İlkesi Şablonu Eklemek için
ms:assetid: '1a5555cd-6d39-4078-a879-4106864674be'
ms:contentKeyID: 18125022
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720206(v=WS.10)'
---

Hak İlkesi Şablonu Eklemek için
===============================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Hak İlkesi Şablonu Ekleme
-------------------------

#### Hak İlkesi Şablonu Eklemek için

1.  **Genel Yönetim** sayfasını açın ve hak ilkesi şablonu eklemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Hak ilkesi şablonları**'nı tıklatın.

3.  **Dil** alanında, şablonun kullanmasını istediğiniz dil seçeneğini tıklatın.

4.  **Hak ilkesi şablonu ekle**'yi tıklatın.

5.  **Şablon kimliği** alanında, şablon için bir ad, açıklama ve haklar isteği URL'si belirtin.

6.  **Kullanıcılar ve gruplar** alanında, **Kullanıcılar veya gruplar ekle**'de, eklenecek kullanıcı veya grubun geçerli e-posta adresini yazın ve sonra **Ekle**'yi tıklatın. Gerektiğinde diğer kullanıcıları veya grupları eklemek için aynı işlemi yineleyin.

7.  **Geçerli kullanıcılar veya gruplar**'da, hakların atanacağı kullanıcının veya grubun e-posta adresini seçin.

8.  Seçili kişi veya gruba hak vermek için tüm hakların onay kutularını işaretleyin. Kalan kullanıcı ve gruplara hak vermek işin işlemi tekrarlayın.

9.  **Süre sonu ilkesi** alanında, üç süre sonu seçeneğinden birini seçin ve sonra uygun bir şekilde süre sonu tarihi veya saati belirtin. Uygunsa, **İçerik kullanım lisansları her ... günde bir yenilenmelidir**'i seçin ve yenilemeler arasındaki gün sayısını belirtin.

10. **Uzatılan ilke** alanında, dört seçenekten birini veya daha fazlasını seçin. **Uygulamaya özgü verileri zorla**'yı seçerseniz, zorlanacak veri için bir ad ve değer belirtin ve ardından **Ekle**'yi tıklatın.

11. İptal işlemini uygulamak için, **İptal ilkesi** alanında, **İptal isteyin** onay kutusunu seçin ve sonra aşağıdaki adımları izleyin:

    1.  **URL veya UNC** alanına iptal listesi dosyasının yollanacağı URL'yi yazın Bağlantısı kesilmiş kullanıcıları ve dış kullanıcıları desteklemeniz gerekirse, bu URL'ye hem kurumsal ağdan hem de Internet'ten erişilebilmelidir.
    2.  **İptal listesi yenileme aralığı**'nda, iptal listesinin geçerli kalacağı gün sayısını yazın. Kullanıcı iptal listesinin bu değerden daha eski bir kopyasına sahipse, içeriği kullanmak için güncelleştirilmiş bir iptal listesini edinmelidir.
    3.  **Ortak anahtar dosyası**'nda, yolu ve dosya adını yazın veya iptal listesinin ortak anahtar dosyasını bulmak için **Gözat**'ı tıklatın. Bu dosya hakkında daha fazla bilgi için bu konuda daha önce geçen "İptal listesine imza ekleme" bölümüne bakın.

    | ![](/security-updates/images/Cc720206.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | İptal işlemini yaparken dikkatli olun. Belirttiğiniz yenileme aralığına bağlı olarak iptal listesini düzenli olarak yenilemeniz gerekir; aksi takdirde liste otomatik olarak geçersiz hale gelir ve kullanıcıların o listeyi gerektiren içeriği kullanmasını önler. Kullanıcıların içeriği kullanmasını yanlışlıkla engellememek için iptal listesinin yenilenmesi için gerekli kıldığınız aralığı dikkatle değerlendirin. Daha fazla bilgi için bu konuda daha önce geçen "[İptali Yönetme](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)" bölümüne bakın. |

12. **Gönder**'i tıklatın.

İptal işlemi hakkında daha fazla bilgi için bu konuda daha önce geçen "[İptali Yönetme](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)" bölümüne bakın.

İptal seçeneklerini belirtirken dikkat edilmesi gereken noktalar için, bu konuda daha önce geçen "[İptal İlkelerini Tanımlama](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)" bölümüne bakın.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.
