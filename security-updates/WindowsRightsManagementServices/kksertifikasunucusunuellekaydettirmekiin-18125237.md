---
TOCTitle: Kök Sertifika Sunucusunu El İle Kaydettirmek için
Title: Kök Sertifika Sunucusunu El İle Kaydettirmek için
ms:assetid: 'aecdebb5-b28b-4b58-937a-392bb6ce9643'
ms:contentKeyID: 18125237
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747727(v=WS.10)'
---

Kök Sertifika Sunucusunu El İle Kaydettirmek için
=================================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayardaki Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. İyi bir güvenlik yöntemi olarak, bu yordamı uygulamak için Farklı çalıştır'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Çevrimdışı kayıt işlemi yapıyorsanız, RMS istemcilerinin kayıt gerçekleşene kadar lisanlar için RMS sunucularına bağlanmaya çalışmadıklarından emin olun. İstemciler Web hizmetlerine kaydettirilmemiş bir RMS sunucusuna bağlanmaya çalışırsa hata verir ve kullanılmaz bir hal alırlar. İstemcilerin RMS sunucusuna bağlanmaya çalışmamalarını sağlayamıyorsanız, en iyi uygulama olarak kayıt işlemi bittikten sonra oluşan hata durumlarını ortadan kaldırmak için IIS'i sıfırlamanız gerekir.

Çevrimdışı kayıt yaptırmayı seçtiyseniz ve bilgisayarınız Internet'e bağlanmak ve sunucu lisans sertifikası istemek için Windows Server 2003 veya Windows XP Service Pack 2 gibi ileri tarayıcı güvenlik yapılandırması kullanıyorsa, servis lisans sertifikasının karşıdan yüklenmesini sağlamak için Kayıt Hizmet Web sitesinin URL'sini Güvenilir Siteler bölgesine eklediğinizden emin olun. Bu URL, https://activation.drm.microsoft.com şeklindedir.

Çevrimdışı kayıt işlemi yapıyorsanız, Microsoft Kayıt Hizmetine kayıt isteği göndermek için kullandığınız bilgisayarın sertifika alanında GTE Cyber Trust Root CA yüklenmiş olduğundan emin olun. Bu sertifika yetkilisi Windows Server 2003 kullanan bilgisayarlarda varsayılan değer olarak güvenilirdir. Bilgisayarınız farklı bir Windows sürümü kullanıyorsa, Windows Güncelleme'den son sertifika güncellemelerini yükleyerek bu sertifika yetkilisine (CA) güvenebilirsiniz.

Kök Sertifika Sunucusunu El İle Kaydettirmek için
-------------------------------------------------

#### Kök Sertifika Sunucusunu El İle Kaydettirmek için

1.  Kök sertifika sunucusu olmasını istediğiniz bir sunucuya RMS yükledikten sonra **Genel Yönetim** sayfasını açın, kök sunucu lisans sertifikası almak istediğiniz Web sitesinin yanındaki **RMS'yi bu Web Sitesinde Yönet**'i tıklatın.

2.  **Küme kaynakları** alanında **Kaydet**'i tıklatın. **Kaydet** iletişim kutusu açılır.

3.  **Çevrimdışı** seçeneğini seçin ve **Gönder** düğmesini tıklatın. **Dosya Yükleme** iletişim kutusu görünür.

4.  **Kaydet**'i tıklatın. **Farklı kaydet** iletişim kutusu görünür.

    | ![](images/Cc747727.note(WS.10).gif)Not                                                                                        |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | **Karşıdan Dosya Yükleme** iletişim kutusunda **Aç**'ı tıklatmayın. **Aç**'ı tıklatırsanız bir hata mesajı görüntülenir ve kayıt istek dosyası kaydedilmez. |

5.  Kayıt isteğini bir dosyaya göndermek için **Kaydet**'i tıklatın. Dosya varsayılan olarak *Sunucu\_adı*EnrollRequest.xml adıyla masaüstüne kaydedilir, buradaki *sunucu\_adı* yerine, RMS sunucunuzun adı konur. İstediğiniz konumu **İçine kaydet** aşağı açılır menüsünden seçerek dosyayı başka bir konuma kaydedebilirsiniz. **Dosya adı** bölümüne yeni bir giriş yaparak dosyaya varsayılandan farklı bir isim verebilirsiniz.

6.  Kayıt istek dosyasını kaydettiğinizde **Karşıdan yükleme tamamlandı** iletişim kutusu görünür. Dosyadaki XML kodunu görüntülemek için **Aç**'ı tıklatabilirsiniz, fakat dosyaya herhangi bir değişiklik yapmayın. Dosyanın saklandığı klasörü açmak için **Klasör Aç**'ı tıklatın. Dosyaya göz atmayı ve yerini doğrulamayı bitirdiyseniz **Kapat**'ı tıklatın.

7.  Kayıt istek dosyasını Internet'e bağlanabilen bir bilgisayara aktarın ve [Kayıt Hizmeti Web sitesine]() gidin.

8.  Sunucu lisans sertifikası almak içim Web sitesindeki yönergeleri izleyin.

9.  Sunucu lisans sertifikasını bu kök sertifika sunucusuna geri taşıyın.

10. **Küme kaynakları** alanında **Kaydet**'i tıklatın. **Kaydet** iletişim kutusu açılır.

11. **Kayıt** iletişim kutusunda **Gözat** düğmesini tıklatın, karşıdan yüklediğiniz sunucu lisans sertifikasını bulun ve **Al** düğmesini tıklatın.

12. Bu sertifikayı almak istediğinizi onaylamak için **Evet**'i tıklatın.

13. **Küme kaynakları** alanı sunucu lisans sertifikasını gösterecek şekilde güncellenecektir.
