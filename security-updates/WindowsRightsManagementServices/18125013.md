---
TOCTitle: RMS Sunucusunu Çalıştırma
Title: RMS Sunucusunu Çalıştırma
ms:assetid: '1533426b-89c2-43e0-8068-ca97ddab8606'
ms:contentKeyID: 18125013
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720205(v=WS.10)'
---

RMS Sunucusunu Çalıştırma
=========================

RMS sunucusunu çalıştırma, RMS'nin kuruluşa dağıtılma işleminden sonraki yönetim görevlerini belirtir. Bu bölümde, RMS sunucusunu yönetmenize yardımcı olacak bilgiler, genel yönetim görevi yordamları ve ek bilgi kaynakları ile birlikte en iyi uygulama yöntemlerine yönelik bilgiler sağlanır.

Bu konuda

-   [RMS'yi Yönetme](https://technet.microsoft.com/9b573c55-c14c-436c-b3c5-7ba445de1562)
-   [RMS - Nasıl yapılır?](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)
-   [RMS Kaynakları](https://technet.microsoft.com/d91221cf-e38e-4add-b7b9-50e63aad9a28)

Bu Kılavuzda Kullanılan Terminoloji
-----------------------------------

**hesap sertifikası**  
Kullanıcı hesaplarını, hak hesabı sertifikasında veya RAC'deki anahtar çiftleriyle ilişkilendiren işlem.

<!-- -->

**hesap sertifikası hizmeti**  
Hak hesap sertifikalarını oluşturan ve dağıtan bir RMS Web hizmeti. Ayrıca bkz: hesap sertifikası.

<!-- -->

**etkinleştirme proxy hizmeti**  
RMS 1.0 sürümü istemcilerinin makine etkinleştirmesini destekleyen bir RMS Web hizmeti. Makine etkinleştirme isteklerini Microsoft Etkinleştirme Hizmeti'ne iletmek için kullanılır. Etkinleştirme hizmeti, istemci bilgisayar için benzersiz bir kasa ve eşleşen RMS makine sertifikası üretir ve RMS sunucusundaki etkinleştirme proxy hizmeti istek gönderen istemci bilgisayara tekrar iletilir. Ayrıca bkz: kasa.

<!-- -->

**yönetim hizmeti**  
Yönetim Web sitesine ev sahipliği yapan, RMS yönetimine olanak sağlayan ve kümeye ilişkin yapılandırma veritabanını güncelleştiren bir RMS Web hizmeti.

<!-- -->

**uygulama bildirimi**  
İlişkili RMS etkinleştirilmiş uygulamanın modüllerini ve uygulama ortamında nelerin çalışabileceğini açıklayan bir XML belgesi. RMS korumalı içerik oluşturmak veya RMS korumalı içeriği kullanmak için RMS istemci API'lerine yazan herhangi bir uygulamanın çalıştırma zamanında bildirim sağlaması gerekir.

<!-- -->

**özellik**  
Active Directory'de bir nesnenin özelliği. Her nesne sınıfı için, şema sınıfın bir örneğinin hangi özelliklere sahip olması gerektiğini ve hangi ek özelliklere sahip olabileceğini tanımlar.

<!-- -->

**bağlama**  
RMS istemcisinin kullanım lisansı koşullarını istenen haklarla karşılaştırarak doğruladığı RMS sisteminde yer alan ve hakları uygulayan mekanizma. Söz konusu koşullar sağlanırsa, haklar verilir.

<!-- -->

**sertifika**  
Sıklıkla kimlik doğrulamak ve açık ağlarda bilginin güvenliğini sağlamak için kullanılan dijital bir belge. Ortak anahtarı, ilişkili özel anahtarı bulunduran varlıkla güvenli olarak bağlayan bir sertifika. Sertifikalar, yayıncı sertifika yetkilisi (CA) tarafından dijital olarak imzalanır ve bir kullanıcı, bilgisayar veya hizmet için yayınlanabilir. Ayrıca bkz: özel anahtar, ortak anahtar.

<!-- -->

**istemci kaydı**  
Kullanıcı bilgisayarının veya aygıtının, lisans sunucusu tarafından tanınacak yayımlama lisansları oluşturmasına olanak sağlayan, istemci lisans sertifikası oluşturma işlemi.

<!-- -->

**istemci lisans sertifikası**  
RMS sunucusu tarafından oluşturulan ve RMS istemci bilgisayarlara konan sertifika. Bu sertifika, kullanıcıların RMS etkinleştirilmiş ağa bağlanmadan korumalı içeriği çevrimdışı olarak yayımlamasına olanak sağlar. İstemci lisans sertifikası RMS istemcinin yayımlama lisanslarını dijital olarak imzalamak için kullanacağı anahtarı içerir.

<!-- -->

**koşul**  
Yayımlama lisansında bir araya getirilen haklar grubunun bir parçası olan belirli kısıtlama ve parametreler kümesi. Bunlar kullanım sırasında uygulanır. Zaman koşulu, bir kullanıcının RMS korumalı içerik için süre sonu belirlemesine olanak veren ve sık kullanılan bir koşuldur.

<!-- -->

**yapılandırma veritabanı**  
Bir sunucu veya kümenin RMS yapılandırma bilgilerini içeren veritabanı.

<!-- -->

**içeriği kullanma**  
Korumalı içeriğin bir parçası için kullanım haklarının şifresini çözme ve uygulama.

<!-- -->

**içerik anahtarı**  
Yayımlama ve kullanma sırasında korumalı içeriğin hem şifrelenmesinde hem de şifresinin çözülmesinde kullanılan anahtar. Simetrik anahtar olarak da bilinir. RMS 128 bit AES içerik anahtarı kullanır.

<!-- -->

**içerik sahibi**  
Korumalı içerik için erişim ilkelerini saptayan kişi veya kuruluş.

<!-- -->

**şifre çözme**  
Şifreli metni düz metne dönüştürerek şifreli verileri tekrar okunabilir şekle getirme işlemi.

<!-- -->

**dijital imza**  
Bir iletinin, dosyanın veya dijital olarak kodlanmış bilginin sahiplerinin kimliklerini bilgiye bağlamasına izin veren yöntem. Bilgiyi dijital olarak imzalama işlemi, bilginin üzerinde değişiklik yapılmasını ve imza olarak adlandırılan bir etikete dönüşen, gönderenin elindeki bazı gizli bilgileri içerir. Dijital imzalar, ortak anahtar ortamlarında kullanılır, izin vermeme ve bütünlük hizmetleri sunar.

<!-- -->

**DRMRemote hizmeti**  
Farklı RMS sunucuları arasındaki iletişimde kullanılan .NET Uzaktan Yönetim üzerinden hizmet sunan Windows RMS Web hizmeti.

<!-- -->

**şifreleme**  
Bilgiyi, sadece belirli bir alıcının okuyabileceği bir şekle döndürme işlemi. Şifreleme, bilgiyi güvenli olarak saklamak için etkili bir yoldur. Şifrelenmiş bir dosyanın şifresini çözmek için, alıcının bu dosyayı tercüme edecek olan gizli anahtar veya parolaya sahip olması gerekir. Ayrıca bkz: ortak anahtar şifrelemesi.

<!-- -->

**kayıt**  
Kök sertifika sunucusunun, Microsoft kayıt hizmeti tarafından imzalanmış bir sunucu lisans sertifikası aldığı işlem.

<!-- -->

**kayıt isteği**  
Sunucu lisans sertifikası için, RMS kök sertifika sunucusu tarafından Microsoft Kayıt Hizmeti'ne gönderilen istek.

<!-- -->

**dışlama**  
Bir istemcinin kullanım lisansı isteğini dışlama ilkesine dayanarak reddetmek için RMS sunucusu tarafından kullanılan süreç. Ayrıca bkz: dışlama listesi.

<!-- -->

**dışlama listesi**  
RMS lisans hizmeti tarafından lisansların reddedileceği sorumluların listesi.

<!-- -->

**dışlama ilkesi**  
RMS yapılandırma veritabanında yer alan ve kuruluşta dışlamanın uygulanma yöntemini denetleyen ayarlar.

<!-- -->

**Genişletilebilir Haklar İşaretleme Dili (XrML)**  
RMS tarafından, desteklediği tüm lisanslar için kullanılan XML tabanlı biçim; bu lisanslar şunlardır: korumalı içeriğe uygulanan RMS ilkesini belirten belgeler olan makine sertifikaları, RAC'ler, CLC'ler, kullanım lisansları, yayımlama lisansları ve sunucu lisans sertifikalarıdır.

<!-- -->

**sertifika verme lisansı**  
Korumalı içeriğe uygulanan RMS ilkesini belirten veriler.

<!-- -->

**lisans kümesi**  
Kök sertifika kümesi dışında RMS lisans ve yayımlama hizmetlerini kullanan bir veya daha fazla sunucu. Bu sunucular ortak bir veritabanı ve bağlantı URL'si kullanır ve birden fazla sunucu kullanılıyorsa, bu sunucuların yük dengeleyici bir yazılım veya donanım ile kullanılarak dağıtılması gerekir. Sertifika veya kök kümesinin tersine, lisans kümesindeki RMS sunucuları kullanıcılara sertifika veremez.

<!-- -->

**lisans sunucusu**  
Kök sertifika kümesi dışında RMS lisans ve yayımlama hizmetlerini çalıştıran sunucu.

<!-- -->

**lisans hizmeti**  
Kullanım lisansları veren bir RMS Web hizmeti.

<!-- -->

**kasa**  
Korumalı içeriğin kullanımının geçerli olması için kimlik doğrulaması yapmaktan, bilgileri şifrelemekten ve bilgilerin şifresini çözmekten, güvenilen yazılım işlemini değiştirilmeye ve incelenmeye karşı korumaktan sorumlu yazılım modülü. Güvenlik havuzu olarak da bilinir.

<!-- -->

**günlük hizmeti**  
Günlüğe kaydedilen verileri ileti sırasından, RMS sunucusu veya kümesinin günlük veritabanına aktaran bir RMS dinleyici hizmeti.

<!-- -->

**makine etkinleştirme**  
RMS 1.0 sürümüne sahip bir bilgisayar için benzersiz kasa ve makine sertifikası edinme süreci. RMS 1.0 SP1'deki makine etkinleştirme, söz konusu makinedeki her kullanıcı için bir makine sertifikası edinme sürecidir.

<!-- -->

**bildirim**  
Uygulamanın işlem alanına yüklenebilen, yüklenemeyen ve kimi durumlarda yüklenebilen kitaplık veya programların tanıtıldığı imzalı XML belgesi.

<!-- -->

**Microsoft Etkinleştirme Hizmeti**  
RMS 1.0 sürümü istemcilerin isteklerine yanıt olarak RMS makine sertifikaları ile kasalar veren ve Microsoft tarafından barındırılan bir Web hizmeti.

<!-- -->

**Microsoft Kayıt Hizmeti**  
RMS dağıtımında kök sertifika sunucusuna sunucu lisans sahibi sertifikası veren ve Microsoft tarafından barındırılan Web hizmeti.

<!-- -->

**ön sertifika**  
RMS sertifika hizmetinin, bir uygulamanın RMS sunucusundan kullanıcı adına hak hesabı sertifikası istemesine olanak sağlayan özelliği. Ön sertifika kullanılarak alınan hak hesabı sertifikaları yalnızca kullanıcının ortak anahtarını içerir.

<!-- -->

**sorumlu**  
RMS güvenlik şemasında yerleşik bir role sahip olan ve nesnelerin güvenli hale getirilebildiği bir varlık (örneğin, kullanıcı, grup veya korumalı içerik yöneticisi).

<!-- -->

**özel anahtar**  
Ortak anahtar algoritmasıyla kullanılan şifreli anahtar çiftinin gizli yarısı. Özel anahtarlar genellikle simetrik oturum anahtarının şifresini çözmek, verileri dijital olarak imzalamak veya ilişkili özel anahtarla şifrelenmiş verilerin şifresini çözmek için kullanılır. Ayrıca bkz: ortak anahtar, ortak anahtar şifrelemesi.

<!-- -->

**sağlama**  
RMS sunucusunu bir kuruluşta çalışacak şekilde yapılandırmak için.

<!-- -->

**ortak anahtar**  
Ortak anahtar algoritmasıyla kullanılan şifreli anahtar çiftinin gizli olmayan yarısı. Ortak anahtarlar genellikle bir oturum anahtarı şifrelerken, bir dijital imza doğrularken veya ilişkili özel anahtarla şifresi çözülebilen verileri şifrelerken kullanılır. Ayrıca bkz: özel anahtar, ortak anahtar şifrelemesi.

<!-- -->

**ortak anahtar şifrelemesi**  
Matematiksel açıdan ilişkili iki şifreleme anahtarı kullanan bir şifreleme yöntemi. Bir anahtar özel anahtar olarak adlandırılırken ve gizli olarak saklanır. Diğeri ortak anahtar olarak adlandırılır ve tüm potansiyel alıcılara serbestçe verilir. Tipik bir senaryoda, gönderen, bir iletiyi şifrelemek için alıcının ortak anahtarını kullanır. Sadece alıcı iletinin şifresini çözmek için kullanılacak ilgili özel anahtara sahiptir. Ortak anahtar ve özel anahtar arasındaki ilişkinin karmaşıklığı, sağlanan anahtarların yeterince uzun olması durumunda birine bakarak diğerini tahmin etmenin bilgi işlem bakımından imkansız olması anlamına gelir. Asimetrik şifreleme olarak da adlandırılır. Ayrıca bkz: özel anahtar, ortak anahtar.

<!-- -->

**yayımlama lisansı**  
RMS korumalı içeriği yayımlarken oluşturulan lisans. Diğer öğelerin yanı sıra içeriğe kimin erişebileceğini, hangi hakların verileceğini ve hangi koşullarda erişilebileceğini belirtir. Sertifika verme lisansı olarak da adlandırılır.

<!-- -->

**yayımlama hizmeti**  
Yayımlama lisanslarını imzalayan ve istemci lisans sahibi sertifikalarını veren bir RMS hizmeti. Ayrıca bkz: istemci lisans sertifikası; yayımlama lisansı.

<!-- -->

**RAC**  
Hak hesabı sertifikası tanımına bakın.

<!-- -->

**iptal**  
Geçersiz lisanslara sahip varlıkları listeleyen işlem.

<!-- -->

**iptal listesi**  
Sertifikayı verenin iptal ettiği sertifika ve lisansların listelendiği XrML tabanlı belge. Ayrıca bkz: iptal.

<!-- -->

**hak**  
RMS teknolojisiyle korunan içerik üzerinde belirli kişilerin gerçekleştirmesine izin verilen bir eylem. Bu haklar, koşullar kullanılarak daha da kısıtlanabilir.

<!-- -->

**hak hesabı sertifikası (RAC)**  
Bir kullanıcının hesabını ve anahtarını belirli bir bilgisayara veya bilgisayar gruplarına bağlayan, RMS etkinleştirmesindeki makine sertifikasını kullanan sertifika. Sertifikanın bileşenleri, kullanıcıların korumalı içeriği kullanmalarını sağlamak üzere kullanılır. RMS SDK'de grup kimlik sertifikası (GIC) olarak da adlandırılır.

<!-- -->

**hak yönetimi (RM)**  
Şifreleme, sertifika ve kimlik doğrulama kullanılarak dijital verilerin kalıcı biçimde korunmasını sağlayan teknoloji. Yetkili alıcıların veya kullanıcıların, korumalı içeriği içerik sahibi tarafından belirlenen haklara veya iş kurallarına göre kullanabilmeleri için lisans almaları gerekir.

<!-- -->

**Rights Management Services istemcisi**  
RMS sistemindeki tüm istemci bilgisayarların yüklemesi gereken RMS API'leri grubu. Bu, makine etkinleştirmesi için bir önkoşuldur ve RMS etkinleştirilmiş uygulamaları kullanmak için gereklidir.

<!-- -->

**hak ilkesi şablonu**  
RMS korumalı içeriğe uygulanabilen standart kullanıcı kümesini, hakları ve koşulları tanımlar. Kullanıcı içeriğin bir bölümüne hak ilkesi şablonu uyguladığında, şablonun tanımladığı hak ve koşullar, yayımlama lisansının bir parçası haline gelir.

<!-- -->

**RMS etkinleştirme**  
RMS 1.0 sürümünde son kullanıcın bilgisayarına kasa yerleştirme süreci. Bu, yalnızca RMS etkinleştirme hizmeti tarafından sağlanabilir ve RMS teknolojisini kullanmak için kesinlikle gereklidir. RMS SP1 1.0'da, bu, bir makineyi kullanan kullanıcı için söz konusu makinenin sertifikası edinme işlemidir ve RMS etkinleştirme hizmetine bağlanılmasını gerektirmez. Etkinleştirme olarak da adlandırılır.

<!-- -->

**RMS Sertifika Hizmeti**  
Microsoft .NET Passport kimlik bilgilerini temel alarak kullanıcılara hak hesabı sertifikaları veren, Microsoft tarafından barındırılan Web hizmeti.

<!-- -->

**RMS istemcisi**  
RMS sistemindeki tüm istemci bilgisayarların yüklemesi gereken RMS API'leri grubu. Bu, makine etkinleştirmesi için bir önkoşuldur ve RMS etkin uygulamaları kullanmak için gereklidir.

<!-- -->

**RMS makine sertifikası**  
RMS etkinleştirmesi sırasında son kullanıcının bilgisayarına yerleştirilen sertifika. Bu sertifikadaki ortak anahtar, kullanıcının hak hesabı sertifikasında bulunan özel anahtarını şifrelemek için kullanılır.

<!-- -->

**RMS etkin uygulama**  
Kullanıcılara oluşturdukları içeriğe iliştirilecek hakları belirtme olanağı sağlamak için Rights Management Services SDK'si kullanılarak uzatılmış bir uygulama.

<!-- -->

**RMS etkin bilgisayar**  
RMS tarafından korunan içeriği işleyebilmesi için RMS istemci bileşeninin yüklendiği ve RMS makine etkinleştirmesinin gerçekleştirildiği bilgisayar.

<!-- -->

**RMS korumalı içerik**  
RMS teknolojisiyle korunan dijital bilgiler.

<!-- -->

**kök sertifika kümesi**  
Bir RMS dağıtımında yönetim, kayıt, hesap sertifikası verme, etkinleştirme proxy, lisans ve yayımlama hizmetlerini kullanan bir veya daha fazla sunucu. Bu sunucular ortak bir veritabanı ve bağlantı URL'si kullanır ve bir yazılım ya da donanım yük dengeleyicisinin ardında dağıtılmalıdır. Her Active Directory ormanında tek bir kök sertifika kümesi bulunabilir.

<!-- -->

**kök sertifika sunucusu**  
Bir RMS dağıtımında yönetim, kayıt, hesap sertifikası verme, etkinleştirme proxy, lisans ve yayımlama hizmetlerini kullanan birincil sunucu. Her Active Directory ormanında tek bir kök sertifika sunucusu olabilir.

<!-- -->

**güven kökü**  
Diğer sertifikaların güveninin temelini oluşturan güvenilen varlık. Tüm sertifika sağlayıcılarının ve asıl kullanıcının köke güvenmesi gerekir.

<!-- -->

**güvenlik kimliği (SID)**  
Her Windows kullanıcı, grup ve bilgisayar hesabını tanımlayan Windows veri yapısı. İlk kez yaratıldıklarında, ağdaki her hesaba benzersiz bir SID verilir. Windows'taki iç işlemler, hesabın kullanıcı veya grup adı yerine hesap güvenlik kimliğine başvurur.

<!-- -->

**sunucu lisans sertifikası**  
RMS sunucusunun kimlik bilgilerini oluşturarak, onun geçerli bir sertifika ve lisans hizmeti olmasına ve çalışabilmesine olanak sağlayan sertifika. Lisans sertifikası, yayımlama lisanslarındaki içerik anahtarlarını şifrelemek için kullanılan ortak anahtarı içerir.

<!-- -->

**sunucu hizmeti**  
Başka bir hizmet tarafından kullanılması amaçlanan RMS Web hizmeti.

<!-- -->

**hizmet bağlantı noktası (SCP)**  
RMS dağıtımının kök sertifika kümesi URL'sine başvuruda bulunan bir Active Directory nesnesi. RMS istemcisi RMS hizmetlerini bulmak için bu bilgiyi kullanır.

<!-- -->

**alt kayıt**  
Lisans sunucusu hazırlık işleminin, sunucunun kök sertifika kümesinden sunucu lisans sertifikasını aldığı bölümü.

<!-- -->

**alt kayıt isteği**  
Sunucu lisans sertifikası için, kök sertifika kümesine lisans sunucusu tarafından gönderilen istek.

<!-- -->

**alt kayıt hizmeti**  
Hazırlık sırasında lisans sunucuları tarafından verilen sunucu lisans sertifikalarına ilişkin istekleri yanıtlayan kök sertifika sunucusundaki bir RMS Web hizmeti.

<!-- -->

**Super Users**  
Super Users grubunun bir üyesi.

<!-- -->

**Super Users grubu**  
RMS sunucusu tarafından yayımlanan içerik açılırken bu sunucunun sahip lisansları vereceği her RMS kümesi için yönetim açısından tanımlanan isteğe bağlı kullanıcı grubu.

<!-- -->

**kullanım lisansı**  
Bir son kullanıcının korumalı içeriği ne şekilde kullanabileceğini belirten hakları ve koşulları listeleyen lisans. Son kullanıcı lisansı (EUL) olarak da bilinir.
