---
TOCTitle: 'RMS''nin Yetkisini Almak için'
Title: 'RMS''nin Yetkisini Almak için'
ms:assetid: '8b563c25-17cd-4b9b-ae42-695497ab6439'
ms:contentKeyID: 18125196
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747665(v=WS.10)'
---

RMS'nin Yetkisini Almak için
============================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

| ![](/security-updates/images/Cc747665.Warning(WS.10).gif)Uyarý                                    |
|--------------------------------------------------------------------------------------------------------------|
| Bir sunucunun yetkisini aldığınızda, standart RMS yapılandırmasına geri yüklenemez. Bu yordam geri alınamaz. |

| ![](/security-updates/images/Cc747665.Warning(WS.10).gif)Uyarý                                                                                         |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS'nin yetkisini aldıktan sonra, başka bir RMS örneği yüklemeyi denemeden önce Program Ekle veya Kaldır kullanılarak RMS'nin tamamen kaldırılmış olması gerekir. |

RMS'nin Yetkisini Alma
----------------------

#### RMS'nin Yetkisini Almak için

1.  RMS'nin yetkisini almak istediğiniz sunucuya oturum açın.

2.  **Genel Yönetim** sayfasını açın ve ardından **RMS'yi bu Web sitesinde yönet** bağlantısını tıklatın.

3.  **Yönetim Girişi** sayfasında, **Güvenlik ayarları** bağlantısını tıklatın.

4.  **RMS'nin Yetkisini Alma** alanında, **RMS yüklemesinin yetkisinin alınmasını etkinleştir** onay kutusunu seçin ve ardından **Etkinleştir**'i tıklatın.

5.  İstendiğinde, RMS yüklemesi yetkisini sürekli olarak almak istediğinizi onaylamak için **Tamam**'ı tıklatın.
