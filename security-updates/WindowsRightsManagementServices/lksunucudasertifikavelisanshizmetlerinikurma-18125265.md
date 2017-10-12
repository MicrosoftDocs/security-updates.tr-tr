---
TOCTitle: İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma
Title: İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma
ms:assetid: 'cce29a2f-984f-48ed-9187-0eb68286ec5b'
ms:contentKeyID: 18125265
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747756(v=WS.10)'
---

İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma
===================================================

RMS'yi bir ormanda kurmak için, ilk olarak bir sunucuya yükleyin ve bunu yapılandırın. Dağıttığınız ilk sunucu kök sertifika sunucusudur. Bu sunucu hem sertifika hem de lisans desteği sağlar ve tek sunuculu yapılandırmada tek sunucu olarak veya kök sertifika kümesinin başlangıç sunucusu olarak kullanılabilir.

Ek RMS Sunucularını Yükleme ve Sağlama için Gerekli Roller, İzinler ve Haklar
-----------------------------------------------------------------------------

RMS'yi yüklemek için yerel yönetici ayrıcalıklarına sahip bir hesabı kullanarak oturum açmanız gerekir. Bununla birlikte, Active Directory'nin RMS'nin kimliğini doğrulayabilmesi için etki alanına geçerli bir etki alanı hesabını kullanarak oturum açmış olmanız gerekir. RMS'yi, Active Directory altyapınızın Windows 2000 yerel modunu kullandığı bir ortamda dağıtıyorsanız, Active Directory grup üyeliğini genişletmeye çalışırken RMS Active Directory nesnelerindeki memberOf özniteliğini okuyamayabilir. RMS'nin memberOf özniteliğini okumasını sağlamak için RMS hizmet hesabı, ormanınızdaki Windows 2000 öncesi uyumlu erişim grubunun üyesi olan bir etki alanı hesabı olmalıdır. Gizli üyelikleri olan gruplar dağıttıysanız RMS hizmet hesabını gizli üyelikleri okumasına olanak tanıyan izinlerle yapılandırmanız gerekir.

| ![](images/Cc747756.note(WS.10).gif)Not                    |
|-----------------------------------------------------------------------------------------|
| RMS hizmet hesabı, RMS'yi yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. |

Başlangıç Sunucusu için Yükleme ve Sağlama İşlemleri
----------------------------------------------------

RMS sunucusunu dağıtma işlemi iki adımdan oluşur. İlk olarak, RMS sunucu yazılımının IIS, Message Queuing ve ASP.NET gibi tüm destekleyici yazılımlarla birlikte yüklenmesi gerekir. Yükleme hakkında daha fazla bilgi için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “RMS Service Pack 1'i Yüklemek İçin” konusuna bakın.

| ![](images/Cc747756.note(WS.10).gif)Not                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS komut isteminden de yüklenebilir. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "RMS'yi Komut İsteminden Yükleme" konusuna bakın. |

RMS'yi sunucuya yükledikten sonra, RMS'yi sunucu üzerindeki tek bir Web sitesinde kullanılmak üzere yapılandırmanız gerekir. Bu Web sitesini yapılandırdığınızda, Web sitesinin ayarlarının birçoğu değiştirilir ve sanal dizinler eklenir. Bu değişiklikler hakkında daha fazla bilgi için, bu belge grubundaki "RMS Teknik Başvuru Kılavuzu" bölümünde bulunan "RMS için Internet Information Services Desteği" konusuna bakın.

IIS'deki varsayılan Web sitesini kullanabilir veya yeni bir Web sitesi oluşturabilirsiniz. RMS'yi varsayılan Web sitesinden başka bir sitede sağlamak için, sağlama işlemini başlatmadan önce Web sitesini oluşturmalısınız. Varsayılan Web sitesini başka amaçlarla kullanıyorsanız, varsayılan Web sitesi için varsayılan yapılandırmanın korunabilmesi amacıyla RMS için yeni bir site oluşturmalısınız.

**Başlat** menüsünde **Windows RMS Yönetimi**'ni tıklattığınızda, **Genel Yönetim** sayfası görünür. Bu sayfada, Web sitesinde sağlama işlemine başlayabilirsiniz. İlk RMS sunucusunu sağlamak için, aşağıdaki bilgileri sağlamanız gerekir:

-   RMS yapılandırması, günlük ve dizin hizmetleri veritabanları için kullanılacak veritabanının adını belirtin.
    SQL Server örneğinizin yerel sunucu adıyla aynı olmayan bir adı varsa, her şey tek bir sunucuda yüklü olsa da, bunu uzak SQL Server örneği olarak ayarlamalısınız.
    Sağlama işlemi sırasında oturum açmış olan kullanıcı hesabının veritabanı sunucusunda veritabanı oluşturma izni olması gerekir.
