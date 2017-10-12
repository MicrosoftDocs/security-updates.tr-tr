---
TOCTitle: 'RMS SSS: Dağıtım'
Title: 'RMS SSS: Dağıtım'
ms:assetid: '5559ae65-77ae-4e0b-bfd8-3512409ed29b'
ms:contentKeyID: 18125098
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720274(v=WS.10)'
---

RMS SSS: Dağıtım
================

RMS Dağıtımı Hakkında SSS
-------------------------

-   [RMS için kullanılan güvenlik sorumluları genel adres listesi (GAL) üyesiyse, herhangi bir Exchange sürümü bağımlılığı söz konusu mudur?](#bkmk_20)
-   [SQL Server'ın RMS'deki rolü nedir?](#bkmk_21)
-   [Kullanıcı bilgisayarının RMS kullanması için RMS kök kümesiyle aynı etki alanına mı katılması gerekir?](#bkmk_22)
-   [Kullanıcı RMS Sunucusunu çevre ağına yerleştirmek isterse, RMS ile iletişim kurmak için Internet'e açılan güvenlik duvarında ve intranete açılan güvenlik duvarında hangi bağlantı noktaları açılmalıdır?](#bkmk_23)
-   [Yalnızca lisans sağlayıcı kümesindeki alt kayıt sunucuları nasıl kaydedilir ve istemcilere bu küme hakkında bilgilendirmek için bir şey yapmam gerekir mi?](#bkmk_24)
-   [Lisans sağlayıcı küme kullanmanın yararları nelerdir?](#bkmk_25)
-   [RMS yüklemesini tümüyle geri almak için ne yapmam gerekir?](#bkmk_26)
-   [RMS istemcisini, Program Ekle veya Kaldır'ı kullanarak kaldırdıktan sonra, başka bir dosya kaldırmam gerekir mi?](#bkmk_27)
-   [RMS, FAT dosya sistemiyle çalışır mı?](#bkmk_28)
-   [RMS tarafından kullanılan veritabanı sunucusu için hangi normal donanım yapılandırması önerilir?](#bkmk_29)
-   [RMS'nin grup genişletmesi için genel katalog kullanımı genel katalog sunucu performansını nasıl etkiler?](#bkmk_30)
-   [RMS, Active Directory'de şema değişikliği gerektirir mi?](#bkmk_31)
-   [Hizmet bağlantı noktası (SCP), RMS kümesinin yüklendiği etki alanındaki farklı etki alanı denetleyicileri arasında otomatik olarak çoğaltılır mı?](#bkmk_32)
-   [Kullanıcıların kendi makinelerinde yönetim hakları yoksa, RMS istemcisi nasıl yüklenir ve yapılandırılır?](#bkmk_33)
-   [RMS'nin ölçeklenebilirliği ne demektir?](#bkmk_35)
-   [RMS, donanımdaki RMS anahtarlarının güvenliğini sağlamak için donanım güvenlik modüllerini (HSM) destekler mi?](#bkmk_36)

<span id="BKMK_20"></span>
#### RMS için kullanılan güvenlik sorumluları genel adres listesi (GAL) üyesiyse, herhangi bir Exchange sürümü bağımlılığı söz konusu mudur?

RMS, Active Directory'ye bağlıdır, ancak Exchange'e bağlı değildir. Bununla birlikte, Exchange 5.5 kendi dizinini sağlar ve Active Directory'yi kullanmaz. Active Directory'deki tüm kullanıcı ve grup nesnelerinin, tam etki alanı adını içeren geçerli bir e-posta özniteliği olduğundan emin olun. 2000 veya daha sonraki sürümünü kullanıyorsanız, bu işlem otomatik olarak yapılır.

<span id="BKMK_21"></span>
#### SQL Server'ın RMS'deki rolü nedir?

RMS, tüm hizmet yapılandırma verilerini, sistemdeki sorumlular hakkındaki bilgileri ve tüm günlük verilerini depolamak ve Active Directory ve dağıtım listesi genişletme işlemi sırasındaki aramaları önbelleğe almak için veritabanı kullanır. RMS, SQL Server 2000 ve SQL Server 2005 ile tam olarak test edilmiştir.

<span id="BKMK_22"></span>
#### Kullanıcı bilgisayarının RMS kullanması için RMS sunucusuyla aynı etki alanına mı katılması gerekir?

Kullanıcı bilgisayarının RMS kümesiyle aynı etki alanının üyesi olması gerekmez, ancak bilgisayarın bir RMS kümesi bulabilmesi gerekir. İstemci bilgisayarların RMS kümesini bulmak için kullanabilecekleri en kolay yöntem, hizmet bağlantı noktası (SCP) aracılığıyla Active Directory araması kullanmaktır. Ancak, Active Directory araması kullanmadan RMS kümesini bulmak için istemcideki kayıt defteri ayarları da belirlenebilir. Kesin kayıt defteri ayarları RMS etkin uygulamaya bağlıdır.

<span id="BKMK_23"></span>
#### Kullanıcı RMS Sunucusunu çevre ağına yerleştirmek isterse, RMS ile iletişim kurmak için Internet'e açılan güvenlik duvarında ve intranete açılan güvenlik duvarında hangi bağlantı noktaları açılmalıdır?

İç kullanıcıların, hak hesabı sertifikaları (RAC) ve kullanım lisansları veren RMS sunucularına erişmeleri gerekir. RMS sunucusu, sunucunuzun SSL kullanmak üzere yapılandırılmış olup olmamasına göre, varsayılan olarak HTTP'yi (TCP 80 bağlantı noktası) veya HTTPS'yi (TCP 443 bağlantı noktası) dinlediğinden, bu bağlantı noktalarının Internet'e açılan güvenlik duvarında açık olması gerekir. Intranet'e açılan güvenlik duvarındaki etki alanında bulunan üye sunucular tarafından kullanılan ek bağlantı noktalarını açmanız gerekir.

<span id="BKMK_24"></span>
#### Yalnızca lisans sağlayıcı kümesindeki alt kayıt sunucuları nasıl kaydedilir ve istemcilere bu küme hakkında bilgilendirmek için bir şey yapmam gerekir mi?

Kuruluşta kök kümesin içinde ilk RMS sunucusu oluşturulduğunda, bu sunucu Microsoft Kayıt Hizmeti'nden sunucu lisans sertifikası alır. Başka bir RMS sunucusu yüklendiğinde ve sağlandığında, bunu kök kümesine katabilir veya bunu yalnızca lisans sağlayıcı kümede bir sunucu olarak kaydedebilirsiniz. Alt yalnızca lisans sağlayıcı sunucusu olarak kaydettirmeyi seçerseniz bu sunucu, RMS kök kümesine bir kayıt isteği gönderir. RMS etkin uygulamalar, istemci uygulamasının yalnızca lisans sağlayıcı kümeyi arayacağı yeri belirtir. Office 2003, varsayılan olarak kök kümesine dayalı bir RMS etkin uygulama örneğidir. Bu davranış kayıt defteri ayarlarıyla geçersiz kılınarak, uygulamanın yeni alt yalnızca lisans sağlayıcı küme araması sağlanabilir.

<span id="BKMK_25"></span>
#### Alt lisans sağlayıcı küme kullanmanın yararları nelerdir?

Yararlarından biri, kuruluştaki bölümleri birbirinden ayırmaktır. RMS kümesi arasında güvenilen bir yayımlama etki alanı oluşturulmazsa, içeriği yalnızca ilgili lisans sunucusuna erişim hakkı olan kullanıcılar kullanabilir. Bu yöntemle, hukuk bölümü, RMS şifreli e-postalarının bölüm dışındakiler tarafından okunmasını engelleyebilir. Buna ek olarak, yalnızca lisans sağlayıcı sunucuda, hak şablonları, günlüğe kaydetme, Super Users grubu üyeliği ve dışlama ilkeleri gibi çeşitli seçenekler ayarlanabilir.

<span id="BKMK_26"></span>
#### RMS yüklemesini tümüyle geri almak için ne yapmam gerekir?

RMS yüklemesini düzgün bir şekilde geri almak için aşağıdaki yordamı uygulayın.

**RMS yüklemesini geri almak için**
1.  RMS kümenizin hizmet bağlantı noktasını (SCP), RMS yönetimi Web sitesini kullanarak kaldırın.

2.  Sunucudaki RMS yapılandırmasını geri almak için **Genel Yönetim** sayfasından, **RMS'yi bu Web sitesinden kaldır**'ı tıklatın. Önce yalnızca lisans sağlayıcı kümelerdeki sunucuların yapılandırmasını geri almanız ve ardından kök kümesi sunucularının yapılandırmasını geri almanız gerekir.

3.  **Denetim Masası**'nda **Program Ekle veya Kaldır**'ı tıklatın ve **Rights Management Services**'i kaldırın.

4.  Veritabanı sunucunuzda, kalan tüm RMS veritabanlarını kaldırın.

5.  RMS hizmet hesabını, veritabanı sunucularınızdaki yetkili oturumlar listesinden kaldırın ve ardından hesabı Active Directory'den de kaldırın.

6.  RMS istemcileri Windows XP ve Windows 2000 çalıştırıyorsa, istemci bilgisayarlardan RMS istemcisini kaldırın.

| ![](images/Cc720274.Important(WS.10).gif)Önemli                                                                                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu yordam tamamlandıktan sonra, telif haklı içeriği açamazsınız. Değerli verileri korumak için RMS kullanıldıysa, RMS yüklemesini geri almadan önce RMS'nin yetkisini alın. |

<span id="BKMK_27"></span>
#### RMS istemcisini, Program Ekle veya Kaldır'ı kullanarak kaldırdıktan sonra, başka bir dosya kaldırmam gerekir mi?

Gerekli değilse de, %systemroot%\\system32 dizininden kasayı silebilirsiniz.

<span id="BKMK_28"></span>
#### RMS, FAT dosya sistemiyle çalışır mı?

Evet. NTFS dosya sistemi önerilse de, RMS, bilgisayarda FAT sistemini kullanarak çalışır.

<span id="BKMK_29"></span>
#### RMS tarafından kullanılan veritabanı sunucusu için hangi normal donanım yapılandırması önerilir?

Günlük veritabanı, özellikle RMS'nin yoğun olarak kullanıldığı ortamlarda hızlı bir şekilde büyür. Veritabanı sunucunuz için SQL Server kullanmayı düşünüyorsanız, Windows 2000 Advanced Server veya Windows Server 2003, Enterprise Edition üzerinde, etkin beklemede yapılandırmasına sahip bir kümede yapılandırılan SQL Server 2000 Enterprise Edition veya SQL Server 2005 Enterprise Edition kullanmayı düşünmelisiniz. Bu durumda, önerilen yapılandırmalar RAID-1 günlük diskleri ve RAID-5 veri diskleri ile en az 512 MB RAM'dir. Bu yapılandırma için önerilen en düşük CPU, 1,4 GHz hızında çalışan Pentium III'tür. Ayrılmış veritabanı sunucularında, birden çok CPU gerekmez.

<span id="BKMK_30"></span>
#### RMS'nin grup genişletmesi için genel katalog kullanımı genel katalog sunucu performansını nasıl etkiler?

RMS sunucusu grup genişletme listelerini önbelleğe aldığından, bu işlem genel katalog sunucusuna fazla yük getirmemelidir. Grup üyeliğinde sık olarak yapılan güncelleştirmeler genel katalog sunucusu gereksinimini artırsa da, yeni grup listelerini alma işleminin zaman aşımı değeri kayıt defteri kullanılarak yapılandırılabilir. Büyük grupların sık olarak genişletilmesi performansı düşürür. Daha fazla bilgi için bu belge grubunda "RMS: İşlemler" bölümünde bulunan "Active Directory Önbellek Ayarlarını Değiştirme" konusuna bakın.

<span id="BKMK_31"></span>
#### RMS, Active Directory'de şema değişikliği gerektirir mi?

RMS'nin yayımlama lisansında belirtilen grubu orman sınırları çapında başarılı bir şekilde genişletmesi için, yerel Active Directory ormanında uzak ormandaki grubu temsil eden bir kişi nesnesi bulunmalıdır. RMS, kişi nesnesinin özniteliklerini sorgulayabilir ve bu nesnenin farklı bir ormandaki grubu temsil ettiğini ortaya çıkarabilir.

RMS'nin bu işlemi yapması için, Active Directory, Exchange Server 2003 veya daha ilerisi şema özniteliğinin msExchOriginatingForest olmasını gerektirir. Ormanda çalışan tek bir Exchange Server 2003 sunucunuz varsa, bu öznitelik Active Directory şemasına varsayılan olarak yüklenir. Bu öznitelik, RMS'ye katılacak her Active Directory şemasının ormanında bulunmalıdır. Exchange Server 2003 kullanmıyorsanız, RMS Yönetim Araç Seti'ni kullanarak şemayı Active Directory yapınıza ayrı olarak yükleyebilirsiniz.

<span id="BKMK_32"></span>
#### Hizmet bağlantı noktası (SCP), RMS sunucusunun yüklendiği etki alanındaki farklı etki alanı denetleyicileri arasında otomatik olarak çoğaltılır mı?

Ormana ilk RMS sunucusu sağlandıktan sonra, bu sunucunun Active Directory'deki Yapılandırma kapsayıcısında bulunan Hizmetler kapsayıcısının altında bir kapsayıcı nesnesi oluşturmak için yeterli izni olan bir etki alanı hesabı kullanılarak Active Directory'ye kaydettirilmesi gerekir. Enterprise Admins yerleşik güvenlik grubu, gereken izinlere sahip hesaba örnek olarak verilebilir. Bu işlem, SCP'yi oluşturur. Bu, Hizmetler kapsayıcısında olduğundan, Active Directory bilgiyi ormandaki tüm etki alanı denetleyicilerine çoğaltır.

<span id="BKMK_33"></span>
#### Kullanıcıların kendi makinelerinde yönetim hakları yoksa, RMS istemcisi nasıl yüklenir ve yapılandırılır?

RMS istemcisi bir Windows Installer dosyasıdır ve Systems Management Server 2003 gibi bir yazılım dağıtımı altyapısı kullanılarak dağıtılabilir. RMS istemcisi, yönetim haklarına sahip bir hizmet hesabı kullanan Grup İlke nesnesiyle (GPO) de dağıtılabilir. RMS istemcisi Windows Vista çalıştırıyorsa, işletim sistemiyle tümleşik olduğu için artık ayrı bir RMS istemci yüklemesi gerekli olmaz.

<span id="BKMK_35"></span>
#### RMS'nin ölçeklenebilirliği ne demektir?

RMS durum bilgisi olmayan bir Web hizmetidir ve diğer Web siteleri veya hizmetleri gibi kümelendirilebilir ve yük dengelemesi yapılabilir. RMS performansı çoğunlukla işlemcinin kullanılabilirliğine bağlı olduğundan, işlemci eklemek performansı artırabilir.

<span id="BKMK_36"></span>
#### RMS, donanımdaki RMS anahtarlarının güvenliğini sağlamak için donanım güvenlik modüllerini (HSM) destekler mi?

Evet. RMS, nCipher HSM gibi CAPI uyumlu HSM'lerle çalışır.
