---
TOCTitle: Sistem Kurtarma Hazırlığı
Title: Sistem Kurtarma Hazırlığı
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18125173
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747659(v=WS.10)'
---

Sistem Kurtarma Hazırlığı
=========================

RMS sunucusu tarafından kullanılan Internet ve intranet bağlantılarını, RMS sertifika sunucusunu, alt kayıtlı bir RMS lisans sunucusunu veya RMS yapılandırma veritabanlarını barındıran veritabanı sunucuları da dahil RMS sistemindeki bileşenlerden birindeki hata, hizmetin beklenmedik biçimde yitirilmesine neden olabilir. RMS sistemi kurarken, RMS hizmetinde olabilecek bir kaybın BT sistemlerinize ve önemli verilerinize olası etkisini göz önünde bulundurmak ve bileşeni olabildiğince etkin bir şekilde kurtarmak üzere hazırlık yapmak önemlidir.

RMS yapılandırma veritabanlarını barındıran veritabanı sunucularındaki hata, RMS korumalı bilgilere erişilmesini engelleyebilecek bir bileşende olabilir. Bu bölümde, RMS sistemi için sistem koruma hazırlığı yaparken, aşağıdakilerle ilgili dikkat edilmesi gereken konular ve unsurlar açıklanır:

-   [Internet Bağlantısı](#bkmk_1)
-   [Intranet Bağlantısı](#bkmk_2)
-   [Sertifika ve Lisans Hizmetleri](#bkmk_3)
-   [Veritabanı Sunucuları](#bkmk_4)
-   [Active Directory](#bkmk_5)

<span id="BKMK_1"></span>
Internet Bağlantısı
-------------------

Çevrimiçi sunucu kaydı kullanıyorsanız, RMS sunucusu, sunucu lisans sertifikası (SLC) almak ve bunu her yıl yenilemek için sağlama işlemi sırasında Internet bağlantısı gerektirir. Bir yıllık kullanımın sonuna gelindiğinde, sertifika sunucusu, olayları Sistem Olay Günlüğüne kaydederek sertifikanızı yenilemenizi bildirir. Olaylar, SLC süre sonundan bir ay önce (Olay Kimliği 16), SLC süre sonundan bir hafta önce (Olay Kimliği 17) ve SLC süresi dolduğunda (Olay Kimliği 18) günlüğe kaydedilir. RMS Yönetimi Web sitesinin RMS Genel Yönetimi Web sayfası da, SLC süre sonunun yaklaştığı konusunda uyarıda bulunur. Microsoft Operations Manager (MOM) için RMS Yönetim Paketi kullanıyorsanız, süre sonu olayları bir uyarı tetikler. RMS sunucusunda Internet bağlantısı kullanılamıyorsa, sunucu lisans sertifikası RMS Yönetimi Web sitesindeki **Yenile** düğmesi kullanılarak yenilenemez; güncelleştirilmiş bir sertifika istemek için çevrimdışı kayıt işlemi kullanılmalıdır.

En iyi yöntem olarak, sertifika süresi dolduğunda Internet bağlantısının kullanılamaması durumunda oluşacak karmaşaları engellemek için SLC'yi süre sonu tarihinden daha önce yenileyin. RMS sunucusu, geçerli bir SLC olmadan RMS hizmetlerini sağlayamaz; bu durumda kullanıcılar RMS korumalı bilgiler yayımlayamaz veya RMS korumalı bilgileri okumak için gereken kullanım lisanslarını ve hak hesabı sertifikalarını (RAC) alamaz. RMS korumalı içeriğin bir bölümü için önceden kullanım lisansı ve RAC almış olan kullanıcılar, bu kullanım lisanslarının veya RAC'lerinin süresi dolana kadar bilgilere erişmeye devam eder.

<span id="BKMK_2"></span>
Intranet Bağlantısı
-------------------

RMS, bağlantılı bir altyapıya dayanan istemci-sunucu teknolojisidir. RMS sunucuları, çalışan bir intranet ağı olmadan, kuruluştaki gerekli hizmetlere veya hizmetleri sağlamak üzere kullanıcılara bağlanamaz. Kullanıcılar, intranet bağlantısı olmadan, RMS sunucularından hak hesabı sertifikalarını (RAC), istemci lisans sertifikalarını (CLC) ve kullanım lisanslarını alamaz.

En iyi yöntem olarak, kuruluşlar, uzak sitelerden RMS sunucu sitelerine yedek yönlendirme mimarileri ve yerine çalışma bağlantıları düşünmelidir.

Kullanıcı, bilgisayarı için CLC aldıktan sonra, RMS korumalı bilgileri RMS sunucusuna bağlantısı yokken çevrimdışı olarak yayımlayabilir. Bazı RMS etkin e-posta uygulamaları, kullanıcıların, RMS korumalı e-posta iletilerini intranet bağlantısı olmasa da okuyabilmelerini sağlamak için, posta kutusu eşitlenirken ilişkili RMS korumalı e-posta iletilerine yönelik kullanım lisanslarını otomatik olarak karşıdan yükleyecek şekilde yapılandırılmıştır.

<span id="BKMK_3"></span>
Sertifika ve Lisans Hizmetleri
------------------------------

RMS sistemi, yoğunluklu olarak Internet Information Services (IIS) 6.0'daki iki sanal dizine dayanır; sertifika ve lisans hizmetleri. Bu hizmetler kullanıcıların ve bilgisayarlarının RMS ortamına kaydettirilmesine ve RMS etkin uygulamaların RMS korumalı bilgiler yayımlamasına ve bu bilgilere erişmesine olanak verir. Bu hizmetler kullanılamaz olursa, geri yükleninceye kadar kullanıcılar reddedilebilir.

Hizmetin kullanılamaması durumuna hazırlıklı olmak için, sertifika sunucusu ve alt kayıtlı lisans sunucusu oluşturmayı düşünerek kümedeki herhangi bir düğümde oluşan hatanın hizmetin kullanılabilirliğini etkilememesini sağlayın.

İyi bir uygulama yöntemi olarak, herhangi bir düğümdeki hatanın tüm performansı etkilemesini engellemek için kümelerde ek kapasite oluşturun. Kümeye ilk sertifika sunucusunu ve her alt kayıtlı lisans sunucusunu veya ilk alt kayıtlı lisans sunucusunu yüklerken, sağlama işlemi sırasında girilen yapılandırma seçeneklerini ve verileri dikkatle kaydedin.

<span id="BKMK_4"></span>
Veritabanı Sunucuları
---------------------

RMS sistemindeki en önemli bileşenler, yapılandırma veritabanlarını tutan veritabanı sunucularıdır. Her RMS sunucusu veya sunucu kümesi, yapılandırma ve günlük bilgilerini depolamak için veritabanlarını kullanır. Yapılandırma bilgileri RMS'nin çalışması için gereklidir. Bu veritabanları sunucu lisans sertifikasını, üretilen RMS ilke şablonlarını ve RMS sistemine kaydettirilen kullanıcıların listesini tutar; RMS sunucusuyla birlikte bir donanım güvenlik modülü kullanılmıyorsa, RMS sunucusunun özel ve ortak anahtarlarını da içerir. RMS veritabanlarının yedekleriyle, önceki bir RMS yüklemesini yeni bir sunucuya geri yükleyebilir veya RMS sistemini yeniden oluşturabilirsiniz. Veritabanı kaybının oluşturduğu etki, veritabanına bağlı olarak değişir. Aşağıdaki listede belirli veritabanı hatalarının etkileri açıklanmaktadır:

-   **Yapılandırma veritabanı**. RMS sunucusu işlemi sırasında bu veritabanı kullanılamaz olursa, RMS gerekli bilgileri önbelleğe aldığından RMS hizmetleri çalışmaya devam edebilir. Ancak, RMS hizmetinin yapılandırma veritabanıyla etkileşimde bulunmasını gerektiren, yeni kullanıcı kaydı gibi bir olay oluşursa, RMS hizmeti hatayla karşılaşır ve yeni kullanıcı RMS korumalı içerikle çalışamaz. IIS hizmetini yeniden başlatma veya zamanlanmış yerel önbellek yenileme işlemi gibi, RMS sunucusunun önbelleğe alınan bilgileri atmasına neden olan bir işlem gerçekleşirse RMS hizmeti çalışmaz. RMS sunucusu, yapılandırma veritabanı kullanılabilir duruma gelinceye kadar normal hizmetine geri dönemez.
    Yapılandırma veritabanı bozulursa veya kalıcı olarak kullanılamaz olursa, RMS sunucuları çalışmaz.
-   **Dizin hizmetleri veritabanı**. Genel katalog sunucusundan alınan grup adları ve bunlara ilişkin üyelik ayrıntıları hakkında önbelleğe alınan bilgileri tutar. Bu tablo kısa süreli olarak kullanılamaz olduğunda, RMS hizmetlerinde fark edilebilir bir azalma gözlenmez. Asıl amacı, genel katalog sunucusu için artıklık sağlamak ve hizmet yükünü azaltmaktır.
-   **Günlük veritabanı**. RMS sunucusunda günlük işlemi etkinleştirilirse, bu günlüğün depolanacağı veritabanıdır. Veritabanı kullanılamıyorsa, günlük girişleri RMS sunucusundaki Message Queuing (MSMQ olarak da bilinir) hizmetinde oluşturulur ve başka türlü yapılandırılmadıysa tüm kullanılabilen disk alanını kullanır.

En iyi yöntem olarak, veritabanı sunucularını, etkin beklemede, yerine çalışma koruması sağlamak üzere kümelendirin. Ayrıca, RMS sertifika sunucuları ve kümelerine ve lisans sunucuları ve kümelerine yönelik veritabanlarını düzenli olarak yedekleyin.

Başka bir uygulama yöntemi olarak, hazır bir yedek veritabanı sağlamak üzere işlem günlüğünü göndermeyi kullanın. Bu uygulama ek donanım gerektirebilir, ancak kuruluşların veritabanlarını çok hızlı bir şekilde kurtarmasını sağlar. Microsoft BT, RMS yapılandırma veritabanı kurtarması için bu yöntemi uyguladı. Bunu yapmak için RMS sağlama işlemi sırasında sanal SQL adını seçin. Sanal SQL adı, Etki Alanı Ad Sistemi'ni (DNS) kullanarak gerçek SQL adına eşleme yapmanızı sağlar. Özgün SQL Server'ın çalışmasını durdurduğu durumda, DNS adı eşlemesini özgün sunucudan yedek sunucuya değiştirerek yedek SQL Server'a kolayca geçebilirsiniz. Bu çözümün Microsoft'taki iç uygulaması hakkında daha fazla bilgi için, [Microsoft Web sitesindeki](http://go.microsoft.com/fwlink/?linkid=42070) (http://go.microsoft.com/fwlink/?LinkId=42070) Microsoft Corporation örnek çalışmasına bakın.

<span id="BKMK_5"></span>
Active Directory
----------------

RMS, iki önemli hizmette Active Directory'ye dayanır: kullanıcı kimlik doğrulaması ve genel katalog hizmeti. Active Directory'nin kullanılamadığı durumda, kullanıcı kimlik doğrulaması yapılamaz ve kullanıcılar ve bilgisayarları RMS sistemine kaydettirilemez. RAC almak için sertifika ardışık düzeni gerekir; bu ardışık düzen ise kimlik doğrulaması gerektirir. Kullanıcının RAC'si varsa, lisans ardışık düzeni varsayılan olarak anonim olduğundan, daha fazla kimlik doğrulaması gerekmeden kullanım lisansı alabilir.

Kuruluş varlıkları, RMS korumalı bilgilere erişimi olan kişileri belirtmek için Active Directory'de grup üyelikleri kullanabileceğinden, Active Directory'nin kullanılamaz olması kullanıcıların kullanım lisansı almalarını engeller. Grup üyeliği bilgileri RMS sunucusunda varsayılan olarak 15 dakika önbellekte tutulduğundan, genel katalog hizmetinin geçici olarak kullanılamaması durumu sorun oluşturmaz. Önbellek güncelleştirmeleri arasındaki süreyi artırmak veya azaltmak isterseniz, geçerlilik süresini denetleyen kayıt defteri anahtarını değiştirin. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Active Directory Önbellek Ayarlarını Değiştirme" konusuna bakın.
