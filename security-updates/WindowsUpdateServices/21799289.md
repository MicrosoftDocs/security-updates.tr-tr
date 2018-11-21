---
TOCTitle: 'Windows Server Update Services 3.0 SP2 Sürüm Notları'
Title: 'Windows Server Update Services 3.0 SP2 Sürüm Notları'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21799289
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939886(v=WS.10)'
---

Windows Server Update Services 3.0 SP2 Sürüm Notları
====================================================

Bu sürüm notları, Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) sürümünü açıklar. Bu belge aşağıdaki bölümleri içerir:

1.  Bu Sürümdeki Yenilikler
2.  WSUS 3.0 SP2 Sunucu Yüklemesi için Sistem Gereksinimleri
3.  WSUS Sunucusu için Yapılandırma Önkoşulları ve En İyi Uygulama Önerileri
4.  Windows Small Business Server Önkoşulları
5.  WSUS 3.0 SP2 Uzak Konsolu Yüklemesi için Sistem Gereksinimleri
6.  İstemci Yüklemesi için Sistem Gereksinimleri
7.  Yükseltme Gereksinimleri ve Öneriler
8.  WSUS 3.0 SP2'yi Yükleme
9.  Katılımsız WSUS 3.0 SP2 Yüklemeleri için Kurulum Komut Satırı Parametreleri
10. Bilinen Sorunlar

Bu Sürümdeki Yenilikler
-----------------------

