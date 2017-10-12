---
TOCTitle: RMS Service Pack 1 Yüklemek için
Title: RMS Service Pack 1 Yüklemek için
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18125285
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747689(v=WS.10)'
---

RMS Service Pack 1 Yüklemek için
================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

RMS'yi yüklediğiniz bilgisayar, bir etki alanında üye sunucu veya bir etki alanı denetleyicisi olmalıdır. RMS'yi bir çalışma grubundaki bağımsız çalışan bir sunucuya dağıtamazsınız.

| ![](images/Cc747689.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| İlk kök sertifika sunucusunun hem yüklenmesini hem de hazırlanmasını tamamlayıncaya kadar RMS'yi başka herhangi bir sunucuda hazırlamayın. Yönergeler için bkz: [İlk Kök Sertifika Sunucusunu Sağlamak için](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)", [Lisans Sunucusu Sağlamak için](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)" veya "[Kümeye Sunucu Eklemek için](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)". |

| ![](images/Cc747689.Important(WS.10).gif)Önemli                                                                                                                                                                                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS SP1, etkin olarak RMS'nin daha önceki sürümünü çalıştıran bir sunucuya yüklenebilir. Bununla birlikte, RMS'nin yetkisini aldıysanız, yeni bir RMS SP1 örneği yüklemeyi denemeden önce Program Ekle veya Kaldır kullanılarak RMS'nin tamamen kaldırılmış olması gerekir. |

RMS Service Pack 1 Yükleme
--------------------------

#### RMS Service Pack 1 Yüklemek için

1.  RMS SP1 yüklemek istediğiniz sunucuya yerel Administrators grubunun bir üyesi olan etki alanı ile oturum açın.

2.  **Hoş Geldiniz** iletişim kutusu ekranda göründüğünde, yüklenecek yazılım listesini gözden geçirin ve sonra **İleri** seçeneğini tıklatın.

3.  **Lisans Sözleşmesi** iletişim kutusunda, sözleşmeyi inceleyin, **Kabul ediyorum**'u seçin ve sonra **İleri**'yi tıklatın.

4.  **Klasör**'de, varsayılan klasörü kabul edin veya yeni bir klasör belirleyin ve sonra **İleri**'yi tıklatın.

5.  **Yüklemeyi Onayla** iletişim kutusunda, yüklemeyi başlatmak için **Yükle** seçeneğini tıklatın.

6.  **Yükleme Tamamlandı** iletişim kutusu göründüğünde, **Kapat**'ı tıklatın.

    | ![](images/Cc747689.note(WS.10).gif)Not                                                        |
    |-----------------------------------------------------------------------------------------------------------------------------|
    | "Uygulama yeniden başlıyor" hata iletisi görünürse, Microsoft Internet Explorer'daki **Genel Yönetim** sayfasını yenileyin. |

RMS'yi komut isteminden de yükleyebilirsiniz. Yönergeler için bu konuda daha sonra yer alan "[RMS Sunucusunu Komut İsteminden Yükleme](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)" bölümüne bakın.
