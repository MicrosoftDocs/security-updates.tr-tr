---
TOCTitle: Uygulamaları Dışlamak için
Title: Uygulamaları Dışlamak için
ms:assetid: '422f2ddd-bcf4-45f1-905a-b8bad30fd7dd'
ms:contentKeyID: 18125069
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720262(v=WS.10)'
---

Uygulamaları Dışlamak için
==========================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Dışlama ilkeleri, kullanım lisansı korunan içeriğe bağlı olduğunda istemci tarafından uygulanır.

Uygulamaları Dışlama veya Uygulamaları Dışlamayı Durdurma
---------------------------------------------------------

#### Uygulamaları Dışlamak için

1.  **Genel Yönetim** sayfasını açın ve sonra hak korumalı içerikle uygulamaların hangi sürümlerinin kullanılabileceğini denetlemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetimbağlantıları** alanında, **Dışlama ilkeleri**'ni tıklatın.

3.  **Uygulamayı dışlama** alanında, RMS korumalı uygulamayı veya bileşeni dışlamak için **Etkinleştir**'i tıklatın.

    Uygulamayı dışlamayı devre dışı bırakmak için, **Devre dışı bırak**'ı tıklatın.

4.  Dışlanacak uygulamanın veya bileşenin dosya adını yazın, dışlanacak en düşük ve en yüksek sürümleri (*x*.*x*.*x*.*x* biçiminde) yazın ve sonra **Bu uygulamayı dışla**'yı tıklatın.

    Uygulamayı (veya bileşeni) dışlama listesinden silmek için, dosya adını seçin ve sonra **Seçilen uygulamaları dışlama listesinden sil**'i tıklatın.

    | ![](/security-updates/images/Cc720262.note(WS.10).gif)Not                                                                                                                                                                                                                                                                        |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | RMS, uygulama sürümünün 4 basamaklı, nokta ile ayrılmış biçimde olmasını gerektirir (\#.\#.\#.\# ). Bununla bazı, belirli uygulamalar, uygulama sürümünü 2 veya 3 basamaklı, nokta ile ayrılmış sayılarla belirtir. Bu durumda, sürüm numarasını RMS'nin gerektirdiği biçime uyarlamak için uygun olacak şekilde, .0 eklemeniz gerekebilir. |

#### Uygulamaları Dışlamayı Durdurmak için

1.  **Genel Yönetim** sayfasını açın ve sonra hak korumalı içerikle uygulamaların hangi sürümlerinin kullanılabileceğini denetlemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetimbağlantıları** alanında, **Dışlama ilkeleri**'ni tıklatın.

3.  **Uygulamayı dışlama** alanında **Devre Dışı Bırak**'ı tıklatın.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)" bölümüne bakın.
