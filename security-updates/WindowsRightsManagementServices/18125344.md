---
TOCTitle: 'RMS SSS: Güvenlik Konuları'
Title: 'RMS SSS: Güvenlik Konuları'
ms:assetid: 'ff433834-79aa-481f-bd39-3393be12a26f'
ms:contentKeyID: 18125344
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747757(v=WS.10)'
---

RMS SSS: Güvenlik Konuları
==========================

RMS Güvenlik Konuları Hakkında SSS
----------------------------------

-   [Süper kullanıcı hesabı nedir?](#bkmk_43)
-   [RMS bir güvenlik çözümü müdür?](#bkmk_44)
-   [Alıcıların, kullanım lisans süreleri dolduktan sonra, telif haklı belgelere erişimlerini uzatmak için istemci makinelerindeki saati geri almalarını engellemek üzere kullanılabilecek ne tür yöntemler vardır?](#bkmk_45)
-   [Domain Admins grubu üyeleri, etki alanlarındaki bir kişiye yönelik belgeleri okuyabilir mi?](#bkmk_46)
-   [Anladığım kadarıyla, her kasa, sistemde oluşturulan her sertifika ve lisansın kimliğini, Microsoft'a kaydettirilen bir hizmetten gelir gibi doğrulayabiliyor. Bu koruma hangi tehdide karşıdır?](#bkmk_47)
-   [Bir kaba tahmin saldırısı kullanarak bir belgeyi açabilen bir kişi, bu anahtarla başka belgeleri de açabilir mi?](#bkmk_48)
-   [Şifreleme teknolojilerine getirilen ihracat kısıtlamaları nedeniyle, anahtarların herhangi bir bölümü anahtarı dağıtan kuruluşun dışında açıklanabilir mi?](#bkmk_49)
-   [Kötü niyetli saldırganların yetki alma özelliğini uzaktan etkinleştirmesini nasıl engelliyorsunuz?](#bkmk_50)
-   [Kullanıcı tarafından telif haklı içeriğin ekran görüntüleri alınabilir mi?](#bkmk_51)
-   [RMS ile ilişkili dosyaların yedeğini oluşturan yöneticiler telif haklı içeriğe erişim hakkı kazanabilir mi?](#bkmk_52)
-   [Windows'un kullandığı takas dosyası, herhangi bir anda içeriği "açık" durumda bırakan, şifresi açılmış içerik bulundurur mu?](#bkmk_53)
-   [RMS'nin farklı yönetim özelliklerine erişebilecek yöneticileri sınırlama olanağı var mıdır?](#bkmk_54)
-   [RMS korumalı belgeler, oluşturuldukları anda, kullanıcının sabit diskine mi yoksa paylaşılan klasöre mi yerleştirilir?](#bkmk_55)
-   [Dosyayı açarken Otomatik Kaydetme Dosyası ve Geçici Dosyalar şifrelenir mi?](#bkmk_56)
-   [Telif haklı e-posta aldığımda, posta bir ekle birlikte görüntüleniyor. Posta kaydedilemiyor gibi görünüyor, ama eki kaydedebiliyorum, RMS bozulmuş olabilir mi?](#bkmk_562)

<span id="BKMK_43"></span>
#### Süper kullanıcı hesabı nedir?

RMS, tüm telif haklı içeriğin üzerinde tam denetime sahip özel bir Super Users grubunu destekler. Super Users grubu üyelerine, Super Users grubunun yapılandırıldığı RMS kümesi tarafından kendilerine verilen tüm kullanım lisanslarında tüm sahip hakları verilir. Dolayısıyla, bu grubun üyeleri her türlü korumalı dosyanın şifresini çözebilir ve bunların üzerindeki korumayı kaldırabilir. Bu grubun bir üyesi, örneğin yeni sahibin dosyaları yayımlayabilmesi ve yönetebilmesi için, işten çıkarılan bir çalışan tarafından yayımlanmış dosyalar üzerindeki korumayı kaldırabilir.

<span id="BKMK_44"></span>
#### RMS bir güvenlik çözümü müdür?

Hayır, RMS bir güvenlik çözümü değildir. Office 2007 gibi bir RMS etkin uygulamayla kullanıldığında, “ilke uygulama çözümü” olarak kabul edilebilir. Kullanıcı, verileri görüntüleme yetkisi yoksa, şifrelemeyi kırmaya çalışmak için bir kaba tahmin saldırısı kullanabilir. Şifreleme sağlam olsa da, tüm diğer yazılım şifreleme düzenleri gibi bu da kırılabilir. Ancak, kullanıcının verileri görüntüleme hakkı varsa, bu bilgileri kopyalayabilir, dijital fotoğrafını çekebilir ve yetkisi olmayan kullanıcılara verebilir.

<span id="BKMK_45"></span>
#### Alıcıların, kullanım lisans süreleri dolduktan sonra, telif haklı belgelere erişimlerini uzatmak için istemci makinelerindeki saati geri almalarını engellemek üzere kullanılabilecek ne tür yöntemler vardır?

RMS, istemci sistemindeki saatin ileri veya geri alındığını algılayarak kullanıcının içeriği kullanmasını engeller. RMS, buna ek olarak, RMS sunucusu ve istemcisi arasında ölçülebilir bir saat farkı olup olmadığını da algılar.

<span id="BKMK_46"></span>
#### Domain Admins grubu üyeleri, etki alanlarındaki bir kişiye yönelik belgeleri okuyabilir mi?

Domain Admins grubu üyeleri, RMS super user grubunun üyesiyse veya kullanıcı hesabının kimliğine bürünüyorsa, söz konusu kullanıcı hesabı için korunan içeriği okuyabilir. Domain Admins grubu üyelerinin etki alanındaki kullanıcı hesapları üzerinde denetimi olduğundan, Domain Admins grubunun güvenilmeyen bir üyesi olması senaryosunda bir değişiklik yoktur.

En iyi yöntemlerden biri, yalnızca Domain Admins grubu üyelerini, telif haklı içeriğe erişmeleri gerekiyorsa Super Users grubuna eklemektir. Super Users grubunun bir üyesine lisans verildiğinde, RMS sunucusunun Uygulama olay günlüğüne 49 no'lu olay kaydedilir. 49 no'lu olay açıklaması şu şekildedir: **“Super users grubundaki bir kullanıcıya lisans verildi. Kullanıcının e-posta adresi: &lt;Kullanıcı Diğer Adı&gt;”** burada **Kullanıcı Diğer Adı** yerine, kullanıcının e-posta hesabı yerleştirilir.

Diğer gruplarda kaynaklara erişimi sınırlamak için kullanıldığı gibi, Super Users grubu için de, herhangi bir kişinin bu gruba yetkisi olmadan katılmasını engellemeye yardımcı olmak üzere uyarı tanımlamalı ve güvenlik denetimleri yapmalısınız.

<span id="BKMK_47"></span>
#### Anladığım kadarıyla, her kasa, sistemde oluşturulan her sertifika ve lisansın kimliğini, Microsoft'a kaydettirilen bir hizmetten gelir gibi doğrulayabiliyor. Bu koruma hangi tehdide karşıdır?

Sertifikaların bütünlüğünü doğrulama olanağı olmadığında, bir kullanıcı başka bir kullanıcı için verilen hak hesabı sertifikasını (RAC) yanıltıcı bir şekilde kullanabilir ve içerik için kullanım lisansı alabilir veya belgeden korumayı kaldıran bir uygulama oluşturabilir.

<span id="BKMK_48"></span>
#### Bir kaba tahmin saldırısı kullanarak bir belgeyi açabilen bir kişi, bu anahtarla başka belgeleri de açabilir mi?

Telif haklı içeriğin her parçası rasgele oluşturulan farklı bir simetrik anahtarla şifrelenir. Bu nedenle, her belgenin anahtarı benzersizdir ve diğer belgelerin şifresini çözmek için kullanılamaz.

<span id="BKMK_49"></span>
#### Şifreleme teknolojilerine getirilen ihracat kısıtlamaları nedeniyle, anahtarların herhangi bir bölümü anahtarı dağıtan kuruluşun dışında açıklanabilir mi?

Microsoft kökünde imzalanan uygulamalar Microsoft anahtar imzalama köküne bağlıdır, ancak bu noktadan sonra, Microsoft tarafından veya müşterinin dağıtımı tarafından herhangi bir anahtar başkalarına gösterilmez.

<span id="BKMK_50"></span>
#### Kötü niyetli saldırganların yetki alma özelliğini uzaktan etkinleştirmesini nasıl engelliyorsunuz?

Saldırganın, RMS kümesinde yönetim haklarına sahip bir kullanıcı hesabının kimlik bilgilerine gereksinimi vardır. Varsayılan olarak, RMS yönetim arabirimi, RMS sunucusunda yalnızca yerel biçimde kullanılabilir. Durumun böyle olması sağlanarak, Uzak Masaüstü Protokolü (RDP) devre dışı bırakılır ve fiziksel olarak güvenli olan sunucu riski azaltmaya yardımcı olur.

<span id="BKMK_51"></span>
#### Kullanıcı tarafından telif haklı içeriğin ekran görüntüleri alınabilir mi?

RMS hakları kopyalama işlevine izin vermeyecek şekilde ayarlanırsa, RMS tarafından Windows Alt+PrtSc tuşlarının kullanımı devre dışı bırakılır. Ancak, yönetilmeyen masaüstlerinin bulunduğu ortamda, kullanıcı, içeriği yakalamak için Microsoft dışındaki ürünleri kullanabilir.

<span id="BKMK_52"></span>
#### RMS ile ilişkili dosyaların yedeğini oluşturan yöneticiler telif haklı içeriğe erişim hakkı kazanabilir mi?

Hayır, yedek oluşturabilirler, ancak erişim hakları yoktur.

<span id="BKMK_53"></span>
#### Windows'un kullandığı takas dosyası, herhangi bir anda içeriği "açık" durumda bırakan, şifresi açılmış içerik bulundurur mu?

RMS istemcisi şifresi çözülen içeriği uygulamaya geri gönderdikten sonra, bu içerik takas dosyasında görülebilir. Rights Management Services (RMS) Software Development Kit'te (SDK) bulunan RMS uygulama geliştirme önerilerinde bu oluşumun engellemesine yönelik adımlar vardır, ancak bunu uygulamanın yükü RMS etkin uygulamanın üzerine kalır.

<span id="BKMK_54"></span>
#### RMS'nin farklı yönetim özelliklerine erişebilecek yöneticileri sınırlama olanağı var mıdır?

Evet, Active Directory'de farklı RMS Admin grupları oluşturabilir, kullanıcı ekleyebilir ve sonra yönetim sayfaları için uygun bir erişim denetimi listesi (ACL) oluşturabilirsiniz. Örneğin, RMS yönetimi Web sayfası ACL'lerinin varsayılan yapılandırması, Güvenlik ayarları sayfasına yalnızca sunucuyu sağlama işlemi yapan kullanıcı tarafından erişilebileceğini belirtir.

<span id="BKMK_55"></span>
#### RMS korumalı belgeler, oluşturuldukları anda, kullanıcının sabit diskine mi yoksa paylaşılan klasöre mi yerleştirilir?

RMS, kullanıcının yerel bilgisayarında depolanan belgeleri korumak için kullanılabilse de, tercih edilen seçenek Şifreleme Dosya Sistemi'dir (EFS). RMS belgeyi korumak için kullanıcının aracılığını (fareyi birkaç kez tıklatma) gerektirirken, EFS belgeleri herhangi bir eylem gerektirmeden korur.

<span id="BKMK_56"></span>
#### Dosyayı açarken Otomatik Kaydetme Dosyası ve Geçici Dosyalar şifrelenir mi?

Evet, tüm geçici dosyalar şifrelenir.

<span id="BKMK_562"></span>
#### Telif haklı e-posta aldığımda, posta bir ekle birlikte görüntüleniyor. Posta kaydedilemiyor gibi görünüyor, ama eki kaydedebiliyorum, RMS bozulmuş olabilir mi?

Hayır. Beklenen davranış budur. Gördüğünüz ek, RMS istemcisi tarafından şifresi çözülmeden önceki şifreli iletidir. Telif haklı olma durumu devam eder ve şifresi çözüldükten sonra kaydedilemez.
