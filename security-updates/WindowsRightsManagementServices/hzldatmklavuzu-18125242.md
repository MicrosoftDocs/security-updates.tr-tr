---
TOCTitle: Hızlı Dağıtım Kılavuzu
Title: Hızlı Dağıtım Kılavuzu
ms:assetid: 'b8fb69b6-3e0b-4836-8c05-8bd93f522a7c'
ms:contentKeyID: 18125242
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747735(v=WS.10)'
---

Hızlı Dağıtım Kılavuzu
======================

Bu kılavuz Service Pack 1 yüklü RMS çalıştıran bir sunucuyu hızlı bir şekilde kurmanıza yardımcı olma amacına yöneliktir. Böylece, RMS'yi değerlendirebilir ve kuruluşunuzda geniş ölçekli bir dağıtım yapmak isteyip istemediğinize karar verebilirsiniz.

**1. Adım – RMS için hazırlanma**

RMS, hizmeti kullanmadan önce yüklediğiniz ve yapılandırdığınız diğer bileşenlere bağımlıdır. Aşağıdaki adımları tamamladığınızda altyapınız RMS için temel gereksinimleri karşılayacaktır.

1.  Windows Server 2003 çalıştıran bir bilgisayarı yapılandırın ve sonra Active Directory etki alanına ekleyin. (Yalnızca bir tane sunucusu olan küçük kuruluşlarda, bu bilgisayar Active Directory'nin etki alanı denetleyicisi de olabilir. Ancak, bu durumda bilgisayar Windows Server 2003, Standard Edition; Windows Server 2003, Enterprise Edition; veya Windows Server 2003, Datacenter Edition kullanıyor olmalıdır. Windows Server 2003, Web Edition kullanan bir bilgisayar, etki alanı denetleyicisi olamaz.)
2.  Sunucuyu, **Uygulama Sunucusu** rolü için yapılandırın. Bunu yapmak için **Başlat**'ı tıklatın, **Denetim Masası**'nı çift tıklatın ve sonra **Program Ekle veya Kaldır**'ı çift tıklatın. **Program Ekle veya Kaldır**'da, **Windows Bileşenleri Ekle/Kaldır** seçeneğini tıklatın ve sonra **Uygulama Sunucusu**'nun altında aşağıdaki hizmetlerin etkinleştirilmiş olduğundan emin olun:
    -   **ASP.NET**
    -   **Internet Information Services (IIS)**
    -   **Message Queuing**

    Her hizmet için varsayılan seçenekleri kabul edin. Başka hiçbir yapılandırma gerekmez.
3.  Aşağıdaki veritabanı uygulamalarından birini kullanarak veritabanı sunucusunu yapılandırın:
    -   Microsoft® SQL Server 2000 SP3a. Bu, SQL Server 2000'in yerel bir yüklemesi veya aynı etki alanında bulunan uzak bir yükleme olabilir.
    -   Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A. Yerel bir yükleme olmalıdır. MSDE 2000'i [Microsoft Web sitesinden](http://go.microsoft.com/fwlink/?linkid=17799) (http://go.microsoft.com/fwlink/?LinkID=17799) yükleyebilirsiniz.

    Microsoft SQL Server Desktop Engine, kuruluş çapındaki veritabanını tam olarak çalıştırmak ve desteklemek için gereken araçları içermediğinden, RMS veritabanlarını desteklemek amacıyla yalnızca sınama ortamlarında kullanılması önerilir. Buna ek olarak, MSDE uzak ağları desteklemediğinden, bunu RMS ile aynı sunucuya yüklemeniz gerekir ve RMS kümesine başka RMS sunucuları yükleyemezsiniz. Microsoft SQL Server Desktop Engine kullanım koşullarında, Microsoft SQL Server Desktop Engine veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınız belirtilir. Bu kısıtlama nedeniyle, RMS yapılandırma veritabanını yedekleyemez ve geri yükleyemez, günlük bilgilerini görüntüleyemez veya yapılandırma veritabanında depolanan verileri doğrudan değiştiremezsiniz.
4.  Kullanıcılar intranetiniz üzerinden bu hizmete bağlanmaya çalıştığında bu hizmetin adının ne olarak bilinmesini istediğinize karar verin (örneğin, http://sertifika.contoso.com). Etki Alanı Adı Sistemini (DNS), bu URL'yi RMS bilgisayarının IP adresine çözümlemek için yapılandırın. Diğer DNS bölgelerindeki istemcilerin RMS sunucusunun veya sunucularının IP adreslerini çözümleyebileceğinden emin olmak amacıyla küme URL'si için tam DNS etki alanı adı kullanmalısınız.
5.  RMS ile kullanmak üzere bir yönetici hesabı oluşturun.
6.  RMS SP1 yüklemeye hazırsınız. Bu adımla ilgili daha fazla yönerge için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “RMS Service Pack 1'i Yüklemek için” konusuna bakın.

**Sık Kullanılan İsteğe Bağlı özellikler**

Aşağıdaki özellikler isteğe bağlıdır; bunları kullanmayı seçerseniz RMS'yi yükleme ve sağlama işlemine başlamadan önce gerekli hazırlığı yaptığınızdan emin olun:

-   RMS'yi, özel anahtarları depolamak için donanım güvenlik modülünü (HSM) kullanmak üzere yapılandırabilirsiniz. Donanım güvenlik modülü kullanmak istiyorsanız, sürücülerin düzgün yapılandırıldığından ve güvenlik uzayının tanımlandığından emin olun.
-   RMS bilgisayarınız Internet'e bağlanabiliyorsa, sağlama işlemi sırasında sunucu lisans sertifikasını otomatik olarak karşıdan yükleyebilirsiniz. Kuruluşunuz Internet'e bağlanmak için bir proxy sunucusu kullanıyorsa, Internet Explorer'da proxy ayarlarını, kimlik doğrulama gereksinimleri de dahil olmak üzere doğrulayın ve daha sonra kullanmak üzere kaydedin.
-   RMS'yi bir etki alanı denetleyicisinde çalıştıracaksanız ve RMS hizmetlerini çalıştırmak için bir kullanıcı hesabı kullanmayı planlıyorsanız, kullanıcı hesabı izninin yerel olarak oturum açmasına olanak sağlamak için Etki Alanı Denetleyicisi Güvenlik İlkesi'nin yapılandırılmış olduğundan emin olun. Etki Alanı Denetleyicisi Güvenlik İlkesi'nin nasıl yapılandırılacağı hakkında daha fazla bilgi için bkz. Windows Server 2003 Yardım ve Destek Merkezi.

**2. Adım - İlk RMS sunucusunun hazırlanması**

Hazırlama, bir Web sitesini RMS ile yapılandırma işlemidir; böylece kullanıcılar hizmeti kullanmaya başlayabilir. Kuruluşunuzun kök sertifika sunucusunu yapılandırmak için aşağıdaki adımları izleyin:

1.  Bilgisayarda yerel yönetici ayrıcalıklarına sahip bir etki alanı kullanıcısı olarak oturum açın. RMS'yi etki alanı denetleyicisine yüklüyorsanız, etki alanı yöneticisi olarak oturum açın.
2.  **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gelin, **Windows RMS**'nin üzerine gelin ve sonra **Genel Yönetim** sayfasını açmak için **Windows RMS Yönetimi**'ni tıklatın. Bu sayfa bu sunucuda bulunan Web sitelerini listeler.
3.  RMS ile hazırlamak için istediğiniz Web sitesini tıklatın ve sonra **RMS'yi bu Web sitesinde hazırla**'yı tıklatın. Sayfa açıldığında, sayfanın en üstünde **RMS Kök Sertifika Sunucusunu Hazırla** ifadesi görünür.
4.  Sayfayı kuruluşunuza ait bilgilerle tamamlayın.
    -   **Küme URL**'si kutusunda, önceki yordamdaki 4. adımda yapılandırdığınız hizmet adını yazın (sertifika.contoso.com gibi). Yüklemenizle SSL kullanmak istiyorsanız, protokol listesinde HTTPS protokolünü tıklatın. Bunu yaptığınızda, SSL etkinleştirilir; ancak, bu seçimi yapmak RMS Web hizmetleri için SSL'yi gerektirmez. Bunu IIS aracılığıyla ayrıca yapılandırmalısınız.
    -   Sunucunuz Internet'e proxy sunucu üzerinden bağlıysa, **RMS Proxy Ayarları** alanında, önceki yordamın isteğe bağlı özellikler kısmında açıklandığı gibi Internet Explorer'dan kaydettiğiniz bilgilerle bölümü tamamlayın.
    -   **Sunucu Internet Bağlantısı** alanında, sunucunun Internet kullanarak Microsoft Kayıt Hizmeti'ne bağlanmasını ve sağlama işlemi sırasında sunucu lisans sertifikası almasını istiyorsanız **Çevrimiçi** seçeneğini işaretleyin. Microsoft Kayıt Hizmetine el ile bağlanmak, sunucu lisans sertifikası yüklemek ve RMS hazırlığından sonra almak istiyorsanız **Çevrimdışı** seçeneğini işaretleyin.
5.  **Gönder**'i tıklatın.
    Yaklaşık 60-90 saniye içinde hazırlama işlemi başarıyla tamamlanır ve yeni hazırlanmış RMS sunucunuzu yönetebileceğiniz **Genel Yönetim** sayfasına geri dönersiniz.
6.  RMS sunucusunun **Yönetim** giriş sayfasını açmak için **Genel Yönetim** sayfasında **RMS'yi bu Web sitesinde yönet**'i seçin.
    4. adımda Sunucu Internet Bağlantısı için Çevrimdışı seçeneğini işaretlediyseniz, devam etmeden önce "El ile Kök Sertifika Sunucusu Kaydettirmek için" yordamını tamamen uygulayın.
7.  Yönetim giriş sayfasında, **RMS hizmet bağlantı noktası** bağlantısını tıklatın.

| ![](images/Cc747735.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu yordamdaki sonraki adım olan hizmet bağlantı noktası kaydettirme, Active Directory ormanı Yapılandırma kapsayıcısındaki Hizmetler kapsayıcısı altında kapsayıcı nesnesi oluşturmak için yeterli ayrıcalıklara sahip bir etki alanı hesabının kullanılmasını gerektirir. Önceden tanımlanmış güvenlik grubu olan **Enterprise Admins** gerekli ayrıcalıklara sahip hesaba bir örnektir. |

1.  **RMS hizmet bağlantı noktası** sayfasında, **URL'yi Kaydet** düğmesini tıklatın. Bu, RMS'nin hizmet bağlantı noktasını Active Directory'de kaydeder; böylece RMS etkinleştirilmiş uygulamalar RMS lisans, etkinleştirme proxy ve sertifika hizmetlerini bulabilir. 

**3. Adım - Windows RMS'yi sınama**

RMS'yi tam olarak kullanabilmeniz için öncelikle, istemci bilgisayarlara Microfost Windows Rights Management Services istemcisi ve RMS etkin bir uygulama yüklemeniz gerekir. Kullanıcılar Active Directory etki alanının üyesi olmalıdır ve istemci bilgisayarlar etki alanına eklenmelidir. Ayrıca, etki alanı kullanıcılarının tümü Active Directory'de tanımlanmış e-posta adreslerine sahip olmalıdır. RMS'yi sınamak için:

1.  İstemci bilgisayarda geçerli bir etki alanı kullanıcısı olarak oturum açın.
2.  Service Pack 1 için RMS istemcisi yükleyin.
3.  RMS etkinleştirilmiş bir uygulama yükleyin.
4.  RMS korumalı bir dosya oluşturun, herkes için dosyaya salt okuma hakkı verin ve sonra dosyayı kullanıcıların tam erişime sahip olduğu bir paylaşılan klasöre kaydedin.
5.  Bilgisayara farklı bir kullanıcı olarak oturum açın. Dosyayı açın ve değişiklik yapmaya çalışın. RMS düzgün şekilde yüklenmişse, dosyada değişiklik yapamazsınız.
