---
TOCTitle: Yönetim İlgili Kişisini Belirtmek için
Title: Yönetim İlgili Kişisini Belirtmek için
ms:assetid: '31777458-5530-4ae0-ac1f-131b3d98dd35'
ms:contentKeyID: 18125049
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720237(v=WS.10)'
---

Yönetim İlgili Kişisini Belirtmek için
======================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

Bu yordamda belirtilen yöneticinin kök sertifika sunucusunda yerel yönetici olması gerekir, çünkü oturum açmış kullanıcının lisans sunucusu hazırlamak için kök sertifika sunucusunda izinlere sahip olması gerekir. Lisans sunucusu hazırlamaya çalışan kullanıcının bu dosyada izinlere sahip olmaması durumunda, kullanıcı bu işlemde atanmış yöneticiye, kullanıcı hesabına gerekli izinleri vermesine yönelik bir istek gönderebilir. Daha fazla bilgi için bu konuda daha önce yer alan "[Alt Kayıt Hizmeti Dosyasında İzinler Ayarlama](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)" bölümüne bakın.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Yönetim İlgili Kişisini Belirtme
--------------------------------

#### Yönetim İlgili Kişisini Belirtmek için

1.  **Genel Yönetim** sayfasını açın ve sonra yönetim ilgili kişisini belirtmek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Sertifika ayarları**'nı tıklatın.

3.  **Yönetim ilgili kişisi** alanına, lisans sunucusunun sağlanması sırasında oluşabilecek alt kayıt sorunlarında başvurulacak yöneticinin e-posta adresini *kullanıcı\_adı*@*etki\_alanı\_adı.com* biçiminde yazın.

4.  Sayfanın altında, **Gönder**'i tıklatın.
