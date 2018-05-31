---
TOCTitle: Super Users Grubu Ayarlamak için
Title: Super Users Grubu Ayarlamak için
ms:assetid: 'f2ef847e-2824-471f-9079-5c343094aba8'
ms:contentKeyID: 18125340
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747798(v=WS.10)'
---

Super Users Grubu Ayarlamak için
================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

RMS için Super users grubu olarak atanabilmesi için, grup öncelikle Active Directory'de bulunmalı ve o grubun özellikleri hesap adıyla aynı bir e-posta adresi (tam etki alanı adı olarak belirtilen) içermelidir.

Super Users Grubu Ayarlama
--------------------------

#### Super Users Grubu Ayarlamak için

1.  **Genel Yönetim** sayfasını açın ve sonra Super Users grubu oluşturmak istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Güvenlik ayarları**'nı tıklatın.

3.  **Super Users** alanında, Super Users grubu eklemek için **Etkinleştir**'i tıklatın.

4.  **Super Users grup adı**'nda, bu Active Directory ormanında bulunan ve üyelerine RMS tarafından korunan tüm belgeler için sahip hakları verilecek varolan bir grubun tam etki alanı adını *grup\_adı*@*etki\_alanı\_adı.com* biçiminde yazın ve **Kaydet**'i tıklatın.

    Super users grubunun haklarını devre dışı bırakmak için, **Devre dışı bırak**'ı tıklatın.

Bu yordamı uygulama hakkında daha fazla bilgi için bu konuda daha önce geçen "[Super Users Grubunu Kullanma](https://technet.microsoft.com/0febcb3e-7124-4e51-971a-1013b928d33b)" bölümüne bakın.