-   RMS hizmet hesabı için kullanılacak hesabı belirtin. Yerel yapılandırma için, Local System ayrıcalıklarına sahip hizmeti çalıştırmayla ilgili yapısal güvenlik sorunları yüzünden önerilmemesine rağmen, Local System hesabını kullanabilirsiniz.
    Uzak SQL Server örneği veya birden fazla RMS sunucusu içeren bir yükleme için, etki alanı hesabını belirtmeniz gerekir. Kullandığınız etki alanı hesabı Active Directory arama ayrıcalıklarına sahip olmalıdır; bu hesap Yönetim konsolunun altında çalıştırılacağı IIS Uygulama Havuzu'nu oluşturmak için kullanılır. Varolan bir veritabanını yükseltmiyorsanız veya kullanmıyorsanız, RMS hizmet hesabı veritabanı oluşturma ayrıcalıkları gerektirir. Varolan veritabanlarını kullanıyorsanız, hesabın her RMS veritabanı için okuma ve yazma izinlerine gereksinimi vardır.
-   Bu Web sitesine erişmek için kullanılacak URL'yi belirtin. Varsayılan değer sağladığınız sitenin adıdır (varsayılan IIS yüklemesi olan bir sunucuyu sağlıyorsanız, bu değer Varsayılan Web sitesi'dir). Farklı bir Web sitesine erişmek için özel bir URL belirtebilirsiniz; örneğin, yük dengeleme URL'sini desteklemek veya hem intranet hem de Internet erişimini desteklemek için bunu yapabilirsiniz. Özel URL'nin çalıştığını doğrulamanız ve hem **Genel Yönetim** hem de **Hazırlama** sayfalarının sanal kökleri bulabilmesi için site adını DNS'ye eklemeniz gerekir. Bu URL Internet etkin dağıtım içinse, yeni URL'nin hem Internet'ten hem de kurumsal ağdan kullanılabildiğini doğrulayın.
-   Kayıt için kullanılan kök yükleme özel anahtarını korumak için kullanılacak yöntemi seçin. Varsayılan yöntem yazılım tabanlı şifreleme kullanmak ve şifrelenmiş özel anahtarı RMS yapılandırma veritabanında depolamaktır. Varsayılan yapılandırmayı kullanıyorsanız, veritabanındaki değeri şifrelemek için sağlam bir parola sağlamalısınız.
    Ancak, bilgisayarda yüklü ve yapılandırılmış bir donanım güvenlik modülü (HSM) varsa, donanım güvenlik modülüyle kullanmak ve özel anahtarları akıllı kart gibi bir donanımda depolamak üzere şifreleme hizmeti sağlayıcısı da (CSP) seçebilirsiniz. RMS, tam RSA sağlayıcısı gerektirir ve yalnızca bu sağlayıcılar CSP'ler listesinde yer alır. RMS özel anahtarını korumak için HSM kullanılması özellikle önerilir.
    RMS özel anahtarını parolayla korumak için yazılım tabanlı CSP seçeneğini kullanırsanız, bu parolayı ileride kullanmak üzere güvenli bir arşivde koruyun. Yapılandırma veritabanının yedek kopyasını da parolayla depolamalısınız. Bunu yaptığınızda, SQL veritabanı zarar görürse RMS'yi geri yükleyebilirsiniz. Herhangi bir nedenle parolayı değiştirirseniz, ilgili parolayla korunan özel anahtarı depolayan yapılandırma veritabanının yeni bir yedek kopyasını oluşturun ve sonra her ikisini de güvenli arşive yerleştirin. Yapılandırma veritabanının nasıl yedekleneceği ve geri yükleneceği hakkında daha fazla bilgi için, bu belge grubundaki “RMS Dağıtımı Planlama” bölümünde bulunan “RMS için Sistemi Yedekleme ve Geri Yükleme” konusuna bakın.
-   Sunucu lisans sertifikasında kullanılacak adı belirtin. Varsayılan olarak, bu, sunucunun adıdır.
-   Gerekirse, Internet'e erişmek için kullanılacak proxy sunucuyu (adresi ve bağlantı noktasıyla birlikte) belirtin.
-   Diğer RMS yöneticileri bir lisans sunucusuyla alt kayıt yaptırmaya çalıştığında sorun oluşursa, yöneticiyle iletişim kurmak için kullanabilecekleri bir e-posta adresi belirtin. Kök yüklemesini sağladıktan sonra, adresi değiştirebilirsiniz.
-   Kök yüklemenin sunucu lisans sertifikasını Microsoft Kayıt Hizmeti dışında kimin iptal edebileceğini denetlemek için sunucu lisans sertifikası iptal yöntemini seçin. Üçüncü taraf iptalini kullanmak için ilgili üçüncü parti varlığına ilişkin ortak anahtarı içeren dosyanın yolunu ve adını belirtmelisiniz.

