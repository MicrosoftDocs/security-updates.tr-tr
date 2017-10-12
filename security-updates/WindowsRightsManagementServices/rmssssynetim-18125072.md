---
TOCTitle: 'RMS SSS: Yönetim'
Title: 'RMS SSS: Yönetim'
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18125072
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747547(v=WS.10)'
---

RMS SSS: Yönetim
================

RMS Yönetimi Hakkında SSS
-------------------------

-   [Kuruluştan ayrılan bir kullanıcının belgelere yönelik izinlerini iptal etmek için kullanılacak en iyi yöntem hangisidir?](#bkmk_1)
-   [RMS içeriği alışverişi yapmak üzere iki kuruluş arasında güven oluşturulduğunda, güvenen şirkete aktarılan XrML lisans sertifikası için özel bir işlem yapılması gerekir mi?](#bkmk_2)
-   [RMS gezici kullanıcı profilleriyle nasıl çalışır?](#bkmk_3)
-   [Bir kuruluş neden RMS'nin yetkisini almak ister?](#bkmk_4)
-   [Yetki alma süreci baştan sona nasıl işler?](#bkmk_5)
-   [Yalnızca bazı kullanıcıların belgeleri kurtarmasına olanak verilecek şekilde RMS sunucusunun yetkisi alınabilir mi?](#bkmk_6)
-   [Sunucu Uygulama Dizinine Erişemiyor hatası ne anlama gelir?](#bkmk_7)
-   [RMS sunucusuyla birlikte izleme kullanabilir miyim?](#bkmk_8)
-   [Saat farklılığı nedir ve nasıl yönetilmelidir?](#bkmk_9)

<span id="BKMK_1"></span>
#### Kuruluştan ayrılan bir kullanıcının belgelere yönelik izinlerini iptal etmek için kullanılacak en iyi yöntem hangisidir?

Genelde, belgelerin, tek tek kullanıcı hesapları yerine Active Directory'de tanımlanan kullanıcı gruplarına göre lisanslanması en iyi yöntemdir. Bu yöntemin önerilmesinin nedeni, bir kullanıcı kuruluştan ayrıldığında bu kullanıcının Active Directory grubundan kaldırılabilmesi ve dolayısıyla bu gruba gönderilen belgeleri okumasının engellenmesidir. Ancak, belgelerin hakları, belgenin her açılışında kullanıcının kullanım lisansı almasını gerektirecek şekilde ayarlanmadıysa, kullanıcı kullanım lisansı olan belgeleri okumaya devam edebilir. Bu hak tanımlanmadıysa, kullanıcının kullanım lisansına sahip olduğu belgeleri açmasını engellemenin tek yolu, kullanıcının lisans deposunu bilgisayarından silmektir.

<span id="BKMK_2"></span>
#### RMS içeriği alışverişi yapmak üzere iki kuruluş arasında güven oluşturulduğunda, güvenen şirkete aktarılan XrML lisans sertifikası için özel bir işlem yapılması gerekir mi?

Güvenilen bir kullanıcı etki alanı veya güvenilen bir yayımlama etki alanı oluşturduğunuzda, hak yönetimi sisteminize katılacak ortak kuruluşa güvenmeyi seçersiniz. Bu durumda, diğer kuruluşun bilgilerinize zarar vermeyeceğine güvenmenin riskini alırsınız. İyi bir uygulama yöntemi olarak, sunucu lisans sertifikasını RMS sunucunuza almadan önce bu sertifika üzerinde değişiklik yapılması riskini azaltmaya yardımcı olması için, ortak kuruluştan RMS sunucu lisans sertifikasını S/MIME e-postası gibi bir yetkili kanal kullanarak göndermesini isteyin.

<span id="BKMK_3"></span>
#### RMS gezici kullanıcı profilleriyle nasıl çalışır?

Kullanıcıları tanımlamak için kullanılan hak hesabı sertifikaları (RAC) bilgisayara özgüdür. Gezici profiller kullanılırken, RMS'nin bir bilgisayarda ilk defa kullanılması, kullanıcı için söz konusu bilgisayarda yeni bir RAC oluşturur.

<span id="BKMK_4"></span>
#### Bir kuruluş neden RMS'nin yetkisini almak ister?

RMS yetkisini almak, RMS sunucusunu altyapıdan çıkarır ve kullanıcıların telif haklı içeriği korumasız bir şekilde kaydetmesini sağlar. Kuruluşların bunu yapmayı seçmesinin üç temel nedeni vardır:

-   Mimari tasarımı basitleştirme (örneğin, sunucuları bir kümede birleştirme).
-   Prototip bir pilot ortamını üretim ortamına geçirme.
-   RMS sunucularını birleştirme (örneğin, bir satın alma işleminden sonra).

<span id="BKMK_5"></span>
#### Yetki alma süreci baştan sona nasıl işler?

Yetki alma süreci, RMS kök kümesi tarafından yetki alma hizmeti etkinleştirilerek başlatılır. Yetki alma hizmeti etkinleştirildiğinde, diğer tüm hizmetler (lisans ve sertifika gibi) devre dışı bırakılır. Ardından, her kullanıcının RMS etkin uygulamasının, RMS özelliği kullanıldığında yetki alma hizmetine bağlanacak şekilde yönlendirilmesi gerekir. RMS etkin uygulamalara örnek olarak Microsoft Office 2003 verilebilir. Office 2003'te, RMS istemcisi, kayıt defteri anahtarları kullanılarak RMS hizmetlerine yönlendirilir. Belirli bir kayıt defteri anahtarı yetki alma hizmetini tanımlar. Bu anahtar istemciyi yetki alma hizmetine yönlendirecek şekilde yapılandırıldıktan sonra, RMS kümesi kullanıcıya sağlanmış olan izinlerden bağımsız olarak, ilgili içerik için kendisine tüm izinleri (okuma, yazma, kopyalama, yazdırma, düzenleme, vb) sağlayan kullanım lisansları verir. Kullanıcılar, RMS kümesinin yetkisi tümüyle alındıktan sonra, tutmak istedikleri belgelerdeki tüm hak korumalarını kaldırmaya yönlendirilmelidir. Bu işlem yapıldıktan sonra, RMS kümesi tümüyle hizmet dışına alınabilir

RMS kümesi hizmetten çekildikten sonra telif haklı bir belgeyi geri yüklemeniz gerektiği durumlara yönelik iyi bir uygulama yöntemi olarak, RMS kümesi yapılandırma veritabanının yedeğini oluşturun. RMS kök kümesinin özel anahtarı olmadan, telif haklı içerik sunucu kaldırıldıktan sonra yalnızca belgenin yazarı tarafından açılabilir.

<span id="BKMK_6"></span>
#### Yalnızca bazı kullanıcıların belgeleri kurtarmasına olanak verilecek şekilde RMS sunucusunun yetkisi alınabilir mi?

Yetki alma hizmetine erişimi denetlemek için yetki alma Web hizmetine (decommission.asmx) bir erişim denetim listesi (ACL) uygulayarak, telif haklı içerik için yalnızca belirli kullanıcıların şifre çözme anahtarı alabilmesini sağlayabilirsiniz.

<span id="BKMK_7"></span>
#### Sunucu Uygulama Dizinine Erişemiyor hatası ne anlama gelir?

Bazen, RMS'yi yükledikten sonra yapılan ilk RMS yönetimi Web sitesini açma girişiminde bu hata görüntülenebilir. Bu hatayı aldıktan sonra RMS'yi yapılandıramaz veya yönetemezsiniz.

Bu hata, genellikle Internet Information Services (IIS), IIS 5.0 yalıtım modunda çalışırken oluşur. Bu ayarı sunucunuzda devre dışı bırakmak üzere aşağıdaki yordamı kullanın ve bu sorunu çözmek için IIS'yi yeniden başlatın.

**IIS 5.0 yalıtım modunu devre dışı bırakmak için**
1.  RMS sunucusunda yerel Administrators grubunun bir üyesi olarak oturum açın.

2.  **Başlat**'ı tıklatın, **Yönetimsel Araçlar**'ın üzerine gelin ve **Internet Information Services (IIS) Yöneticisi** öğesini tıklatın.

3.  **IIS Yöneticisi**'nde, yerel bilgisayarı genişletin, **Web Siteleri**'ni sağ tıklatın ve **Özellikler**'i tıklatın.

4.  **Hizmet** sekmesini tıklatın, **WWW hizmetini IIS 5.0 yalıtım modunda çalıştır** onay kutusundaki işareti kaldırın ve **Tamam**'ı tıklatın.

5.  Bu değişiklik IIS hizmetinin yeniden başlatılmasını gerektirir. IIS hizmetini yeniden başlatmanız istendiğinde, **Evet**'i tıklatın.

<span id="BKMK_8"></span>
#### RMS sunucusuyla birlikte izleme kullanabilir miyim?

Rights Management Services, Microsoft® .NET Framework kullanılarak oluşturulduğundan, sistem olaylarını kaydetmeye ve sorunları gidermeye yardımcı olmak üzere izleme işlevini etkinleştirebilirsiniz.

Web.config veya Machine.config dosyasını değiştirerek izleme uygulayabilirsiniz. İzlemeyi, Machine.config dosyasında uyguladığınızda, bilgisayardaki tüm yazılım bileşenleri için çalışır; ancak, Web.config dosyasında uygularsanız, yalnızca Web hizmetlerinde oluşan olaylar izlenir.

**İzlemeyi etkinleştirmek için**
1.  Machine.config dosyasını veya Web.config dosyasını açın ve sonra aşağıdaki satırları bu dosyadaki &lt;system.diagnostics&gt; bölümünün altına ekleyin:

    
        ```
2.  Komut isteminden IISRESET komutunu çalıştırarak IIS'yi yeniden başlatın.

3.  Gerekli olan verileri topladıktan sonra, 1. adımda eklediğiniz satırları .config dosyasından kaldırın.

4.  Komut isteminden IISRESET komutunu çalıştırarak IIS'yi yeniden başlatın.

| ![](images/Cc747547.Important(WS.10).gif)Önemli                                                                                                                                                                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS sunucusunda izleme kullandığınızda, kullanım lisansı almada ve hak hesabı sertifikası vermede oluşan uzun süreli gecikmeler gibi performans sorunları görülebilir. İzlemeyi, yalnızca varolan sorunları tanılamanıza ve gidermenize yardımcı olacağı sınırlı durumlarda kullanın. |

<span id="BKMK_9"></span>
#### Saat farklılığı nedir ve nasıl yönetilmelidir?

Saat farklılığı, bir bilgisayardaki saatin zamanıyla başka bir bilgisayardaki saatin zamanının farklı olmasıdır. Bu durum, bir odadaki iki kişinin kol saatlerinin saati biraz farklı göstermesi kadar olağan bir durumdur. Saat farklılığı, lisansta geçerlilik süresi belirttiğiniz durumlarda soruna neden olabilir.

Lisanstaki geçerlilik süresi, yayımcının saatine göre ayarlanır. Bunlar arasındaki saat farkı yayımlama ve kullanma döngüsünde iki noktada soruna neden olabilir:

-   Bir uygulama, RMS sunucusunun saatine göre geçerlilik süresi sona ermiş veya daha sonra başlayacak bir yayımlama lisansı kullanarak kullanım lisansı almaya çalıştığında. Bu durumda istek başarısız olur. Bu, son kullanıcı kullanım lisansı istediğinde veya uygulama belge için ön lisans almaya (kullanıcı adına kullanım lisansı almak için) çalıştığında oluşabilir.
-   Lisans geçerlilik süresi dolduysa (veya henüz başlamadıysa), lisans kullanma girişimi başarısız olur. Aksi durumda, yalnızca süresi dolan (veya henüz geçerli olmayan) haklar kullanılamaz.

Örneğin, yayımlama bilgisayarının saati kullanma bilgisayarının saatinden 15 dakika gerideyse ve yayımcı, içerik süresinin 15 dakika içinde dolacağını belirten bir yayımlama lisansı oluşturursa, kullanım lisansı tarafından içeriği görüntülemek için sağlanan hakların süresi zaten dolmuş olduğundan, kullanıcı sunucudan kullanılamayan bir kullanım lisansı alacaktır.

Saat farklılığı sorunlarına yönelik mükemmel bir çözüm yoktur. Olanağınız varsa, hakkın geçerlilik süresi başlangıcını, saatleri sizin saatinizden geride olan kullanıcıların o andaki saatlerinden önceki bir zamana ayarlamak ve lisans geçerlilik süresini de saatleri sizinkinden ileride olan kullanıcılar için uzatmak iyi bir çözümdür. Özellikle geçerlilik süreleri kısa olan lisanslar oluştururken saat farklılığı sorunlarının etkisini aklınızda bulundurmanız önerilir.
