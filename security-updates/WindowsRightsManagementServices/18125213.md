---
TOCTitle: Hak İlkesi Şablonu Düzenlemek için
Title: Hak İlkesi Şablonu Düzenlemek için
ms:assetid: '9580b934-bd6f-4097-9d3c-4fc14a3147fa'
ms:contentKeyID: 18125213
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747684(v=WS.10)'
---

Hak İlkesi Şablonu Düzenlemek için
==================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Hak İlkesi Şablonu Düzenleme
----------------------------

#### Hak İlkesi Şablonu Düzenlemek için

1.  **Genel Yönetim** sayfasını açın ve sonra hak ilkesi şablonunu düzenlemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Hak ilkesi şablonları**'nı tıklatın.

3.  **Şablon** adının altında, düzenlenecek şablonun adını tıklatın.

4.  **Şablon kimliği** alanında **Şablon adı**, **Şablon açıklaması** ve **Hak isteme URL'si** alanlarındaki bilgileri uygun bir şekilde değiştirin.

5.  **Kullanıcılar ve gruplar** alanında, aşağıdakilerden birini veya daha fazlasını yapın:

    -   Kullanıcı veya grup eklemek için, **Kullanıcılar veya gruplar ekle** alanında, eklenecek belirli bir kullanıcı veya grubun geçerli e-posta adresini yazın, **Ekle**'yi tıklatın ve sonra **Geçerli kullanıcılar veya gruplar**'da adı seçin. **Haklar** alanında, seçilen kullanıcıya veya gruba verilecek tüm hakları seçin.
    -   Varolan kullanıcı ve grubun haklarını değiştirmek için, **Geçerli kullanıcılar veya gruplar**'da adı seçin ve sonra haklar onay kutularını uygun bir şekilde seçin veya temizleyin.
    -   Kullanıcı veya grubu kaldırmak için, **Geçerli kullanıcılar veya gruplar** alanında adı seçin ve sonra **Kaldır**'ı tıklatın.

6.  **Süre sonu ilkesi** alanında, içerik lisanslarının süresi sona erdiğinde ve yenilenmesi gerektiğinde değiştirilecek bilgileri uygun bir şekilde düzenleyin.

7.  **Uzatılan ilke** alanında, içerik lisanslarının nasıl uygulanacağını değiştirmek için, yazar haklarının devamlılığı, güvenilir tarayıcıların desteklenip desteklenmediği, içerikteki lisans devamlılığı ve herhangi bir uygulamaya özgü verinin zorlanması gibi bilgileri uygun bir şekilde düzenleyin.

8.  **İptal ilkesi** alanında, bu şablon kullanılarak oluşturulacak içerik için bir iptal listesinin gerekip gerekmeyeceğini seçin. **İptal iste**'yi seçerseniz, aşağıdaki ayarları uygun bir şekilde tamamlayın:

    -   **URL** alanına iptal listesi dosyasının yollanacağı URL'yi yazın Bağlantısı kesilmiş kullanıcıları ve dış kullanıcıları desteklemeniz gerekirse, bu URL'ye hem kurumsal ağdan hem de Internet'ten erişilebilmelidir. Daha fazla bilgi için bu konuda daha önce geçen "[İptal Uygulama](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)" bölümüne bakın.
    -   **İptal listesi yenileme aralığı**'nda, iptal listesinin geçerli kalacağı gün sayısını yazın. Kullanıcı iptal listesinin bu değerden daha eski bir kopyasına sahipse, içeriği kullanmak için güncelleştirilmiş bir iptal listesini edinmelidir.
    -   **İptal listesi ortak anahtarı**'nda, iptal listesi ortak anahtar dosyasının yolunu ve dosya adını yazın. Bu dosya hakkında daha fazla bilgi için, bu konuda daha önce geçen "İptal Listesine İmza Ekleme" bölümüne bakın.

    | ![](/security-updates/images/Cc747684.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | İptal işlemini yaparken dikkatli olun. Belirttiğiniz yenileme aralığına bağlı olarak iptal listesini düzenli olarak yenilemeniz gerekir; aksi takdirde liste otomatik olarak geçersiz hale gelir ve kullanıcıların o listeyi gerektiren içeriği kullanmasını önler. Kullanıcıların içeriği kullanmasını yanlışlıkla engellememek için iptal listesinin yenilenmesi için gerekli kıldığınız aralığı dikkatle değerlendirin. Daha fazla bilgi için bu konuda daha önce geçen "[İptali Yönetme](https://technet.microsoft.com/df732a7d-1fb0-4845-87ca-fab4bc5f98a0)" bölümüne bakın. |

9.  **Gönder**'i tıklatın.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.
