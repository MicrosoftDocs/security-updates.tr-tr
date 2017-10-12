---
TOCTitle: RMS Proxy Ayarlarını Değiştirmek için
Title: RMS Proxy Ayarlarını Değiştirmek için
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18125179
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747594(v=WS.10)'
---

RMS Proxy Ayarlarını Değiştirmek için
=====================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

Proxy sunucusu kimlik doğrulaması yöntemleri hakkında daha fazla bilgi edinmek ve bu yöntemlerin Windows Server 2003'te nasıl çalıştığını görmek için bkz. Internet Information Services Yardımı.

RMS Proxy Ayarlarını Değiştirme
-------------------------------

#### RMS Proxy Ayarlarını Değiştirmek için

1.  **Genel Yönetim** sayfasını açın ve sonra **RMS'yi bu Web sitesinde yönet** bağlantısını tıklatın.

2.  **Küme Yönetimi**'nde, **Güvenlik Ayarları**'nı tıklatın.

3.  Daha önce RMS ile bir proxy sunucusu kullanmadıysanız **Bu bilgisayar Internet'e bağlanmak için proxy sunucu kullanır** onay kutusunu işaretleyin. Sayfada tamamlamanız gereken ek adımlar görünür.

4.  **Adres** kutusuna kullanmak istediğiniz proxy sunucusunun IP adresini veya DNS adını yazın.

5.  **Bağlantı noktası** kutusuna proxy sunucusunun Internet'e bağlanmak için kullandığı bağlantı noktası numarasını yazın.

6.  Yerel kaynaklara bağlanmak için proxy sunucusunu kullanmıyorsanız, **Yerel adresler için proxy sunucusunu atla** onay kutusunu seçin.

7.  Uygunsa, **Bu proxy sunucusu kimlik doğrulama gerektirir** onay kutusunu seçin.

    -   Listeden **Basit**, **Özet** ya da **Tümleşik Windows** kimlik doğrulama türlerinden birini seçin.
    -   **Kullanıcı adı** alanına, proxy sunucusu tarafından sorulduğunda verilecek olan kullanıcı adını yazın.
    -   **Parola** alanına, proxy sunucusu tarafından sorulduğunda verilecek olan parolayı yazın.
    -   **Parolayı onaylayın** alanında, girdiğiniz parolayı doğru yazdığınızı doğrulamak için yeniden yazın.
    -   Proxy sunucunuz Tümleşik Windows kimlik doğrulaması kullanıyorsa, **Etki alanı** alanına kullanıcının ait olduğu etki alanını yazın.

8.  **Gönder**'i tıklatın.
