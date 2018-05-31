---
TOCTitle: Kök Sertifika Sunucusunun Kaydettirilmesi
Title: Kök Sertifika Sunucusunun Kaydettirilmesi
ms:assetid: '3f69d25e-ecae-447f-b741-a819c8cf6227'
ms:contentKeyID: 18125061
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720250(v=WS.10)'
---

Kök Sertifika Sunucusunun Kaydettirilmesi
=========================================

Her RMS yüklemesinin en az bir kök sertifika sunucusu içermesi gerekir ve söz konusu yükleme, isteğe bağlı olarak kümedeki başka kök sertifika sunucularını içerebilir. Yüklediğiniz ilk kök sertifika sunucusunun kök sunucu lisans sertifikası alması için Microsoft Kayıt Hizmeti'ne kaydettirilmesi gerekir. Bu sertifika bir RMS uygulamasında güven hiyerarşisinin temelini oluşturur.

Kök sunucu lisans sertifikası aşağıdaki yöntemlerden biri kullanılarak elde edilebilir. RMS sunucunuzun sağlama bilgilerini tamamladıktan sonra kullanacağınız yöntemi seçebilirsiniz:

-   **Çevrimiçi kayıt**. Kök sertifika sunucunuz Internet'e bağlanabiliyorsa sağlama işlemi sırasında otomatik olarak bir sunucu lisans sertifikası alabilirsiniz. Bu varsayılan yöntemdir.
-   **Çevrimdışı kayıt**. Kök sertifika sunucunuz Internet'e bağlı değilse sunucunuzu sağlama işlemi işlemi tamamlandıktan sonra el ile kaydettirebilirsiniz. Bunu yapmak için, sunucu lisans sertifikası elde etmek için bu sunucudan Internet bağlantısı olan diğer bir bilgisayara taşıyabileceğiniz bir kayıt isteği vermeniz ve daha sonra Microsoft Kayıt Hizmetine göndermeniz gerekir. Sağlama sırasında çevrimdışı kayıt seçeneğini tercih ettiyseniz RMS sağlama işlemini tamamlayacak, fakat diğer bilgisayardan edinilen sunucu lisans sertifikası alınana kadar kullanılamayacaktır. Daha fazla bilgi için, bu konunun daha sonraki bölümlerinde yer alan "[Kök Sertifika Sunucusunu El İle Kaydettirmek için](https://technet.microsoft.com/aecdebb5-b28b-4b58-937a-392bb6ce9643)" konusuna bakın.

Kayıt isteği aşağıdaki bilgileri içerir:

-   İptal bilgileri. RMS yüklemesinin standart iptal mi yoksa özel (üçüncü taraf) iptal mi kullanacağı bilgisi. Üçüncü taraf Microsoft iptali kullanılıyorsa, iptal yetkilisinin ortak anahtarı da eklenir.
-   Sertifika Ortak Anahtarı. Sunucu lisans sertifikasının ortak anahtarı. Bu ortak anahtar RMS sunucusunda üretilir ve sunucu lisans sertifikası almak için Microsoft Kayıt Hizmetine gönderilir.
-   SKU. Resmi RMS SKU başlığı.
-   Sürüm RMS sürüm numarası.
-   URL. RMS sunucu kümesi taban URL'si..

Microsoft Kayıt Hizmeti kayıt isteğine yanıt verdiğinde, aşağıdaki bilgileri RMS sunucusuna XML biçiminde gönderir:

-   Sunucu Lisans Sertifikası
-   İmzalayan yetkililerin sertifika zinciri.

RMS kök sertifika sunucusunun çevrimiçi veya çevrimdışı yöntem kullanılarak kaydettirilmesinden bağımsız olarak, aktarılan bilgiler aynıdır. Hangi yöntem kullanılırsa kullanılsın, ek bilgi toplanmaz.

| ![](/security-updates/images/Cc720250.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Çevrimdışı kayıt yaptırmayı seçtiyseniz ve bilgisayarınız Internet'e bağlanmak ve sunucu lisans sertifikası istemek için Windows Server 2003 veya Windows XP Service Pack 2 gibi ileri tarayıcı güvenlik yapılandırması kullanıyorsa, servis lisans sertifikasının karşıdan yüklenmesini sağlamak için Kayıt Hizmet Web sitesinin URL'sini Güvenilir Siteler bölgesine eklediğinizden emin olun. Bu URL, https://activation.drm.microsoft.com şeklindedir. Çevrimdışı kayıt işlemi yapıyorsanız, Microsoft Kayıt Hizmetine kayıt isteği göndermek için kullandığınız bilgisayara tüm en son sertifika güncellemelerinin yüklenmiş olduğundan emin olun. Microsoft Kayıt Hizmetleri SSL sertifikası, Windows Server 2003 çalıştıran tüm bilgisayarlarda varsayılan olarak güvenilen GTE Cyber Trust Kök CA'sıdır. Çevrimdışı kayıt işlemi yapıyorsanız, RMS istemcilerinin kayıt gerçekleşene kadar lisanlar için RMS sunucularına bağlanmaya çalışmadıklarından emin olun. İstemciler Web hizmetlerine kaydettirilmemiş bir RMS sunucusuna bağlanmaya çalışırsa hata verir ve kullanılmaz bir hal alırlar. İstemcilerin RMS sunucusuna bağlanmaya çalışmamalarını sağlayamıyorsanız, en iyi uygulama olarak kayıt işlemi bittikten sonra oluşan hata durumlarını ortadan kaldırmak için IIS'i sıfırlamanız gerekir. |
