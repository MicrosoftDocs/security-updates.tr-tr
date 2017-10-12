---
TOCTitle: 'RMS''yi Ormanlarda Dağıtma'
Title: 'RMS''yi Ormanlarda Dağıtma'
ms:assetid: 'd531dfdc-efff-4eb0-8d99-f1fd19d7a963'
ms:contentKeyID: 18125275
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747685(v=WS.10)'
---

RMS'yi Ormanlarda Dağıtma
=========================

Kuruluşunuzda birden çok Active Directory ormanı varsa ve RMS kullanımını kuruluşunuz genelinde etkinleştirmek istiyorsanız, ağınızı RMS'nin farklı ormanlarda bulunan kullanıcı hesaplarını ve dağıtım gruplarını tanıyabileceği ve bunların kimliklerini doğrulayabileceği şekilde yapılandırdığınızdan emin olun.

RMS kullanıcıları ve dağıtım gruplarını tanımak için Active Directory'yi kullanır. Bir kuruluşun Active Directory dağıtımı birden çok orman içerdiğinde, RMS, RMS sunucusundan farklı bir ormanda yer alan kullanıcıların ve grupların kimliklerini elde etmek için kişi nesnelerini kullanır. Bunu gerçekleştirmek için üç şey gereklidir:

1.  Diğer ormanda da RMS sertifika sunucularının bulunması ve her uzak grup için kişi nesnelerinin tanımlı olması gerekir.
2.  Ormanlarda, gerçek nesneleri içeren ormanları işaret etmelerine olanak tanıyan kişi nesnelerini içeren şema uzantılarının bulunması gerekir.
3.  Kişi nesnelerindeki özniteliklerin, gerçek nesneyi içeren ormanı işaret edecek şekilde eşitlenmesi gerekir.

Örneğin, gruplar bir ormanda oluşturulup yönetilirken kullanıcıların da başka bir ormanda oluşturulup yönetildiğini varsayalım. Kullanıcı belirli bir gruptaki üyeliğe dayanarak içeriğe haklar atamak istiyor. Bu senaryoda, *RMS\_Server\_U* kullanıcı hesaplarını içeren ormandaki sunucu ve *RMS\_Server\_G* grup hesaplarını içeren ormandaki sunucudur. Bu iki RMS sunucusu arasında güvenilen kullanıcı etki alanı kurulmuştur. *RMS\_Server\_U* sunucusunun yayımlama lisansında belirtilen grup üyeliğini orman sınırları çapında başarıyla genişletebilmesi için, yerel Active Directory ormanında uzak ormandaki grubu temsil eden bir kişi nesnesi bulunmalıdır. RMS kişi nesnesinin özniteliklerini sorgulayabilir ve bu nesnenin farklı bir ormanda bulunan bir grubu temsil ettiğini öğrenebilir. Daha sonra, ilgili ormanda bir RMS sunucusu arayabilir ve kendisiyle diğer RMS sunucusu arasında güven ilişkisi olup olmadığını belirleyebilir. *RMS\_Server\_U* sunucusu yayımlama lisansında belirtilen grup için Active Directory'yi sorguladığında, kişi nesnesi grubun başka bir ormana ait olduğunu belirler. *RMS\_Server\_U* sunucusu isteği ilgili etki alanının hizmet bağlantı noktasında (SCP) listelenen RMS sunucusuna iletir. SCP, *RMS\_Server\_G* sunucusunu etki alanı için RMS sertifika sunucusu olarak belirler. Daha sonra, *RMS\_Server\_U* sunucusu grup için üyelik elde etmek amacıyla *RMS\_Server\_G* sunucusunu sorgular.

RMS'nin bu bilgi için sorguladığı öznitelik **msExchOriginatingForest**'dır. Ormanınızda Exchange Server 2003 yüklüyse, bu öznitelik Active Directory şemasına varsayılan olarak yüklenir. Bu öznitelik, RMS'ye katılacak her Active Directory şemasının ormanında bulunmalıdır. Exchange Server 2003 kullanmıyorsanız, RMS Administration Toolkit'i karşıdan yükleyerek bu şema uzantılarını ekleyebilirsiniz. Araç seti bir şema dosyası ve Active Directory'ye nasıl ekleneceğini açıklayan yönergeler içerir.

Kişi nesnesinin diğer ormanlardaki gerçek nesneleri işaret edebilmesi için bu özniteliklerin eşitlenmesi gerekir. Bu öznitelik Active Directory şemanıza eklendikten sonra, değerini, grubun içinde bulunduğu ormanın tam etki alanı adı (FQDN) olacak şekilde yapılandırmanız gerekir; örneğin, corp.fabrikam.com.

Bu işlemi Microsoft Identity Integration Server (MIIS) 2003 veya Identity Integration Feature Pack'i (IIFP) ve Active Directory genel adres listesi (GAL) için yönetim aracını kullanarak gerçekleştirebilirsiniz.

Uzak Active Directory'yi aramak için yeterli ayrıcalıklara sahip olmak ve uzak RMS yüklemesindeki .NET Uzaktan Erişim arabirimlerine çağrıda bulunabilmek için yerel RMS sunucusunu etkinleştirmeniz gerekir.

