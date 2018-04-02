---
TOCTitle: RMS Yönetim Sorunları
Title: RMS Yönetim Sorunları
ms:assetid: '97013c08-d3fa-4ea0-8914-995b6c97f900'
ms:contentKeyID: 18125188
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747605(v=WS.10)'
---

RMS Yönetim Sorunları
=====================

RMS sunucunuzda başarılı bir şekilde yapılandırıldıktan sonra, RMS'nin günlük yönetimi sırasında sorunlarla karşılaşabilirsiniz. Bu sorunlardan bazılarını çözmenize yardımcı olmaları için aşağıdaki bölümlerde bulunan bilgileri kullanabilirsiniz.

RMS Yönetimi Web sitesi açılmaya çalışıldığında "SQL Server yok veya erişim engellendi" iletisi alındı.
-------------------------------------------------------------------------------------------------------

RMS'yi, veritabanı sunucunuz olarak SQL Server 2005'in yeni bir yüklemesini kullanarak yüklediyseniz, SQL Server Hizmeti başlamayabilir. SQL Server 2005'te MSSQLSERVER hizmeti, sunucu başladığında otomatik olarak başlamak üzere yapılandırılmaz. RMS'yi yükledikten sonra SQL Server'i yeniden başlattıysanız ve bu hizmeti otomatik olarak yeniden başlamak üzere yapılandırmadıysanız RMS çalışamaz ve RMS Genel Yönetimi sayfasına erişilemez.

MSSQLSERVER hizmetini başlattıktan sonra, RMS işlevselliğini geri yüklemek için RMS Sunucusunda IIS'yi yeniden başlatmanız gerekir.

Çevrimdışı Kayıt İşlemi Tamamlanamıyor
--------------------------------------

Kayıt isteği dosyası eksikse veya EnrollService Web sitesine gönderilmeden önce değiştirildiyse, çevrimdışı kayıt işlemini tamamlayamazsınız. Kayıt isteği dosyası, kötü amaçlı bir program tarafından veya kullanıcı hatası ya da sistem hatası nedeniyle bozulmuş olabilir.

EnrollService Web sitesi, eksik olan bilgiye bağlı olarak dosyayı yine de kabul ederek sunucu lisans sertifikası döndürebilir veya istek dosyasını reddederek hata verebilir.

Sunucu lisans sertifikası döndürülürse, bu sertifika, kayıt isteği dosyasında bulunan eksiklikleri veya bozuklukları yansıtır ve sertifikayı almaya çalıştığınızda RMS hata verir.

Kayıt işlemini tamamlayamıyorsanız, Internet bağlantısı olan bilgisayarda virüs olup olmadığını denetleyin, RMS sunucusundan kayıt isteği dosyasını yeniden verin ve sonra da bu dosyayı Internet bağlantısı olan bilgisayara aktarmak için farklı bir ortam kullanın. Hatayı almaya devam ediyorsanız, Microsoft Ürün Destek Hizmetleri'ne başvurmanız gerekir.

Günlük Dosyaları Oluşturulmadı
------------------------------

RMS Günlük Hizmeti, hem Message Queuing (MSMQ olarak da bilinir) hizmetini hem de günlük veritabanına erişim olmasını gerektirir. Günlük dosyaları oluşturulmuyorsa, bunun nedeni bileşenlerin doğru biçimde yapılandırılmamış olması veya bileşenler arasındaki iletişimin kesilmesi olabilir.

RMS sunucusunu ve veritabanı sunucusunu sınayarak ağ bağlantıları olduğundan emin olun. Ağ bağlantıları varsa, RMS günlük hizmetinin önkoşullarını gözden geçirmek ve tüm yazılım bağımlılıklarının doğru biçimde yapılandırıldığından emin olmak için aşağıdaki yordamları kullanın.

Öncelikle, Message Queuing yapılandırmasının doğruluğunu denetleyin. Message Queuing, Active Directory Tümleştirmesi etkinleştirilmiş olarak yüklenmelidir.

