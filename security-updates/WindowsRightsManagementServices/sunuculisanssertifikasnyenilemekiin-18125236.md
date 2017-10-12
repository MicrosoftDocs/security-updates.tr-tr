---
TOCTitle: Sunucu Lisans Sertifikasını Yenilemek için
Title: Sunucu Lisans Sertifikasını Yenilemek için
ms:assetid: 'affce9cf-8b46-4293-8e1c-ee06f2ca6537'
ms:contentKeyID: 18125236
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747636(v=WS.10)'
---

Sunucu Lisans Sertifikasını Yenilemek için
==========================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Çevrimdışı yenilemeyi seçtiyseniz ve bilgisayarınız Internet'e bağlanmak ve sunucu lisans sertifikası istemek için Windows Server 2003 veya Windows XP Service Pack 2 gibi gelişmiş bir tarayıcı güvenlik yapılandırması kullanıyorsa, hizmet lisans sertifikasının karşıdan yüklenmesini sağlamak için Kayıt Hizmeti Web sitesinin URL'sini Güvenilen Siteler bölgesine eklediğinizden emin olmalısınız. Bu URL, https://activation.drm.microsoft.com şeklindedir.

Çevrimdışı kayıt işlemi yapıyorsanız, Microsoft Kayıt Hizmetine kayıt isteği göndermek için kullandığınız bilgisayarın sertifika alanında GTE Cyber Trust Root CA yüklenmiş olduğundan emin olun. Bu sertifika yetkilisi Windows Server 2003 kullanan bilgisayarlarda varsayılan değer olarak güvenilirdir. Bilgisayarınız farklı bir Windows sürümü kullanıyorsa, Windows Güncelleme'den son sertifika güncellemelerini yükleyerek bu sertifika yetkilisine (CA) güvenebilirsiniz.

Sunucu Lisans Sertifikasını Yenileme
------------------------------------

#### Sunucu Lisans Sertifikasını Yenilemek için

1.  **Genel Yönetim** sayfasını açın ve sonra sertifikayı yenilemek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim** sayfasındaki **Küme kaynakları** alanında, **Yenile** düğmesini tıklatın. Yenile iletişim kutusu açılır.

3.  Sunucunuz İnternet'e bağlıysa, sunucu lisans sertifikanızı otomatik olarak yenilemek için **Çevrimiçi** seçeneğini seçin ve **Yenile**'yi tıklatın.

4.  Sunucunuz İnternet'e bağlı değilse, **Çevrimdışı** seçeneğini seçin ve **Ver** düğmesini tıklatın. **Dosya Yükleme** iletişim kutusu görünür.

5.  **Kaydet**'i tıklatın. **Farklı kaydet** iletişim kutusu görünür.

    | ![](images/Cc747636.note(WS.10).gif)Not                                                                                        |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | **Karşıdan Dosya Yükleme** iletişim kutusunda **Aç**'ı tıklatmayın. **Aç**'ı tıklatırsanız bir hata mesajı görüntülenir ve kayıt istek dosyası kaydedilmez. |

6.  Yenileme isteğini bir dosyaya göndermek için **Kaydet**'i tıklatın. Dosya varsayılan olarak *Sunucu\_adı*RenewalRequest.xml adıyla masaüstüne kaydedilir, buradaki *sunucu\_adı* yerine, RMS sunucunuzun adı konur. İstediğiniz konumu Kayıt yeri açılan menüsünden seçerek dosyayı başka bir konuma kaydedebilirsiniz. **Dosya adı** bölümüne yeni bir giriş yaparak dosyaya varsayılandan farklı bir isim verebilirsiniz.

7.  Yenileme dosyasını kaydettiğinizde **Karşıdan yükleme tamamlandı** iletişim kutusu görünür. Dosyadaki XML kodunu görüntülemek için **Aç**'ı tıklatabilirsiniz, fakat dosyaya herhangi bir değişiklik yapmayın. Dosyanın saklandığı klasörü açmak için **Klasör Aç**'ı tıklatın. Dosyaya göz atmayı ve yerini doğrulamayı bitirdiyseniz **Kapat**'ı tıklatın.

8.  Yenileme dosyasını İnternet'e bağlanabilen bir bilgisayara taşıyın ve [Kayıt Hizmeti Web sitesine]() gidin (https://go.microsoft.com/fwlink/?LinkId=25828).

9.  Sunucu lisans sertifikası almak içim Web sitesindeki yönergeleri izleyin.

10. Sunucu lisans sertifikasını bu kök sertifika sunucusuna geri taşıyın.

11. **Küme** kaynakları alanında **Yenile**'yi tıklatın. **Yenile** iletişim kutusu açılır.

12. **Yenile** iletişim kutusunda **Gözat** düğmesini tıklatın, karşıdan yüklediğiniz sunucu lisans sertifikasını bulun ve **Al** düğmesini tıklatın.

13. Bu sertifikayı almak istediğinizi onaylamak için **Evet**'i tıklatın.

14. Sunucu lisans sertifikası başarıyla yenilendiğinde, **Küme kaynakları** alanı sunucu lisans sertifikasının yeni son kullanım tarihini gösterecek şekilde güncellenir.

İptal işlemi hakkında daha fazla bilgi için bu konuda daha önce geçen "[Sunucu Lisans Sertifikalarını Yönetme](https://technet.microsoft.com/549979ad-13ee-4abc-8281-3e002a5a9561)" bölümüne bakın.