Çevrimiçi kayıt seçeneğini belirlediyseniz, **Hazırla** sayfasında **Gönder**'i tıklattığınızda (uygun tüm seçenekleri yapılandırdıktan sonra), RMS bir anahtar çifti oluşturur ve ortak anahtarı Microsoft Kayıt Hizmeti'ne gönderir. (Hata iletileri alırsanız, hataların görüntülendiği sayfayı kapatmayın. Hataları giderdikten sonra, IIS'yi durdurup yeniden başlatmak için bir komut istemi penceresi açın ve `IISReset` yazın, önceki ekrana dönün, hazırlama ekranındaki bilgileri yeniden yazın ve sonra **Gönder**'i yeniden tıklatın.) Microsoft Kayıt Hizmeti sunucu lisans sertifikası oluşturur ve onu birkaç dakika içinde yapılandırma veritabanına döndürür. RMS'nin yüklendiği etki alanındaki ilk sunucu olduğundan, bu adım kök sertifika sunucusunu kaydettirme işlemini içerir.

Çevrimdışı kayıt seçeneğini belirlediyseniz, sağlama işlemi tamamlandıktan sonra sunucuyu Microsoft Kayıt Hizmeti'ne el ile kaydettirirsiniz. Sunucunun kullanılabilmesi için kayıt işleminin tamamlanması gerekir. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Kök Sertifika Sunucusunu El İle Kaydettirmek İçin" konusuna bakın.

Sunucu sağlama ve kayıt işlemi tamamlandıktan sonra, **Genel Yönetim** sayfasındaki bağlantılar değişir. **RMS'yi bu sitede hazırla** bağlantısı **RMS'yi bu sitede yönet** bağlantısına dönüşür, **Bu sunucuyu bir kümeye ekle** bağlantısının yerini **RMS hizmet hesabını değiştir** bağlantısı alır ve sayfaya **RMS'yi bu Web sitesinden kaldır** bağlantısı eklenir.

Bu başlangıç sunucusu RMS'nin kök yüklemesini oluşturur. Kök yüklemesi tek bir sunucudan veya kümeden oluşabilir. Başlatma sunucusunu yüklemeyi ve sağlamayı bitirdiğinizde, sertifika ve lisans hizmetleri için artıklık ve yük dengeleme desteği sağlamak üzere ek sunucular kurabilirsiniz.

Yapılandırmanız tamamlandıktan sonra, RMS etkin istemcilerin hizmeti bulabilmesi için kök sertifika kümenizin hizmet bağlantı noktasını Active Directory'ye kaydettirmeniz gerekir. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Hizmet Bağlantı Noktasını Kaydettirme" konusuna bakın. Hizmet bağlantı noktası kaydettirilmemişse, RMS istemciniz RMS ile birlikte kullanılamaz.

| ![](images/Cc747756.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diğer sunucularda RMS yüklemesini başlatmadan önce ilk sunucuda RMS yüklemesini ve sağlamasını tamamlamanız gerekir. RMS, üyelikleri birden çok ormana yayılan Active Directory grupları için içerik korumayı destekler. Kuruluşunuzda birden çok orman veya birden çok ormana yayılan gruplar yoksa, RMS yapılandırma veritabanındaki **MaxCrossForestCalls** küme ilkesini değiştirerek RMS sunucunuzdaki kullanım lisansı verme işleminin performansını en iyi duruma getirebilirsiniz. Bu ilke, bir grubun üyeliğinin aşabileceği orman sınırı sayısının en üst değerini belirtir. Varsayılan değer 10'dur. Bu değeri 0 olarak değiştirmek için, aşağıdaki SQL komutunu kullanın:`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'` |

Aşağıdaki konularda RMS Genel Yönetim sayfasında bulunan görevleri tamamlamak için gereken ayrıntılı adımlar sağlanmaktadır:

-   Başlangıç sunucusunu yüklemek amacıyla yükleme sihirbazının nasıl kullanılacağı hakkında bilgi için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “RMS Service Pack 1'i Yüklemek İçin” konusuna bakın.
-   Başlangıç sunucusunun nasıl sağlanacağı konusunda bilgi için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “İlk Kök Sertifika Sunucusunu Sağlamak İçin” konusuna bakın.
-   Küme oluşturmak amacıyla kök yüklemeye nasıl sunucu ekleneceği konusunda bilgi için, bu konuda daha sonra yer alan “[Sertifika ve Lisans Desteği için Sunucu Ekleme](https://technet.microsoft.com/089ceb62-2a96-444f-ab42-1d5deaabd0c3)” bölümüne bakın.