-   Windows Server 2008 R2 ile tümleştirme.
-   Windows Server 2008 R2'deki BranchCache özelliğine yönelik destek
-   Windows 7 istemcilerine yönelik destek.
-   Windows Update Aracısı (WUA) istemci iyileştirmeleri. Yeni WUA istemcisi çeşitli performans geliştirmeleri ve kullanıcı deneyimi iyileştirmelerine ek olarak müşteri geribildirimlerine dayalı hatalara yönelik bir dizi düzeltme sunar.
    -   İstemci tarama işlemi önceki sürümlerden daha hızlı gerçekleştirilir.
    -   WSUS sunucuları tarafından yönetilen bilgisayarlar artık tam tarama gerçekleştirmek yerine aynı WSUS sunucuları için ‘kapsamı belirlenmiş’ tarama işlemleri gerçekleştirir.  Böylece, Windows Defender gibi Microsoft Update API'lerini kullanan uygulamalar için hedefe yönelik tarama işlemleri çok daha hızlı yapılır.
    -   Windows Update Aracısı (WUA) kullanıcı deneyimi iyileştirmeleri, kullanıcıların güncelleştirmeleri daha iyi düzenlemelerine, güncelleştirmenin değeri ve davranışı konusunda daha fazla bilgiye sahip olmalarına yardımcı olur.
    -   Görüntüsü oluşturulan makineler WSUS konsolunda daha açık görüntülenir. Daha fazla bilgi için, [Windows 2000, Windows Server 2003 veya Windows XP görüntüsü kullanılarak kurulan Windows 2000, Windows Server 2003 veya Windows XP tabanlı bir bilgisayar WSUS konsolunda görünmüyor](http://go.microsoft.com/fwlink/?linkid=159749) konulu makaleye bakın.
-   Yeni özellikler:
    -   Otomatik onay kuralları artık tüm bilgisayarlar veya belirli bilgisayar grupları için onay son tarihinin ve saatinin belirtilebilmesini sağlayan bir özellik içermektedir.
    -   Akış aşağı sunucularda dil seçiminin daha gelişmiş olarak işlenebilmesi, yalnızca belirtilen dillere yönelik güncelleştirmeleri karşıdan yüklediğinizde görüntülenen yeni bir uyarı iletişim kutusu içermektedir.
    -   Yeni Güncelleştirme ve Bilgisayar Durumu raporları, yükleme için onaylanan güncelleştirmelere filtre uygulayabilmenizi sağlar. Bu raporları WSUS konsolundan çalıştırabilir veya uygulama programı arabirimini (API) kullanarak bu işlevselliği kendi raporlarınızla birlikte kullanabilirsiniz.
-   Kullanıcı arabirimi, hem istemcide hem de sunucuda WSUS 3.0 Service Pack 1 ve Service Pack 2 arasında uyumludur.
-   Yazılım güncelleştirmeleri.
-   Windows Update Aracısı'nda bu sürümle birlikte giderilen bilinen sorunlar:
    1.  WSUS 3.0 SP2 ve Windows 7, Windows Update Aracısı'nın yeni bir sürümünü içermektedir (Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 ve Windows Server 2008 için). Bu sürüm şu sorunları giderir: Etkileşimli olmayan bir oturumda yerel olmayan sistem arayanları tarafından çağrılan API'ler başarısız oluyor.
    2.  Windows Update Aracısı'nın 7.2.6001.788 sürümü tarafından giderilen sorun. Bu güncelleştirme şu sorunları giderir: Windows Update Web sayfasından veya Microsoft Update Web sayfasından aynı anda 80 veya daha fazla güncelleştirme yüklemeye çalıştığınızda 0x80070057 hata kodunu alıyorsunuz.
    3.  Windows Update Aracısı'nın 7.2.6001.784 sürümündeki geliştirmeler ve bu sürüm tarafından giderilen sorunlar. Bu güncelleştirme şunları içermektedir: Windows Update hizmetinin tarama süresini kısaltır, imza güncelleştirmelerinin teslim edilme hızını artırır, Windows Installer yeniden yükleme işlevselliği için destek sağlar ve hata iletilerini geliştirir.

<span id="BKMK_SysReqWSUS30SP2"></span>
WSUS 3.0 SP2 Sunucu Yüklemesi için Sistem Gereksinimleri
--------------------------------------------------------

Bu bölümde, WSUS 3.0 SP2 yüklemesi için yazılım ve donanım gereksinimleri açıklanmaktadır.

### WSUS Sunucusunun Yazılım Gereksinimleri

-   Aşağıdaki desteklenen işletim sistemlerinden biri yüklü olmalıdır:
    -   Windows Server 2008 R2
    -   Windows Server 2008 SP1 veya sonraki sürümleri
 
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Warning(WS.10).gif" />Uyarı</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Windows Server 2008 R2'ye yükseltmeden önce Windows Server 2008 üzerinde WSUS 3.0 SP2 yüklüyse, Windows Server 2008 R2'ye yükseltme işlemi başarısız olur. Daha fazla bilgi için, <a href="#bkmk_knownissues">Bilinen Sorunlar</a> bölümüne bakın.
        </td>
        </tr>
        </tbody>
        </table>
 

    -   Windows Server 2003 SP1 veya sonraki sürümleri
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Windows Small Business Server için başka önkoşullar da bulunmaktadır. Daha fazla bilgi için “Windows Small Business Server Önkoşulları” bölümüne bakın.
-   Internet Information Services (IIS) 6.0 veya sonraki sürümleri
-   Microsoft .NET Framework 2.0 veya sonraki sürümleri
-   Aşağıdaki desteklenen veritabanlarından biri yüklü olmalıdır:
    -   Microsoft SQL Server 2008 Standard veya Enterprise Edition
    -   Microsoft SQL Server 2005 SP3 veya sonraki sürümleri
    -   Windows İç Veritabanı

    SQL Server'ın desteklenen sürümlerinden biri yüklü değilse, WSUS 3.0 SP2 Kurulum Sihirbazı, Windows İç Veritabanı'nı yükler.
-   Microsoft Yönetim Konsolu 3.0
-   Microsoft Report Viewer Redistributable 2008

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Önemli</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 R2 için WSUS 3.0 SP2 gerekir. Windows Server 2008 R2'yi yüklerseniz, WSUS 3.0 SP2'yi yüklemelisiniz. Windows Server 2008 R2 üzerine WSUS 3.0 SP1 yüklemeyin.

WSUS 3.0 SP2'nin uzak SQL yapılandırmasındaki ön uç sunucusunda Terminal Hizmetleri ile birlikte kullanılması desteklenmez.
</td>
</tr>
</tbody>
</table>
 

### WSUS Yönetim Konsolunun Yazılım Gereksinimleri

-   Aşağıdaki desteklenen işletim sistemlerinden biri: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 SP2 veya sonraki sürümleri, Windows Small Business Server 2008 veya Windows Small Business Server 2003, Windows Vista veya Windows XP SP2
-   Microsoft .NET Framework 2.0 veya sonraki sürümleri
-   Microsoft Yönetim Konsolu 3.0
-   Microsoft Report Viewer Redistributable 2008

### WSUS Sunucusunun En Düşük Donanım Gereksinimleri

Aşağıdaki liste, temel sunucu yüklemesi için en düşük donanım gereksinimlerini içermektedir. Desteklenen donanım yapılandırmalarının kapsamlı bir listesi için [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) adresindeki WSUS 3.0 SP2 Dağıtım Kılavuzu'na başvurun.

-   Hem sistem bölümü hem de WSUS 3.0 SP2'yi yüklediğiniz bölüm, NTFS dosya sistemiyle biçimlendirilmiş olmalıdır.
-   Sistem bölümünde en az 1 GB boş alan olmalıdır.
-   Veritabanı dosyalarının depolanacağı birimde en az 2 GB boş alan olmalıdır.
-   İçeriğin depolanacağı birimde en az 20 GB boş alan bulunması gerekir; 30 GB boş alan bulunması önerilir.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Önemli</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">WSUS 3.0 SP2, sıkıştırılmış sürücülere yüklenemez.
</td>
</tr>
</tbody>
</table>
 

WSUS Sunucusu için Yapılandırma Önkoşulları ve En İyi Uygulama Önerileri
------------------------------------------------------------------------

WSUS 3.0 SP2'yi yüklemeden önce bu bölümdeki ilgili görevleri tamamladığınızdan emin olun.

### IIS

-   Sunucu Yöneticisi Web Sunucusu (IIS) Rol Hizmetleri sayfasında tüm gerekli özellikleri, varsayılan IIS rol hizmetlerini ve şu rol hizmetlerini yükleyin: **ASP.NET**, **Windows Kimlik Doğrulaması**, **Dinamik İçerik Sıkıştırma** ve **IIS 6 Yönetim Uyumluluğu**.
-   IIS eğer IIS 5.0 yalıtım modunda çalışıyorsa yükleme başarısız olur. WSUS 3.0 SP2'yi yüklemeden önce IIS 5.0 yalıtım modunu devre dışı bırakın.
-   Herhangi bir IIS bileşeni 64-bit bir platforma 32-bit uyumluluk modunda yüklenmişse WSUS 3.0 SP2 yüklemesi başarısız olabilir. 64-bit platformlarda tüm IIS bileşenleri yerel modda yüklenmiş olmalıdır.

### Proxy Sunucular

WSUS 3.0 SP2 bir proxy sunucunun yalnızca HTTP desteği sağlamasına izin verir. En iyi uygulama olarak, WSUS sunucusunu Yapılandırma Sihirbazı veya Yönetim Konsolu aracılığıyla yapılandırmadan önce komut satırını kullanarak (**wsusutil configuresslproxy**), HTTPS çalıştırılan ikinci bir proxy sunucu yapılandırın.

### 80 Numaralı Bağlantı Noktasından Çalıştırılan Web Siteleri

80 numaralı bağlantı noktasından çalıştırılan iki veya daha fazla Web siteniz varsa (örneğin, Windows SharePoint Services), WSUS yüklemeden önce bu Web sitelerinin biri dışında tümünü silin. Bunu yapmazsanız, sunucunun istemcileri kendi kendini güncelleştiremez.

### Virüsten Koruma Programları

WSUS 3.0 SP2'yi yüklerken, yüklemeyi başarıyla gerçekleştirebilmeniz için virüsten koruma programlarını devre dışı bırakmanız gerekebilir. Virüsten koruma yazılımını devre dışı bırakın ve WSUS'yi yüklemeden önce bilgisayarı yeniden başlatın. Bilgisayarın yeniden başlatılması, yükleme işleminin dosyalara erişmesi gerektiğinde dosyaların kilitli olmasını önler. Yükleme işlemini tamamladıktan sonra virüsten koruma yazılımınızı yeniden etkinleştirdiğinizden emin olun. Virüsten koruma yazılımınız ve sürümüyle ilgili tam devre dışı bırakma ve etkinleştirme adımlarını öğrenmek için virüsten koruma yazılımınızın üreticisinin Web sitesini ziyaret edin.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Caution(WS.10).gif" />Dikkat</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Bu geçici çözüm, bilgisayarınızın veya ağınızın kötü amaçlı kullanıcılar veya virüsler gibi kötü amaçlı yazılımlar tarafından gerçekleştirilecek saldırılara karşı daha savunmasız kalmasına neden olabilir. Bu geçici çözümü önermiyoruz, ancak gerekli olduğunu düşünürseniz kullanabilmeniz amacıyla bu bilgileri sağlıyoruz. Bu geçici çözümü kullanmak kendi sorumluluğunuzdadır.

Virüsten koruma yazılımları, bilgisayarınızı virüslere karşı korumanıza yardımcı olur. Virüsten koruma programınızın devre dışı bırakıldığı sırada güvenmediğiniz kaynaklardaki dosyaları karşıdan yüklemeyin ve açmayın, güvenmediğiniz Web sitelerini ziyaret etmeyin ve e-posta eklerini açmayın.
</td>
</tr>
</tbody>
</table>
 

### SQL Server'daki İç İçe Tetikleyiciler Seçeneği

Windows Server Update Services veri deposu olarak bir SQL Server veritabanı kullanmayı planlıyorsanız, WSUS yöneticisi WSUS 3.0 SP2'yi yüklemeden önce, SQL Server yöneticisinin sunucuda iç içe tetikleyiciler seçeneğinin açık olduğunu doğrulaması gerekir. İç içe tetikleyiciler seçeneği varsayılan olarak açıktır, ancak bir SQL Server yöneticisi tarafından kapatılabilir. WSUS 3.0 SP2 Kurulumu, veritabanına özgü bir seçenek olan RECURSIVE\_TRIGGERS seçeneğini açar. Ancak WSUS 3.0 SP2 Kurulumu, sunucu genelinde bir seçenek olan iç içe tetikleyiciler seçeneğini açmaz.

### Uzak SQL Sınırlamaları ve Gereksinimleri

WSUS 3.0 SP2, SQL Server yazılımının uyumlu bir sürümünün, WSUS 3.0 SP2 uygulamasının çalıştırıldığı bilgisayardan ayrı bir bilgisayarda çalıştırılmasını destekler. Uzak SQL yüklemesi için aşağıdaki gereksinimler geçerlidir.

-   Uzak SQL çiftinin arka ucunda etki alanı denetleyicisi olarak yapılandırılmış bir sunucuyu kullanamazsınız.
-   Uzak SQL yüklemesinin ön uç sunucusu olacak bilgisayarda Terminal Hizmetleri çalıştıramazsınız.
-   Hem ön uç bilgisayar hem de arka uç bilgisayar bir Active Directory etki alanına katılmış olmalıdır. Ön uç ve arka uç bilgisayarlar farklı etki alanlarındaysa, WSUS Kurulumu'nu çalıştırmadan önce etki alanları arasında bir güven ilişkisi oluşturun.
-   Uzak SQL yapılandırmasında WSUS 2.0 yüklemeniz zaten varsa ve WSUS 3.0 SP2'ye yükseltmek istiyorsanız, WSUS'yi yüklemeden önce şunları yapın:
    1.  WSUS 2.0'ı kaldırın (Denetim Masası'ndaki **Program Ekle veya Kaldır**'ı kullanarak) ve bu arada varolan veritabanının korunduğundan emin olun.
    2.  SQL Server 2005 SP2 veya SQL Server 2008 yükleyin ve varolan veritabanını yükseltin.

### WSUS 3.0 SP2 Kurulumu sırasında IIS yeniden başlatılır

WSUS 3.0 SP2 kurulumu bildirimde bulunmaksızın IIS'yi yeniden başlatır, bu da kuruluşunuzda varolan Web sitelerini etkileyebilir. En iyi uygulama olarak, etkilenen tarafları bu yükleme öncesinde bilgilendirin. IIS çalışmıyorsa, WSUS 3.0 SP2 kurulumu sırasında IIS başlatılır.

Windows Small Business Server Önkoşulları
-----------------------------------------

Windows Small Business Server üzerinde WSUS 3.0 SP2 yüklüyorsanız aşağıdaki önkoşullar geçerlidir.

### IIS Sanal Kökü Belirli IP Adresleri veya Etki Alanı Adlarıyla Kısıtlanmışsa

Bazı Windows Small Business Server yüklemelerinde, varsayılan IIS Web sitesi **IP adresi ve etki alanı adı kısıtlamaları** kullanmak üzere yapılandırılmış olabilir. Bu durumda, sunucudaki Windows Update İstemcisi kendini güncelleştiremeyebilir. WSUS 3.0 SP2'yi yüklemeden önce kısıtlamayı kaldırın.

### ISA Proxy Sunucu Kullanıyorsanız

-   Windows Small Business Server, Internet'e erişmek için ISA proxy sunucu kullanıyorsa, **Ayarlar** kullanıcı arabirimine (UI) **proxy sunucu ayarları, proxy sunucu adı, bağlantı noktası** yazın.
-   ISA, Windows Kimlik Doğrulaması kullanıyorsa, proxy sunucu kimlik bilgilerini *ETKİALANI*\\*kullanıcı* biçiminde yazın. Kullanıcı, Internet Users grubunun üyesi olmalıdır.

### Ağınıza Bir Alt Ağ Eklediyseniz ve Windows Small Business Server Sihirbazlarını Kullanmadıysanız

WSUS sunucusu kurulum işlemi sunucuya iki IIS sanal kökü yükler: SelfUpdate ve ClientWebService. Kurulum ayrıca, varsayılan Web sitesinin (80 numaralı bağlantı noktasında) kök dizinine, istemci bilgisayarların varsayılan Web sitesi üzerinden kendi kendilerini güncelleştirmelerini sağlayan bazı dosyalar yerleştirir. Varsayılan olarak, varsayılan Web sitesi localhost veya sunucuya iliştirilmiş belirli alt ağlar dışındaki tüm IP adreslerinin erişimini reddedecek şekilde yapılandırılır. Bu nedenle, localhost üzerinde veya bu belirli alt ağlar üzerinde olmayan istemci bilgisayarlar kendi kendini güncelleştiremez. Microsoft Windows Small Business Server sihirbazlarını kullanmadan ağınıza bir alt ağ eklediyseniz şu yordamı gerçekleştirin:

1.  Sunucu Yönetimi'nde, **Gelişmiş Yönetim**'i genişletin, **Internet Information Services**'ı genişletin, **Web Siteleri**'ni genişletin, **Varsayılan Web Sitesi**'ni genişletin, **Selfupdate** sanal dizinini sağ tıklatın ve sonra **Özellikler**'i tıklatın.
2.  **Dizin Güvenliği**'ni tıklatın.
3.  **IP adresi ve etki alanı adı kısıtlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim Ver**'i tıklatın.
4.  **Tamam**'ı tıklatın, **ClientWebService** sanal dizinini sağ tıklatın ve sonra **Özellikler**'i tıklatın.
5.  **Dizin Güvenliği**'ni tıklatın.
6.  **IP adresi ve etki alanı adı kısıtlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim Ver**'i tıklatın.

WSUS 3.0 SP2 Uzak Konsolu Yüklemesi için Sistem Gereksinimleri
--------------------------------------------------------------

WSUS 3.0 SP2 Uzak Konsolu aşağıdaki işletim sistemlerinden herhangi birine yüklenebilir:

-   Windows Server 2008 R2, Windows Server 2008 SP1 veya sonraki sürümleri, Windows Server 2003 SP2 veya sonraki sürümleri, Windows Small Business Server 2003, Windows Small Business Server 2005 veya Windows Small Business Server 2008, Windows Vista veya Windows XP Professional SP3 veya sonraki sürümleri.

WSUS İstemci Yüklemesi için Sistem Gereksinimleri
-------------------------------------------------

WSUS istemci yazılımı olan Otomatik Güncelleştirmeler aşağıdaki işletim sistemlerinden herhangi birine yüklenebilir:

-   Windows Server 2008 R2, Windows Server 2008 SP1 veya sonraki sürümleri, Windows Server 2003 SP2 veya sonraki sürümleri, Windows Small Business Server 2003, Windows Small Business Server 2005 veya Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional SP1, Windows XP Professional SP2, Windows XP Professional SP3 veya sonraki sürümleri, Windows 2000 SP4 veya Windows 7 istemcisi.

Yükseltme Gereksinimleri ve Öneriler
------------------------------------

WSUS'nin aşağıdaki sürümleri WSUS 3.0 SP2'ye yükseltilebilir ve önceki sürümün kaldırılması gerekmez:

-   WSUS 2.0, 2.0 SP1, 3.0 ve 3.0 SP1.

WSUS 1.0 sürümünden WSUS 3.0 SP2 sürümüne yükseltme işlemleri desteklenmez. WSUS 3.0 SP2'yi yüklemeden önce Software Update Services (SUS) 1.0 sürümünü kaldırın.

Windows Server 2008 R2 için WSUS 3.0 SP2 gerekir. Windows Server 2008 R2'yi yüklerseniz, WSUS 3.0 SP2'yi yüklemelisiniz. Windows Server 2008 R2 üzerine WSUS 3.0 SP1'i yüklemeyin.

#### WSUS 3.0 SP2'ye Yükseltmeden Önce

1.  Olay günlüklerindeki son hataları, akış aşağı sunucularla akış yukarı sunucular arasındaki eşitleme sorunlarını ve istemci bildirim sorunlarını denetleyin. Yükseltme işleminden önce bu sorunları giderin.

2.  İsteğe bağlı olarak, WSUS veritabanı için doğru dizin oluşturulduğundan emin olmak üzere DBCC CHECKDB deyimini çalıştırabilirsiniz. DBCC CHECKDB hakkında daha fazla bilgi için, [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) konusuna bakın.

3.  WSUS veritabanını yedekleyin. WSUS 3.0 SP2 kurulumu yeni veritabanını *sürücü*\\WSUS olan varsayılan dizine ekler (burada *sürücü*, en çok boş alan bulunan yerel NTFS sürücüsüdür). Bu dizinde zaten bir veritabanı yedeği varsa, bu yedeğin üzerine yazılabilir. En iyi uygulama olarak, WSUS 3.0 SP2'ye yükseltmeden önce WSUS'nin geçerli sürümünün veritabanı yedeğini farklı bir konuma kaydedin.

4.  WSUS tarafından kullanılan bağlantı noktasını el ile değiştirdiyseniz (yani, Wsusutil yardımcı programını kullanmadıysanız) ve SUS 1.0 ya da WSUS 2.0 kullanıyorsanız, SUS 1.0'ı veya WSUS 2.0 64-bit sürümünü kaldırmadan önce varsayılan Web sitesini başlatın.

5.  Varolan bir WSUS veritabanına açık bağlantılar varsa (örneğin, SQL Server Management Studio açıksa), yükleme işlemi başarısız olabilir. WSUS 3.0 SP2'yi yüklemeden önce tüm bağlantıları kapatın.

### Başarısız Olan Bir Yükseltme İşleminden Kurtarma

WSUS'nin önceki bir sürümünden WSUS 3.0 SP2'ye yükseltiyorsanız ve (desteklenmeyen şekilde SUS 1.0'dan yükseltme girişimi dışındaki herhangi bir nedenle) yükseltme işlemi başarısız olursa aşağıdaki görevleri gerçekleştirin.

1.  WSUS'nin önceki sürümünü yeniden yükleyin.
2.  Yükseltmeyi denemeden önce, veritabanını yedekten geri yükleyin. Önceki bir yüklemeden bir WSUS 3.0 SP2 veritabanı varsa yükseltme işlemini başarıyla tamamlayamazsınız. WSUS çoğu durumda otomatik olarak bir yedek oluşturur. Bunun konumu için WSUSSetup.log dosyasına bakın.
3.  Günlükleri inceleyerek hatanın nedenini belirleyin ve sorunu giderin.
4.  WSUS 3.0 SP2'yi yükleyin.

### WSUS 3.0 SP2'ye yükseltmeden önce bilgisayar adının değiştirilmesi yükseltmenin başarısız olmasına yol açabilir

WSUS 2.0'ı yükledikten sonra ve WSUS 3.0 SP2'ye yükseltmeden önce bilgisayar adını değiştirirseniz, yükseltme başarısız olabilir.

ASPNET ve WSUS Administrators gruplarını kaldırıp yeniden eklemek için aşağıdaki komut dosyasını kullanın. Daha sonra, yükseltmeyi yeniden çalıştırın.

        ```

### WSUS 2.0 üzerinde MSDE'den SQL Server 2008'e veya SQL Server 2005'e geçiş yaptıysanız bir kayıt defteri değerini değiştirmelisiniz

WSUS 2.0 yüklemeniz varsa ve SQL Server 2008'e ya da SQL Server 2005'e geçiş yaptıysanız, 1 olan **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** değerini 0 olarak değiştirmelisiniz. WSUS 3.0 SP2'ye yükseltmeden önce bunu yapmazsanız, yükseltme başarısız olabilir.

### WSUS 3.0 SP2'yi kaldırır ve günlük dosyalarını geride bırakırsanız, yeniden yükleme sonrasında bu dosyalar uygun izinlere sahip olamayabilir

WSUS 3.0 SP2'yi kaldırırsanız, yüklemeyle ilgili günlük dosyalarını saklama seçeneğiniz vardır. WSUS 3.0 SP2'yi yeniden yüklediğinizde, eski günlük dosyaları izinlerini kaybedebilir (genellikle yalnızca WSUS Administrators için). En iyi uygulama olarak, yüklemenin ardından bu günlük dosyalarının izinlerini doğrulayın.

### WSUS 2.0 istemcileri için "Uygun Değil" durum bilgisine sahip güncelleştirmeler varsa, WSUS 3.0 SP2'ye yükseltildikten sonra bu güncelleştirmeler kısa bir süreliğine "Bilinmiyor" olarak görünür

Varolan bir WSUS 2.0 sunucusunda **Uygun Değil** güncelleştirmelerinin yer aldığı istemciler varsa, WSUS 3.0 SP2'ye yükseltildikten sonra bu güncelleştirmelerin durum bilgileri kısa bir süreliğine **Bilinmiyor** olarak listelenebilir. İstemcinin bir sonraki tarama işleminin ardından güncelleştirme durumu yeniden **Uygun Değil** olur.

WSUS 3.0 SP2'yi Yükleme
-----------------------

[http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) adresindeki WSUS Adım Adım Yükleme Kılavuzu, Windows Sunucu Yöneticisi veya WSUSSetup.exe dosyası kullanılarak WSUS 3.0 SP2 yüklenmesine yönelik ayrıntılı yönergeler sunar.

WSUS'yi yükleme ve kullanma ile ilgili tüm bilgiler için bkz:

WSUS Dağıtım Kılavuzu, [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832).

WSUS İşlemler Kılavuzu, [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838).

Katılımsız WSUS 3.0 SP2 Yüklemeleri için Kurulum Komut Satırı Parametreleri
---------------------------------------------------------------------------

WSUS komut satırı kurulum programını kullanarak katılımsız WSUS 3.0 SP2 yüklemeleri gerçekleştirebilirsiniz. Bu tabloda WSUS 3.0 SP2 kurulumu için komut satırı parametreleri gösterilmiştir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Seçenek</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Sessiz yükleme gerçekleştirir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Kaldırma işlemi gerçekleştirir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Önkoşul denetimi. Sistemi inceler ve eksik önkoşulları bildirir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Komut satırı parametrelerini ve bunların açıklamalarını görüntüler.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">WSUS'nin önceki sürümünden yükseltir. (SUS 1.0'dan yükseltme işlemleri desteklenmez.) Bu seçenekle kullanılabilen tek geçerli parametre /q (sessiz yükleme) seçeneğidir. Bu seçenekle kullanılabilen tek geçerli özellik DEFAULT_WEBSITE özelliğidir.</td>
</tr>
</tbody>
</table>
  
Bu tabloda WSUS 3.0 SP2 komut satırı özellikleri gösterilmiştir.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Özellik</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0=içerik yerel olarak barındırılıyor, 1=içerik Microsoft Update'te barındırılıyor</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">İçerik dizininin yolu. Varsayılan olarak <em>WSUSYüklemeSürücüsü\WSUS\WSUSİçeriği</em> kullanılır; burada <em>WSUSYüklemeSürücüsü</em>, en çok boş alan bulunan yerel sürücüdür.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Windows İç Veritabanı veri dizininin yoludur.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Ad <em>SunucuAdı</em>\<em>SQLÖrneğiAdı</em> biçiminde olmalıdır. Veritabanı örneği yerel makinede bulunuyorsa, %COMPUTERNAME% ortam değişkenini kullanın. Mevcut bir örnek yoksa, varsayılan değer %COMPUTERNAME%\WSUS şeklindedir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0=bağlantı noktası 8530, 1=bağlantı noktası 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Günlük dosyasının yolu ve dosya adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0=WSUS sunucusunu yükle, 1=yalnızca konsolu yükle</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0=envanter özelliklerini yükleme, 1=envanter özelliklerini yükle</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0=veritabanını koru, 1=veritabanını kaldır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0=içerik dosyalarını koru, 1=içerik dosyalarını kaldır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0=günlük dosyalarını koru, 1=günlük dosyalarını kaldır (/u yükleme anahtarıyla kullanılır)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=geçerli veritabanını kullan, 1=veritabanı oluştur</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Windows Installer ilerleme iletilerini döndürmek için pencere tanıtıcısı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=Microsoft Update Geliştirme Programı'na katıl, 0=Microsoft Update Geliştirme Programı'na katılma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=içerik konumunu veritabanına yazma, 0=içerik konumunu veritabanına yaz (NLB için)</td>
</tr>
</tbody>
</table>
  
### Örnek Kullanım
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (bağlantı noktası 8530'u kullanarak sessiz modda yükle) WSUSSetup.exe /q /u (WSUS'yi kaldır)  
```
 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939886.Important(WS.10).gif" />Önemli</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">WSUS 3.0 SP2'yi sessiz modda (/q) yüklerseniz ve bilgisayarda tüm önkoşullar yüklü değilse, yükleme işlemi WSUSPreReqCheck.xml adlı bir dosya oluşturur ve dosyayı %TEMP% dizinine kaydeder.
</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_KnownIssues"></span>
Bilinen Sorunlar
----------------

-   WSUS Yükleme Sihirbazı başarıyla tamamlandıktan sonra, kullanıcıya **Son**'u tıklatması bildirilir. Nadiren de olsa, şu hata iletisini içeren bir iletişim kutusu görüntülenir: “**Sunucuyla iletişimde hata oluştu ve bu sihirbazın kapatılması gerekiyor. WSUS Sunucu Yapılandırma Sihirbazı'nı WSUS konsolunun Seçenekler sayfasından yeniden başlatabilirsiniz.**” Yükleme seçimlerinizin kaydedildiğinden emin olmak için, WSUS yönetim konsolundaki **Seçenekler** sayfasını açın ve her bir bölümdeki ayarları onaylayın.
-   **Windows Update Aracısı (WUA) istemcisinin yerelleştirilmiş sürümleri WSUS 3.0 SP2 sürümünden daha ileri bir tarihte yayımlanacaktır**. Bunun nedeni, Windows 7 yerelleştirme zamanlamasına bağlı olmasıdır. WSUS 3.0 SP2'nin yayımlanması ile WUA istemcisinin yerelleştirilmiş sürümünün yayımlanması arasındaki sürede, WUA istemcisi yalnızca beş dili destekler (İngilizce, Almanca, Fransızca, İspanyolca ve Japonca).
-   **Bu SP2 sürümünde kullanıma sunulan yeni Güncelleştirme ve Bilgisayar Durumu raporları, akış aşağı WSUS 3.0 SP1 sunucularının bir WSUS 3.0 SP2 sunucusundan yönetildiği bir ortamda çalışmaz**. Yeni raporlar bir SP1 sunucusu için çalıştırılırsa şu hata iletisi görüntülenir: “Rapor oluşturulurken hata oluştu. Raporu yeniden çalıştırmayı deneyin veya sorun devam ederse ağ yöneticinize başvurun.” Rapor yeniden çalıştırılırsa sorun giderilmez ve bu sorun ağ hizmetleri ile ilgili değildir. Yeni raporlar SP1'de bulunmayan API işlevlerini kullanır; ancak SP2 Yönetim Konsolu, bir SP1 sunucusunu yönetirken yeni raporları engellemez.
-   **SSL bir sertifika adı olmadan yapılandırıldığında WSUS 3.0 SP2'ye yükseltme işlemi başarısız oluyor**. SSL yapılandırılıyorsa sertifika adı gereklidir.
-   **Windows Server 2008 üzerine yüklenen ve Windows İç Veritabanı çalıştıran WSUS 3.0 SP2, Windows Server 2008 R2**'ye yükseltme işlemini engeller. Windows Server 2008 R2'ye yükseltme işlemine devam etmeden önce, Windows İç Veritabanı özelliğini kapatmanızı bildiren bir Uyumluluk Raporu hata iletisi görüntülenir. Windows Server 2008 R2'ye yükseltme işleminin devam edebilmesi için önce Windows İç Veritabanı özelliğininin yükseltilmesi gerekir. Yönergeler ve Windows İç Veritabanı özelliğini yükseltme hakkında daha fazla bilgi için bkz. [Windows İç Veritabanı için en son hizmet paketini edinme](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104).

Telif Hakkı Bildirimi
---------------------

URL ve diğer Internet Web sitesi başvuruları da dahil olmak üzere işbu belgedeki bilgiler önceden haber verilmeksizin değiştirilebilir. Aksi belirtilmedikçe, buradaki örneklerde adı geçen şirketler, kuruluşlar, ürünler, etki alanı adları, e-posta adresleri, logolar, kişiler, yerler ve olaylar gerçek dışıdır. Herhangi bir gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla bir ilişki amaçlanmamaktadır ve bunun amaçlandığı sonucuna varılamaz. İlgili tüm telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakkı kapsamındaki haklara hiçbir sınırlama getirilmeksizin, bu belgenin hiçbir bölümü, Microsoft Corporation'dan yazılı izin alınmadan yeniden üretilemez, yeniden kullanılabileceği bir sisteme yerleştirilemez veya böyle bir sistemde saklanamaz veya herhangi bir biçimde veya herhangi bir araç (elektronik, mekanik, fotokopi, kayıt veya diğer) kullanılarak veya herhangi bir amaçla iletilemez.

Microsoft'un bu belgenin içeriğini kapsayan patentleri veya patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından sağlanan herhangi bir yazılı lisans sözleşmesinde açıkça belirtilmedikçe, bu belgenin size sağlanmış olması bu patentler, ticari markalar, telif hakları ve diğer fikri mülkiyet hakları için size herhangi bir lisans da verilmiş olduğu anlamına gelmez.

© 2009 Microsoft Corporation. Tüm hakları saklıdır.

Microsoft, Active Directory, ActiveX, Authenticode, Excel, InfoPath, Internet Explorer, MSDN, Outlook, Visual Studio, Win32, Windows, Windows Server ve Windows Vista, Microsoft şirketler grubunun ticari markalarıdır.

Diğer tüm ticari markalar ilgili sahiplerine aittir.
