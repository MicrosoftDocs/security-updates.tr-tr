---
TOCTitle: RMS Hesap Sertifikası
Title: RMS Hesap Sertifikası
ms:assetid: 'c9a385c5-6dbb-47f5-a80f-69718e6f9deb'
ms:contentKeyID: 18125262
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747750(v=WS.10)'
---

RMS Hesap Sertifikası
=====================

Hesap sertifikası işlemi kullanıcı hesabını belirli bir bilgisayarla ilişkilendiren ve kullanıcının bu bilgisayarda RMS korumalı içerik kullanmasına olanak tanıyan bir hak hesabı sertifikası oluşturur. Kullanıcı bir istemci bilgisayardan RMS korumalı içerik yayımlamayı veya RMS korumalı içeriği kullanmayı ilk kez denediğinde, RMS etkin uygulama RMS hesap sertifikası hizmetine bir hak hesabı sertifikası isteği gönderir.

Sertifika hizmeti, Windows kimlik doğrulaması veya akıllı kart gibi bir donanım şifreleme aygıtında depolanan bir x.509 sertifikası kullanarak kullanıcının kimliğini doğrulayabilir. Kullanıcı kimliği doğrulandıktan sonra, RMS sunucusu kullanıcının doğrulanmış kimlik bilgilerini temel alarak bir hak hesabı sertifikası oluşturur. İstemci bilgisayarın RMS makine sertifikasının ortak anahtarını kullanarak kullanıcının özel anahtarını şifreler ve şifrelenmiş anahtarı hak hesabı sertifikasına ekler. Daha sonra istekte bulunan uygulamaya hak hesabı sertifikasını verir ve uygulama sonraki yayımlama ve kullanım lisansı isteklerinde kullanılabilmesi için bu hak hesabı sertifikasını bilgisayarda veya aygıtta depolar. Hak hesabı sertifikası da yapılandırma veritabanında depolanır.

Hak hesabı sertifikası isteğinde bulunabilmek için istemci bilgisayarın RMS makine sertifikası gerekli olduğundan, hesap sertifikası işlemi makine etkinleştirme işleminin ardından gerçekleştirilir.

Kullanıcıların, kullandıkları her bilgisayar için hak hesabı sertifikası alması gerekir. Kullanıcı birden fazla bilgisayarda çalışıyorsa her bilgisayar için benzersiz bir hak hesabı sertifikası verilir, ancak tüm bilgisayarlarda bu kullanıcı için aynı anahtar çifti bulunur.

RMS etkin uygulama bir kullanım lisansı isteğinde bulunduğunda, hak hesabı sertifikasını isteğe ekler. Lisans hizmeti içerik anahtarını şifrelemek için hak hesabı sertifikasının ortak anahtarını kullanır; böylece, yalnızca kimliği doğrulanan kullanıcıların kullanım lisansını kullanması sağlanır.

Hesap sertifikası işlemi aşağıdaki adımları içerir:

1.  Kullanıcı belirli bir bilgisayardan RMS korumalı içerik yayımlamayı veya RMS korumalı içeriği kullanmayı ilk kez denediğinde, RMS etkin uygulama kök sertifika sunucusunda çalışan hesap sertifikası hizmetine bir hak hesabı sertifikası isteği gönderir.
2.  Hesap sertifikası hizmeti Windows kimlik doğrulamasını kullanarak kullanıcı kimliğini doğrular.
3.  Hesap sertifikası hizmeti, kullanıcının doğrulanan kimlik bilgilerine dayanarak kullanıcı için hak hesabı sertifikası oluşturur. RMS makine sertifikasının ortak anahtarını kullanarak kullanıcının özel anahtarını şifreler ve şifrelenmiş anahtarı sertifikaya ekler. Daha sonra, hak hesabı sertifikasını istekte bulunan uygulamaya verir.
4.  Uygulama sonraki yayımlama ve kullanım lisansı isteklerinde kullanılabilmesi için bu hak hesabı sertifikasını bilgisayarda veya aygıtta depolar.

İstemcinin RAC isteğinde bulunmak için kullandığı hesap sertifikası hizmeti, RMS istemcisinin yüklü olduğu bilgisayarın türüne bağlıdır. Standart masaüstü bilgisayarlar hesap sertifikası hizmetine (certification.asmx) bağlanır. RMS SP1 ile kullanılmak üzere etkinleştirilen sunucu hizmetleri, RAC'leri sunucu sertifikası hizmetinden (ServeCertfication.asmx) alır. RMS SP1 ile kullanılmak üzere etkinleştirilen mobil aygıtlar, RAC'leri mobil aygıt sertifikası hizmetinden (MobileDeviceCertfication.asmx) alır. RMS SP1'in varsayılan yüklemesinde yalnızca hesap sertifikası hizmeti etkinleştirilir.

RMS SP1'i mobil aygıtlar ve sunucu hizmetleri ile birlikte kullanma konusunda daha fazla bilgi için, bu belge grubunun RMS Sunucusunu Çalıştırma bölümündeki "Mobil Aygıtlar ve Sunucu Hizmetleri için RMS Sunucusu Desteğini Etkinleştirme" konusuna bakın.
