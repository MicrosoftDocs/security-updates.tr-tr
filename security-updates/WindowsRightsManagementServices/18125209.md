---
TOCTitle: Mobil Aygıtların Sertifikasını Etkinleştirmek için
Title: Mobil Aygıtların Sertifikasını Etkinleştirmek için
ms:assetid: '93ec088e-9056-4c3c-bd97-1173fb194578'
ms:contentKeyID: 18125209
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747603(v=WS.10)'
---

Mobil Aygıtların Sertifikasını Etkinleştirmek için
==================================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayardaki Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

Bu yordam, sadece kök sertifika kümesinde uygulanabilir.

Bu yordam, RMS korumalı içeriği kullanırken sunucu hizmetlerini temsil eden kullanıcı hesaplarını içeren bir kullanıcı grubu oluşturduğunuzu kabul eder.

Mobil Aygıtların Sertifikasını Etkinleştirme
--------------------------------------------

#### Mobil Aygıtların Sertifikasını Etkinleştirmek için

1.  Kök sertifika sunucunuzda, bir dosya sistemi tarayıcısı açın ve &lt;sistem sürücüsü&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification klasörüne gidin.

2.  Mobil aygıtların hak hesabı sertifikaları (RAC) alabilmelerini sağlamak için, MobileCertification.asmx dosyasını sağ tıklatın ve ardından **Özellikler**'i tıklatın.

3.  **Güvenlik** sekmesinde, **Ekle**'yi tıklatın ve bu kullanıcı kategorisi ve **RMS Service Group** için oluşturduğunuz grubu ekleyin.

4.  Grupların **İzinler** listesinde **Okuma** ve **Okuma & Yürütme** izinleri için **İzin Ver** onay kutusunu seçin ve daha sonra **Tamam**'ı tıklatın.