Ormanlar arasında grup genişletmesini desteklemek için, her ormandaki RMS hizmet hesabı için kullanılan hesabın Active Directory'de okuma ve yürütme izinlerine de sahip olması gerekir. RMS etki alanı kimlik bilgilerine sahip, kimliği doğrulanmış tüm kullanıcılara otomatik olarak okuma erişimi izni verir. Güvenliği artırmak için, isteğe bağlı erişim denetim listesinden (DACL) bu erişimi kaldırabilir ve bunu farklı ormanlardaki bağımsız hizmet hesaplarıyla değiştirebilirsiniz.

RMS hizmet hesabı için gereken izinler, Active Directory güven ilişkilerinin yerel ormanlar arasında mı yoksa uzak ormanlar arasında mı olduğuna bağlı olarak farklılık gösterebilir. Aşağıdaki liste gereken güven modellerini ve izinleri tanımlar:

-   **İki yönlü güven var**. Yerel RMS ormanı, grubun ait olduğu ormana güvenir ve bu orman da ona güvenir. Her bir ormandaki RMS sunucusuna yönelik RMS hizmet hesabı, ormandaki herhangi bir geçerli etki alanı hesabı olabilir. Yerel RMS hizmet hesabını, grubun ait olduğu ormandaki tüm RMS sunucularının \\Inetpub\\wwwroot\\\_wmcs\\drmRemote klasöründeki DACL'ye eklediğinizden emin olun.
-   **Tek yönlü güven var**. Yerel RMS ormanı, grubun ait olduğu ormana güvenir, ancak söz konusu orman ona güvenmez. Kuruluştaki tüm RMS sunucuları için RMS hizmet hesabının, güvenilen ormandaki geçerli bir etki alanı hesabından olması gerekir. Bu hesabı grubun ait olduğu ormandaki tüm RMS sunucularının \\Inetpub\\wwwroot\\\_wmcs\\drmRemote klasöründeki DACL'ye eklediğinizden emin olun.
-   **Güven yok**. Kuruluştaki ormanlar diğer ormanlardaki kullanıcıların ve grupların kimliğini doğrulayamaz. İlgili gruplar arasında güven ilişkisi yoksa, ormanlar arası grup genişletmeyi kullanmamanız önerilir. Ancak, işiniz gereği böyle yapmanız gerekiyorsa, RMS hizmet hesabını her iki ormanda da geçerli bir etki alanı hesabı olarak yapılandırıp bu senaryoyu etkinleştirebilirsiniz; bu hesapların her biri için aynı kullanıcı adını ve parolasını kullanmanız gerekir. Bunun yanında, her RMS ön uç sunucusunda her iki ormandaki RMS hizmet hesabı için kullanılan etki alanı hesaplarıyla aynı kullanıcı adına ve parolasına sahip bir yerel makine hesabının oluşturulması gerekir. Bu, yerel hizmete otomatik olarak hem uzak Active Directory'de hem de uzak RMS sunucusunda kimlik doğrulaması için yeterli izinleri sağlar.

RMS Güven İlkelerini Kullanma
-----------------------------

Birden çok ormanı olan bir kuruluşta RMS dağıtıldığında, RMS sistemine katılacak kullanıcı hesaplarını barındıran her ormanda bir RMS sertifika sunucusu dağıtılması gerekir. Farklı ormanlardaki kullanıcıların RMS korumalı içeriği paylaşabilmesini istiyorsanız, diğer RMS sunucusu tarafından oluşturulan sertifikalara ve lisanslara güvenilebilmesi için RMS güven ilkelerini yapılandırmanız gerekir. RMS'de güvenilen kullanıcı etki alanları ve güvenilen yayımlama etki alanları olmak üzere iki güven ilkesi bulunmaktadır. Güvenilen kullanıcı etki alanları bir RMS sunucusunun başka bir RMS sertifika sunucusu tarafından oluşturulan hak hesabı sertifikalarına (RAC) güvenmesine ve diğer sunucudan RAC almış kullanıcılara kullanım lisansları vermesine olanak tanır. Güvenilen yayımlama etki alanları, bir RMS sunucusunun, diğer lisans sunucusunu belirten yayımlama lisanslarını temel alan kullanım lisansları oluşturmasına olanak verir.

Birden çok ormanı desteklemek için güven ilkelerini nasıl kullanabileceğinize yönelik bazı seçenekler şöyledir:

-   Her ormanda bir RMS sertifika kümesi ve tüm kullanıcılar tarafından paylaşılan tek bir lisans kümesi. RMS lisans kümesi tüm RMS sertifika kümelerini içeren bir güvenilen kullanıcı etki alanıyla yapılandırılır. RMS istemcileri kullanım lisansları elde etmek amacıyla lisans kümesine bağlanmak için kayıt defteri anahtarı kullanılarak yapılandırılır.
-   Her ormanda bir RMS sertifika ve lisans kümesi; her kümede diğer ormanlardaki RMS sunucularına güvenecek şekilde yapılandırılmış bir güvenilen etki alanı. Her kullanıcı lisans almak için kendi ormanındaki RMS sunucusunu kullanır ve Active Directory'deki hizmet bağlantı noktası aracılığıyla kendi lisans sunucusunu bulabilir.
-   RMS korumalı içeriği kullananlar içeriğin yayımlandığı ormana erişimi olmayan bir orman parçasına aitse, içeriğin lisanslanmasına ve kullanılmasına olanak tanımak için bir güvenilen yayımlama etki alanı kurulabilir. Güvenilen yayımlama etki alanları, içeriği yayımlamak için kullanılan RMS sunucusunun özel anahtarının alınmasını gerektirir.

Güven ilkesi yapılandırma hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Güven ve Güven İlkesini Yönetme" konusuna bakın.