**Message Queuing hizmetinin doğru biçimde yüklenmiş ve yapılandırılmış olduğunu denetlemek için**
1.  **Denetim Masası**'nda **Program Ekle veya Kaldır**'ı tıklatın ve **Windows Bileşenleri Sihirbazı**'nı açmak için **Windows Bileşenlerini Ekle/Kaldır**'ı tıklatın.

2.  **Windows Bileşenleri Sihirbazı**'nda, **Uygulama Sunucusu** onay kutusunu seçin ve **Ayrıntılar**'ı tıklatın.

3.  **Message Queuing** onay kutusunu seçin ve ardından **Ayrıntılar**'ı tıklatın.

4.  **Active Directory Tümleşmesi** onay kutusu seçiliyse, sonraki sınamaya gidin ve Message Queuing hizmetinin çalıştığını doğrulayın. Onay kutusu seçiliyse, 5 ile 9 arasındaki adımları gerçekleştirin.

5.  **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gelin, **Windows RMS**'nin üzerine gelin ve sonra Genel Yönetim sayfasını açmak için **Windows RMS Yönetimi**'ni tıklatın.

6.  Windows RMS'nin sağlandığı Web sitesinin yanındaki **RMS'yi bu Web sitesinden kaldır**'ı tıklatın ve sonra **Tamam**'ı tıklatın.

7.  **Denetim Masası**'ndaki **Program Ekle veya Kaldır**'dan, **Windows Bileşenlerini Ekle/Kaldır**'ı tıklatın, **Uygulama Sunucusu**'nu tıklatın ve sonra **Message Queuing**'i tıklatın.

8.  **Active Directory Tümleşmesi**'ni etkinleştirmek için **Ayrıntılar**'ı tıklatın, **Active Directory Tümleşmesi** onay kutusunu seçin ve ardından **Tamam**'ı tıklatın.

9.  **Genel Yönetim sayfasını** açın. RMS sağlamak istediğiniz Web sitesinin adının yanındaki **RMS'yi bu Web sitesinde hazırla**'yı tıklatın.

İkinci olarak, Message Queuing hizmetinin sunucunuzda çalışıyor olduğunu doğrulayın.

**Message Queuing hizmetinin sunucunuzda çalıştığını doğrulamak için**
1.  **Denetim Masası**'nda **Yönetimsel Araçlar**'ı ve ardından **Hizmetler**'i tıklatın.

2.  **Message Queuing** hizmetini buluncaya kadar hizmetler listesinde aşağı doğru gidin.

3.  Hizmet, **Durum** sütununda **Başladı** olarak belirtilmelidir; bu şekilde belirtilmiyorsa, hizmeti sağ tıklatın ve ardından **Başlat**'ı tıklatın.

Üçüncü olarak, günlük hizmetinin, olayları günlük veritabanına yazma izni olduğunu doğrulayın. RMS günlük hizmeti, RMS hizmet hesabını kullanarak çalışır. RMS hizmet hesabının, veritabanı sunucusunda geçerli bir oturumu olduğunu ve kendisine, veritabanları oluşturmak ve dosyalara bilgi yazmak için gereken izinlerin verilmiş olduğunu doğrulayın.

Tüm bu önkoşullar karşılandıktan sonra, Hizmetler ek bileşenini kullanarak RMS günlük hizmetini durdurun ve yeniden başlatın. RMS günlük hizmeti yeniden başladıktan sonra, veritabanı sunucusunda günlük dosyaları oluşturulmalıdır. Veritabanı sunucunuz olarak SQL Server kullanıyorsanız, aşağıdaki yordam, oluşturulmakta olan günlük dosyalarının nasıl doğrulanacağını gösterir.

**SQL Server üzerine oluşturulmakta olan günlük dosyalarını doğrulamak için**
1.  SQL Server Enterprise Manager'da günlük veritabanına gidin, **Veritabanları**'nı genişletin ve sonra RMS günlüklerini içeren veritabanını genişletin.

