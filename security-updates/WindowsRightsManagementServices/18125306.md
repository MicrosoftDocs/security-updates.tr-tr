---
TOCTitle: Hak Hesabı Sertifikalarını Dışlamak için
Title: Hak Hesabı Sertifikalarını Dışlamak için
ms:assetid: 'e5cd9dec-ac29-437e-8515-dc697ec75edf'
ms:contentKeyID: 18125306
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747785(v=WS.10)'
---

Hak Hesabı Sertifikalarını Dışlamak için
========================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Bu koşullar, kullanım lisansı korunan içeriğe bağlı olduğunda istemci tarafından zorlanır.

Hak Hesabı Sertifikalarını Dışlama
----------------------------------

#### Hak Hesabı Sertifikalarını Dışlamak için

1.  **Genel Yönetim** sayfasını açın ve sonra hak hesap sertifikasını dışlamak istediğiniz Web sitesinin yanında, **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Dışlama ilkeleri**'ni tıklatın.

3.  Kullanıcının hak hesabı sertifikasını dışlamak için, hak hesabı sertifikası dışlama alanında **Etkinleştir**'i tıklatın.

4.  Dışlanacak hesap sertifikasını belirtme yöntemini seçin.

    -   Hesap sertifikasını kullanıcı adına göre dışlamak için, dışlanacak hak hesabı sertifikasının **Kullanıcı adı**'nı tıklatın, dışlanacak kullanıcının adını yazın (*kullanıcı\_adı*@*etki\_alanı\_adı.com* biçiminde) ve sonra **Ekle**'yi tıklatın. Bu seçeneği Active Directory kullanıcı hesapları olmayan iç kullanıcıların hesap sertifikalarını dışlamak için kullanın.
    -   Hesap sertifikasını ortak anahtarına göre dışlamak için, dışlanacak hak hesabı sertifikasının **Ortak anahtar dizesi** bölümünü tıklatın, uygun hak hesabı sertifikası ortak anahtar dizesini yazın ve sonra **Ekle**'yi tıklatın. Bu seçeneği Active Directory kullanıcı hesapları olmayan dış kullanıcıların hesap sertifikalarını dışlamak için kullanın.

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Not                                                                                                                                                                                                                             |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Hesap sertifikasını dışlama listesinden silmek için, listedeki dışlanan hak hesap sertifikasını tıklatın ve sonra **Seçilen ortak anahtarları dışlama listesinden sil**'i tıklatın. O özel hesap sertifikasına sahip kullanıcı artık bu sunucudan RMS korumalı içerik için lisans alabilecektir. |

    | ![](/security-updates/images/Cc747785.note(WS.10).gif)Not                           |
    |------------------------------------------------------------------------------------------------|
    | Hak hesabı sertifikalarını dışlamayı devre dışı bırakmak için **Devre dışı bırak**'ı tıklatın. |

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Hak Hesabı Sertifikalarını Dışlama](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)" bölümüne bakın.