2.  Günlük veritabanını tıklatın, **Tablolar**'ı tıklatın, **DRMS\_log\_master**'ı sağ tıklatın ve sonra **Tablo aç – tüm satırları getir**'i tıklatın. Günlük dosyaları oluşturulmaktaysa, bir veya daha fazla günlük dosyası göreceksiniz.

Yapılandırma Veritabanını Geri Yükleme
--------------------------------------

RMS, işlevsel bir yapılandırma veritabanı olmadan çalışamaz. Yapılandırma veritabanıyla ilgili, veritabanı bozulması veya veritabanı sunucusunda sabit disk hatası gibi sorunlarınız varsa, yapılandırma veritabanının yedeğini geri yükleyerek RMS işlevselliğini geri alabilirsiniz. RMS yapılandırma veritabanını yedekten geri yüklemek için aşağıdaki bilgilere gereksiniminiz vardır:

-   Veritabanının en son alınan yedeğinin adı.
-   Yedek veritabanının geri yükleneceği bilgisayarın adı.
-   RMS sağlama işlemi için kullanılan özgün hesap adı ve parola.
-   Yazılım özel anahtar koruması için belirtilen özgün parola (kullanıldıysa).

RMS tüm ayarları (yedek yapılandırma veritabanından aldığı) koruduğundan, yedek veritabanından geri yükleme işlemi için yeni bir sunucu lisans sertifikası veya yeni özel anahtar gerekmez.

Yedek veritabanını, aşağıdaki yordamı kullanarak geri yükleyebilirsiniz.

**Yedek veritabanını geri yüklemek için**
1.  **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gelin, **Windows RMS**'nin üzerine gelin ve sonra **Genel Yönetim** sayfasını açmak için **Windows RMS Yönetimi**'ni tıklatın.

2.  Windows RMS'nin sağlandığı Web sitesinin yanındaki **RMS'yi bu Web sitesinden kaldır**'ı tıklatın ve sonra **Tamam**'ı tıklatın.

3.  Yapılandırma veritabanınıza ait yedek veritabanı dosyalarını geri yükleyin. Yedekleme işlemi sırasında günlük veritabanınızı yedeklediyseniz ve verilerin devamlılığını sağlamak istiyorsanız, günlük veritabanını da geri yükleyin.

    -   Bu sistem tam bir sistem hatasından sonra geri yükleniyorsa, yedek veritabanı dosyalarını geri yüklemeden önce sistem durumu yedeğinizi kullanarak kayıt defterini geri yükleyin.

4.  Geri yüklenmekte olan veritabanı tek bir kök sertifikası sunucusuna yönelikse, hizmeti yeniden sağlamaya çalışmadan önce aşağıdaki kayıt defteri anahtarını değiştirin:

    -   Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda
        `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0\`
    -   Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda
        `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0\`

    Aşağıdaki girdiyi dize değeri olarak ekleyin ve değeri boş bırakın:

    `GicURL`

    Bu işlem, Active Directory'nin kök sertifika sunucusu bulma işlemini geçersiz kılar ve sayfaları sağlayan kök sertifika sunucusuna erişebilmenizi sağlar.

5.  RMS özel anahtarının güvenliğini sağlamak için bir donanım güvenlik modülü kullandıysanız, anahtarların alınabilmesi için yedek güvenlik evrenini geri yükleyin.

6.  Aşağıdaki adımlardan birini kullanın:

    -   Veritabanını bir küme için değil de tek bir sunucu için geri yüklemek için, RMS'yi sağlamak istediğiniz Web sitesinin yanındaki RMS'yi bu Web sitesinde hazırla'yı tıklatın.
        -veya-
    -   Veritabanını küme için geri yüklemek üzere, RMS'yi sağlamak istediğiniz Web sitesinin yanındaki Bu sunucuyu bir kümeye ekle'yi tıklatın.

7.  Sunucuyu sağlamak için kullanılan özgün RMS hizmet hesabını belirtin.

8.  Kullanmak istediğiniz yedek yapılandırma veritabanını (veritabanı adını ve veritabanının bulunduğu bilgisayarın adını da içerecek şekilde) belirtin.

9.  Bu sunucuyu sağlamak üzere kullandığınız özgün parolayla aynı parolayı belirtin.

10. **Gönder**'i tıklatın.

Sağlama işlemi başlar ve RMS sunucuda yeniden sağlanır.

Daha fazla bilgi için, bu belge grubundaki RMS Dağıtımı Planlama bölümünde bulunan Sistem Kurtarma Planlaması ve RMS Sistemini Yedekleme ve Geri Yükleme konularına bakın.

Süresi Dolan RMS Hizmet Hesabı Parolası
---------------------------------------

RMS'nin çalışması durursa, RMS hizmet hesabı parolasının süresi dolmuş olabilir. IIS Yöneticisi'ne bakın. RMS uygulama havuzları durdurulduysa ve bunları yeniden başlatamıyorsanız, RMS hizmet hesabı parolasının süresi dolmuş olabilir.

RMS hizmet hesabı parolanızın süresi dolarsa, hesabı süresi dolan parolayla kullanan her RMS sunucusunda parolayı değiştirmeniz ve IIS'yi yeniden başlatmanız gerekir. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "RMS Hizmet Hesabı Parolasını Değiştirme" konusuna bakın.

Önceki RMS Yüklemesini Geri Yükleme
-----------------------------------

RMS sunucusu donanımınız veya yazılımınızda hata oluşursa, yeni bir sunucu örneği sağlamak için, önceden yüklenmiş yapılandırma veritabanını kullanarak RMS sunucusunu geri yükleyebilirsiniz.

| ![](images/Cc747605.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                  |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu yordam yalnızca RMS çalıştıran sunucuda hata olması durumunda kullanılabilir. Yapılandırma veritabanınızı çalıştıran sunucuda hata olursa, bu konuda daha önce söz edilen "Yapılandırma Veritabanını Geri Yükleme" bölümüne bakın. RMS sunucunuz aynı zamanda veritabanı sunucunuz olarak da işlev görüyorsa, yedek kopyadan tüm sunucuyu geri yüklemeniz gerekir. |

Özgün yükleme için kullanılan yapılandırma veritabanını göstermek üzere aşağıdaki yordamı kullanın.

**Önceki RMS yüklemesini geri yüklemek için**
1.  RMS sunucusu olarak yapılandırmak istediğiniz bilgisayarda yönetim ayrıcalıklarına sahip bir hesap kullanarak oturum açın. Bu bilgisayarın RMS'ye yönelik en düşük sistem gereksinimlerini karşıladığından emin olun. RMS'ye yönelik sistem gereksinimleri hakkında daha fazla bilgi için bu belge grubundaki "RMS Dağıtımını Planlama" bölümünde bulunan "RMS için Donanım Gereksinimleri" konusuna bakın.

2.  RMS özel anahtarlarını korumak için donanım güvenlik modülü kullanıyorsanız, bu modülün, önceki RMS yüklemesiyle kullanmış olan ayarı ve güvenlik evrenini kullanılarak doğru yapılandırıldığından emin olun.

3.  RMS'yi bilgisayara yükleyin.

4.  RMS yüklemesini tamamladıktan sonra **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gelin, **Windows RMS**'nin üzerine gelin ve sonra **Genel Yönetim** sayfasını açmak için **Windows RMS Yönetimi**'ni tıklatın.

5.  RMS sağlamak istediğiniz Web sitesinin yanındaki **Bu sunucuyu bir kümeye ekle** bağlantısını tıklatın.

6.  **RMS hizmet hesabı** alanına, etki\_alanı\\kullanıcı\_adı şeklindeki RMS hizmet hesabı adını ve RMS'nin birçok normal işlem için altında çalışacağı RMS hizmet hesabının parolasını yazın. Bu bir etki alanı hesabı olmalıdır.

7.  **Yapılandırma veritabanı** alanında, kurtarmak istediğiniz özgün RMS yüklemesine yönelik veritabanı sunucusunun adını ve yapılandırma veritabanının adını belirtin.

8.  **Özel anahtar koruması** alanında, özel anahtarı korumak için bu küme tarafından kullanılan mekanizmayı seçin. Yazılım tabanlı özel anahtar koruması kullandıysanız, bu küme ilk sağlandığında özel anahtarı şifrelemek için kullanılan parolayı vermelisiniz.

9.  **Gönder**'i tıklatın.

İstemciler, izinlerinin süresi dolduğu için RMS korumalı içeriği açamıyor
-------------------------------------------------------------------------

Kullanıcının izinlerinin süresi dolarsa, RMS korumalı içeriği kullanamaz. RMS sunucusunun sistem saati RMS istemcisinin sistem saatinden ileriyse, kullanıcı, izinlerinin süresi dolmadığı halde RMS korumalı içeriği kullanamayabilir. İki bilgisayardaki sistem saatleri aynı olmadığı için, istemci bilgisayar içeriği açmaya çalıştığında aşağıdaki hata görüntülenebilir:

**İzninizin süresi dolduğundan bu iletiyi açma izniniz yok. Farklı bir kimlik bilgisi kümesi kullanarak açmak ister misiniz?**  

İstemci lisansı ve içerik lisansı geçerlidir, ancak saat farklılığı, istemcinin içerik lisansını geçersiz olarak yorumlamasına ve kullanıcıya bu hatayı döndürmesine neden olur. Bu da, kullanıcının, RMS hesap sertifikasıyla veya belge için kendisine verilen haklarla ilgili bir sorun olduğunu düşünmesine yol açar. İstemcideki saat, içerik yayımlama lisansının geçerlilik süresi aralığına geldikten sonra, kullanıcı içeriği açabilir.

İyi bir uygulama yöntemi olarak, RMS sistemindeki istemcileri ve sunucuları aynı saat hizmetiyle eşitlemelisiniz.

RMS, Olayları Uygulama Olay Günlüğüne Kaydetmeye Çalışırken "Erişim Engellendi" hatası oluştu
---------------------------------------------------------------------------------------------

Varsayılan olarak, RMS gibi ASP sayfasında çalıştırılan bileşenler IUSR\_COMPUTERNAME hesabı altında oluşturulur. Bu hesap Guests grubunun üyesidir ve uygulama olay günlüğüne yazmak için gereken güvenlik ayrıcalıkları, Guest hesaplarının olay günlüğüne veri yazmasını engeller.

Bu sorunu çözmek için, kayıt defteri düzenleyicisini kullanarak bu davranışı denetleyen kayıt defteri anahtarını değiştirebilirsiniz.

| ![](images/Cc747605.Caution(WS.10).gif)Dikkat                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kayıt defterinde yanlış düzenlemeler yapmak sisteminize ciddi zararlar verebilir. Kayıt defterinde değişiklik yapmadan önce, bilgisayarınızdaki değerli verileri yedeklemeniz gerekir. |

Aşağıdaki kayıt defteri anahtarını 1 yerine 0 olarak ayarlayın ve değişikliklerin etkili olması için bilgisayarınızı yeniden başlatın.

`HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\EventLog\Application`

Ad: `RestrictGuestAccess`

Tür: `REG_DWORD`

| ![](images/Cc747605.note(WS.10).gif)Not       |
|----------------------------------------------------------------------------|
| Bu ayar, tüm Guest hesaplarının Uygulama Olay Günlüğü'ne yazmasını sağlar. |

Bu hatanın nedeni hakkında daha fazla bilgi için [Microsoft Bilgi Bankası](http://go.microsoft.com/fwlink/?linkid=44167)'nda, günlüğü ASP sayfalarından etkinleştirmeyle ilgili makaleye bakın.
