---
TOCTitle: 'Microsoft Windows Server Update Services 3.0 Sürüm Notları'
Title: 'Microsoft Windows Server Update Services 3.0 Sürüm Notları'
ms:assetid: '94d1385f-4872-4c29-8822-3a4ec5e45ae4'
ms:contentKeyID: 18155266
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708491(v=WS.10)'
---

Microsoft Windows Server Update Services 3.0 Sürüm Notları
==========================================================

Bu sürüm notları, Microsoft® Windows® Server Update Services (WSUS) 3.0 ürününü etkileyen bilinen konuları anlatır ve uygulamayı yüklemeyle ilgili önerileri ve gereksinimleri içerir. Bu notlar aşağıdaki bölümleri içerir:

-   WSUS 3.0 sunucu yüklemesi için sistem gereksinimleri
-   WSUS 3.0 sunucu yüklemesi için yapılandırma gereksinimleri
-   WSUS 3.0 uzak konsol yüklemesi için sistem gereksinimleri
-   WSUS 3.0 uzak konsol yüklemesi için yapılandırma gereksinimleri
-   İstemci yüklemesi için sistem gereksinimleri
-   WSUS 3.0 sunucu yüklemesi için yazılım gereksinimleri
-   WSUS 3.0 sunucu yüklemesi için en az disk alanı gereksinimleri
-   WSUS 3.0 yükseltme gereksinimleri
-   Kurulum komut satırı parametreleri
-   Kurulum ve yükseltme sorunları
-   Bilinen sorunlar
-   Windows Server® 2008 üzerinde WSUS 3.0
-   Windows Small Business Server 2003 Üzerinde WSUS 3.0

| ![](/security-updates/images/Cc708491.note(WS.10).gif)Not                                                                                                                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu belgenin karşıdan yüklenebilir bir kopyası [Microsoft Yükleme Merkezi'nde](http://go.microsoft.com/fwlink/?linkid=71220) ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)) bulunabilir. |

Önemli yapılandırma sorunu: Yapılandırma sihirbazında proxy sunucu parolasının üzerine yazmanız gereklidir
----------------------------------------------------------------------------------------------------------

Kullanıcı adı/parola kimlik doğrulaması gerektiren bir proxy sunucu kullanıyorsanız, WSUS Sunucu Yapılandırma Sihirbazı'nı çalıştırırken proxy sunucu parolasının üzerine yazmazsanız, WSUS sunucusu güncelleştirmelerin eşitlenmesini yapamayabilir. Kurulumun sonunda yapılandırma sihirbazı otomatik olarak başlatıldığı için, bu sorun WSUS'nin eski bir sürümünden WSUS 3.0'a yükseltme yaptıktan sonra eşitleme hatalarına neden olabilir.

Yükseltme yaptıktan sonra yapılandırma sihirbazını iptal ederek veya yapılandırma sihirbazı çalıştığında doğru proxy parolasını yeniden girerek bu sorundan kaçınabilirsiniz. Oluştuktan sonra bu sorunu gidermek için, **Seçenekler** sayfasında, **Güncelleştirme Kaynağı ve Proxy Sunucu**'ya gidin ve proxy parolasını yeniden girin ve ayarı kaydedin.

WSUS 3.0 sunucu yüklemesi için sistem gereksinimleri
----------------------------------------------------

#### WSUS 3.0 sunucusu, Windows Server 2003 Service Pack 1 ve Windows Server 2008 üzerinde desteklenir

WSUS 3.0 sunucusu, Windows Server 2003 Service Pack 1 ve Windows Server 2008 üzerinde desteklenir.

#### WSUS 3.0 sunucuları için Windows 2000 Server desteklenmez

Microsoft Windows® 2000 Server, WSUS 3.0 sunucuları için desteklenen bir işletim sistemi değildir.

#### WSUS 3.0, Terminal Hizmetleri'ni çalıştıran sunucularda desteklenmez

WSUS 3.0, Terminal Hizmetleri çalıştıran sunucularda hala çalışıyor olsa da böyle yapılması desteklenmez ve önerilmez. WSUS 3.0, uzak SQL Server uygulamaları kullanılan yapılandırmalardaki Terminal Hizmetleri çalıştıran sunucuda çalışmaz. Bir Terminal Hizmetleri lisans sunucusunda tüm uzak özel eylemler (yükleme dahil) sistem hesabı olarak çalıştırılacağından ve sunucunun sistem hesabı uzak SQL Server'da izinlere sahip olmayabileceğinden, yükleme başarısız olabilir.

WSUS 3.0 sunucu yüklemesi için yapılandırma gereksinimleri
----------------------------------------------------------

#### IIS yüklenmiş olmalıdır

Microsoft Windows Server Update Services 3.0, Microsoft Windows Server 2003 veya Windows Server 2008 üzerine varsayılan olarak yüklenmeyen Internet Information Services (IIS) ürününü gerektirir. IIS olmadan WSUS 3.0'ı yüklemeye çalışırsanız, Windows Server Update Services Kurulumu, IIS'nin yüklü olmadığını belirten bir hata iletisi görüntüler.

#### IIS, IIS 5.0 yalıtım modunu çalıştırıyorsa yükleme başarısız olur

Sunucuyu Windows 2000 Server'dan Windows Server 2003'e yükselttiyseniz IIS, IIS 5.0 uyumluluk modunda çalışıyor olabilir. IIS Yöneticisi'nde IIS 5.0 yalıtım modunu etkinleştirmek mümkündür. Bu yüklemenin başarısız olmasına neden olur. WSUS 3.0 yüklemeden önce IIS 5.0 yalıtım modunu devreden çıkarmanız gerekecektir.

#### Herhangi bir IIS bileşeni 64-bit bir platforma 32-bit uyumluluk modunda yüklenmişse WSUS 3.0 yüklemesi başarısız olabilir

64-bit platformlarda tüm IIS bileşenleri yerel modda yüklenmiş olmalıdır. Herhangi bir IIS bileşeni 32-bit uyumluluk modundaysa yükleme başarısız olabilir.

#### Proxy sunucular hem HTTP'yi hem de HTTPS'yi desteklemelidir

Kök WSUS sunucusunu yapılandırdığınızda (WSUS sunucusu doğrudan Microsoft Update'ten güncelleştirilir) ve WSUS sunucusu ile Internet arasında bir proxy sunucu olacaksa, proxy sunucu hem HTTP'yi hem de HTTPS'yi desteklemelidir.

#### Bağlantı noktası 80 üzerinde iki veya daha fazla Web sitesi zaten çalışıyorsa, WSUS yüklemeden önce, bu sitelerin biri dışındaki tümünü silin

Bağlantı noktası 80 üzerinde iki veya daha fazla Web sitesi (örneğin, Windows® SharePoint® Services) zaten çalıştırıyorsanız, WSUS yüklemeden önce biri dışındaki tümünü silmeniz gereklidir. Bunu yapmazsanız sunucunuzun istemcileri kendilerini güncelleştiremeyebilir.

#### WSUS 3.0'ı yüklerken virüsten koruma programlarını devre dışı bırakmanız gerekebilir

WSUS 3.0'ı yüklerken, yüklemeyi başarıyla gerçekleştirebilmeniz için virüsten koruma programlarını devre dışı bırakmanız gerekebilir. Virüsten koruma programını devre dışı bıraktıktan sonra, WSUS yüklemesini başlatmadan önce bilgisayarı yeniden başlatın. Bilgisayarın yeniden başlatılması, yükleme işleminin dosyalara erişmesi gerektiğinde dosyaların kilitli olmasını önler. Yükleme işlemini tamamladıktan sonra virüsten koruma programınızı yeniden etkinleştirdiğinizden emin olun. Virüsten koruma programınız ve sürümüyle ilgili tam devre dışı bırakma ve etkinleştirme adımlarını öğrenmek için virüsten koruma programınızın üreticisinin Web sitesini ziyaret edin.

| ![](/security-updates/images/Cc708491.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                              |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu geçici çözüm, bilgisayarınızın veya ağınızın kötü niyetli kullanıcılar veya virüsler gibi kötü amaçlı yazılımlar tarafından gerçekleştirilecek saldırılara karşı daha savunmasız kalmasına neden olabilir. Bu geçici çözümü önermiyoruz, ancak gerekli olduğunu düşünürseniz kullanabilmeniz amacıyla bu bilgileri sağlıyoruz. Bu geçici çözümü kullanmak kendi sorumluluğunuzdadır. |

| ![](/security-updates/images/Cc708491.note(WS.10).gif)Not                                                                                                                                                                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Virüsten koruma programları, virüslere karşı bilgisayarınızı korumanıza yardımcı olması için tasarlanmıştır. Virüsten koruma programınızın devre dışı bırakıldığı sırada güvenmediğiniz kaynaklardaki dosyaları karşıdan yüklememeli ve açmamalı, güvenmediğiniz Web sitelerini ziyaret etmemeli ve e-posta eklerini açmamalısınız. |

#### WSUS 3.0, SQL Server'da iç içe tetikleyiciler seçeneğinin açık olmasını gerektirir

İç içe tetikleyiciler seçeneği varsayılan olarak açıktır, ancak bir SQL Server yöneticisi tarafından kapatılabilir.

Windows Server Update Services veri deposu olarak bir SQL Server veritabanı kullanmayı planlıyorsanız, WSUS 3.0 yöneticisi WSUS 3.0'ı yüklemeden ve kurulum sırasında veritabanını belirlemeden önce, SQL Server yöneticisinin sunucuda iç içe tetikleyiciler seçeneğinin açık olduğunu doğrulaması gerekir.

WSUS 3.0 Kurulumu, veritabanına özgü bir seçenek olan RECURSIVE\_TRIGGERS seçeneğini açar, ancak sunucu genelinde bir seçenek olan iç içe tetikleyiciler seçeneğini açmaz.

İç içe tetikleyiciler seçeneğinin açık olup olmadığını görmek için aşağıdakini kullanın:

**sp\_configure 'nested triggers'**

SQL Server'da iç içe tetikleyiciler seçeneğini açmak için, SQL Server çalıştıran bilgisayarda bir toplu iş dosyasından aşağıdakini çalıştırın:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Sunucunuzda SQL Server Management Studio yoksa, SQL komut dosyalarını komut satırından çalıştırmak isteyebilirsiniz. Microsoft SQL Server 2005 Command Line Query Utility'yi [Microsoft Yükleme Merkezi'nden](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728) edinebilirsiniz. Başlamak için, **sqlcmd** komutunu çalıştırın.

Bir Windows İç Veritabanı içinde SQL komut dosyaları çalıştırmak istiyorsanız, aynı yükleme sayfasından SQL Native Client'ı da yüklemeniz gerekir.

#### Uzak SQL sınırlamaları ve gereksinimleri

WSUS 3.0, uygulamanın geri kalanını içeren bilgisayardan ayrı bir bilgisayar üzerinde veritabanı yazılımı çalıştırma konusunda destek sağlar. Uzak bir SQL yüklemesi yapılandırma için bazı gereksinimler vardır

-   Uzak SQL çiftinin son ucu olarak bir etki alanı denetleyicisi olarak yapılandırılmış bir sunucu kullanamazsınız.
-   Uzak SQL yüklemesinin ön ucundaki sunucu olacak bilgisayarda Terminal Server çalıştırmamalısınız.
-   Arka uçtaki bilgisayar Windows Server 2003 çalıştırıyorsa bu bilgisayarda veritabanı yazılımı olarak en az Microsoft SQL Server 2005 Service Pack 1 ( [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143 adresinde bulunabilir) Windows Server® 2008 çalıştırıyorsa SQL Server 2005 Service Pack 2 kullanmanız gereklidir.
-   Hem ön uç hem de arka uç bilgisayarları bir Active Directory etki alanına katılmalıdır, farklı etki alanlarında bulunuyorsa WSUS kurulumunu çalıştırmadan önce etki alanları arasında çapraz etki alanı güveni kurmanız gereklidir.
-   Bir uzak SQL yapılandırmasında WSUS 2.0 yüklemeniz zaten varsa ve WSUS 3.0'a yükseltmek istiyorsanız, arka uç bilgisayarda WSUS 2.0'ı kaldırmalı (Denetim Masası'ndaki **Program Ekle veya Kaldır**'ı kullanarak) ve bu arada varolan veritabanının korunduğundan emin olmalısınız. Ardından, SQL Server 2005 SP1 veya SP2 yüklemeli ve varolan veritabanını yükseltmelisiniz. Son olarak, ön uç bilgisayarında WSUS 3.0'ı yüklemeniz gerekir.

#### Internet Explorer 7'nin belirli ön sürümlerine ek olarak Terminal Hizmetleri yüklü olduğunda, WSUS yüklenemez

Internet Explorer 7'nin belirli aday sürümleri ile birlikte Terminal Hizmetleri varsa, WSUS kurulumu başarısız olacaktır.

WSUS 3.0 uzak konsol yüklemesi için sistem gereksinimleri
---------------------------------------------------------

WSUS 3.0 uzak konsolu aşağıdaki platformlara yüklenebilir:

-   Windows Server 2008
-   Windows Vista®
-   Windows Server 2003 SP1
-   Windows XP SP2

WSUS 3.0 uzak konsol yüklemesi için yapılandırma gereksinimleri
---------------------------------------------------------------

#### Uzaktan yönetim konsolu ve WSUS 3.0 sunucusu arasında geniş bantlı bağlantı kullanmalısınız

Uzaktan yönetim konsoluyla WSUS 3.0 sunucusuna dar bantlı bir WAN bağlantısıyla bağlanırsanız performans sorunları yaşayabilirsiniz. Güncelleştirme ve bilgisayar görünümlerine filtre uygulayarak güncelleştirme sayısını sınırlayabilirsiniz, ancak uzaktan yönetim konsolu ve WSUS 3.0 sunucuları arasında geniş bantlı bağlantı kullanmanız önerilir. Uzak konsolla ilgili performans sorunlarınız varsa, uzaktan yönetim için Terminal Server kullanan sunucuya bağlanmanızı öneririz.

İstemci yüklemesi için sistem gereksinimleri
--------------------------------------------

Otomatik Güncelleştirmeler, WSUS istemci yazılımıdır. Aşağıdaki işletim sistemlerinden herhangi birinde WSUS ile kullanılabilir:

-   Windows Vista
-   Windows Server 2008
-   Microsoft Windows Server 2003, herhangi bir sürümü
-   Microsoft Windows XP Professional SP2
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 veya Windows 2000 Advanced Server with SP4

WSUS 3.0 sunucu yüklemesi için yazılım gereksinimleri
-----------------------------------------------------

Aşağıdaki tabloda Windows Server 2003 SP1 platformları için gerekli yazılımlar gösterilmiştir. Windows Server 2008 için gereken yazılımlar, Windows Server 2008 üzerinde WSUS 3.0 kullanımı ile ilgili bölümde ele alınacaktır.

WSUS 3.0 kurulumunu çalıştırmadan önce WSUS 3.0 sunucusunun bu gereksinimler listesini karşıladığından emin olun. Bu güncelleştirmelerden herhangi biri yükleme tamamlandıktan sonra bilgisayarın yeniden başlatılmasını gerektiriyorsa, WSUS 3.0'ı yüklemeden önce bilgisayarı yeniden başlatmalısınız.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Gereksinim</th>
<th style="border:1px solid black;" >Ayrıntılar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">İşletim sisteminden yükleme.
Bkz: Konu 1: IIS yüklenmiş olmalıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x86)</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=68935) Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x86) sayfasına bakın. 64-bit platformlar için, <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70637) Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x64) sayfasına bakın .</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 için Microsoft Yönetim Konsolu 3.0</td>
<td style="border:1px solid black;">Bu, WSUS 3.0 kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft Yükleme Merkezi'nde</a> (http://go.microsoft.com/fwlink/?LinkId=70412) adresinde bkz. Windows Server 2003 için Microsoft Yönetim Konsolu 3.0 (KB907265) 64 bit platformlar için Microsoft <a href="http://go.microsoft.com/fwlink/?linkid=70638">Yükleme Merkezi'nde</a> (http://go.microsoft.com/fwlink/?LinkId=70638) adresinde Windows Server 2003 x64 Edition için Microsoft Yönetim Konsolu 3.0 (KB907265).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Bu, WSUS 3.0 kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70410) Microsoft Report Viewer Redistributable 2005 sayfasına bakın.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (isteğe bağlı)</td>
<td style="border:1px solid black;">SQL Server'ın uyumlu bir sürümü önceden yüklenmemişse WSUS 3.0 sizin için Windows İç Veritabanı yükleyecek. Tam SQL Server veritabanı kullanmayı planlıyorsanız, Windows Server 2003 üzerinde (en az) SQL Server 2005 SP1 (<a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Yükleme Merkezi</a>'nde bulunan (http://go.microsoft.com/fwlink/?LinkId=66143) veya üzerinde SQL Server 2005 SP2 (<a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Yükleme Merkezi</a>'nde bulunan http://go.microsoft.com/fwlink/?LinkId=84823) Windows Server 2008kullanmanız gereklidir.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc708491.note(WS.10).gif)Not                                                                                                                                                                                                                                   |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 2.0 önceden yüklenmişse ve SQL Server 2000, SQL Server Desktop Engine 2000 veya SQL Server 2005 SP1 (veya Windows Server 2008 üzerinde SQL Server 2005 SP2) herhangi bir SQL Server veritabanı kullanıyorsa, WSUS 3.0 yüklemeWindows® İç Veritabanı programı yükler ve veritabanını buna geçirir. |
  
WSUS 3.0 sunucu yüklemesi için en az disk alanı gereksinimleri  
--------------------------------------------------------------
  
Aşağıda Windows Server Update Services'ı yüklemek için gereken en az disk alanı verilmiştir:
  
-   Sistem bölümünde 1 GB  
-   Veritabanı dosyalarının depolanacağı birimde 2 GB  
-   İçeriğin depolanacağı bölüm için 20 GB
  
| ![](/security-updates/images/Cc708491.Important(WS.10).gif)Önemli                              |  
|-----------------------------------------------------------------------------------------------------------|  
| WSUS 3.0, sıkıştırılmış sürücülere yüklenemez. Seçtiğiniz sürücünün sıkıştırılmış olmamasına dikkat edin. |
  
WSUS 3.0 yükseltme gereksinimleri  
---------------------------------
  
#### WSUS yüklemenizin doğru çalıştığından emin olun ve yükseltme yapmadan önce WSUS veritabanınızı yedekleyin
  
Önceki sürümden WSUS 3.0'a yükseltiyorsanız, geçerli yüklemenizin doğru çalıştığından emin olun ve yükseltme yapmadan önce WSUS veritabanınızı yedekleyin.
  
1.  Olay günlüklerindeki son hataları, akış aşağı ve akış yukarı sunucular arasındaki eşitleme sorunlarını veya rapor vermeyen istemcilerle ilgili sorunları denetleyin. Devam etmeden önce bu sorunların çözüldüğünden emin olun.  
2.  WSUS veritabanının doğru sıralandığından emin olmak için DBCC CHECKDB çalıştırmak isteyebilirsiniz. CHECKDB hakkında daha fazla bilgi için, bkz. [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  WSUS veritabanını yedekleyin.
  
#### Software Update Services 1.0 kaldırılmalıdır
  
Aynı makinede Software Update Services 1.0 yüklüyse WSUS 3.0 yüklemesi başarısız olur. WSUS 3.0'ı yüklemeden önce Software Update Services 1.0'ı kaldırmalısınız.
  
#### WSUS 3.0'ın beta sürümlerinden RTM sürümüne yükseltme desteklenmez, ancak RC sürümünden RTM sürümüne yükseltme yapılmasına izin verilir
  
WSUS 3.0'ın bir beta sürümünü yüklediyseniz, WSUS 3.0'ın RTM sürümünü yüklemeden önce bunu kaldırmanız ve veritabanını silmeniz gerekir. Yalnızca RC türümünden RTM sürümüne yükseltmek mümkündür.
  
#### 64-bit bir işletim sisteminde WSUS 2.0'dan WSUS 3.0'a yükseltme yapılamaz
  
WSUS 2.0 64-bit işletim sistemlerinde desteklenmemektedir. 64-bit sistemlerde WSUS 2.0'dan WSUS 3.0'a yükseltme yapılması mümkün değildir.
  
Kurulum komut satırı parametreleri  
----------------------------------
  
WSUS komut satırı parametrelerini kullanarak katılımsız WSUS 3.0 yüklemeleri gerçekleştirebilirsiniz. Bu tabloda WSUS 3.0 komut satırı parametreleri gösterilmiştir.
  
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
<td style="border:1px solid black;">Sessiz yükleme gerçekleştirin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Ürünü kaldırın. Yüklüyse Windows İç Veritabanı örneğini de kaldırır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Yalnızca önkoşul denetimi. Ürünü yüklemez ancak sistemi inceler ve eksik olan önkoşulları raporlar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Komut satırı parametrelerini ve açıklamalarını görüntüleyin.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">WSUS'nin 2.0 sürümünden yükseltin. Bu seçenekle ilgili tek geçerli parametre /q (sessiz yükleme). Bu seçenek için tek geçerli özellik DEFAULT_WEBSITE değeridir.</td>
</tr>
</tbody>
</table>
  
Bu tabloda WSUS 3.0 komut satırı özellikleri gösterilmiştir.
  
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
<td style="border:1px solid black;">İçerik dizininin yolu. Varsayılan değer <em>WSUSInstallationDrive</em><strong>\WSUS\WSUSContent</strong>, burada <em>WSUSInstallationDrive</em> en fazla boş alanın bulunduğu yerel sürücüdür.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Windows İç Veritabanı veri dizininin yolu.</td>
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
<td style="border:1px solid black;">0=günlük dosyalarını sakla, 1=günlük dosyalarını kaldır (/u yükle anahtarıyla birlikte kullanılan).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0=geçerli veritabanını kullan, 1=veritabanı oluştur</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">MSI ilerleme iletilerini döndürmek için pencere tanıtıcısı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1=Microsoft Update Geliştirme Programı'na katıl, 0=katılma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1=içerik konumunu veritabanına yazma, 0=içerik konumunu veritabanına yaz (NLB için)</td>
</tr>
</tbody>
</table>
  
#### Örnek Kullanım
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](/security-updates/images/Cc708491.Important(WS.10).gif)Önemli                                                                                                        |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0'ı sessiz modda (/q) yüklerseniz ve makinede tüm önkoşullar yüklü değilse, yükleme işlemi WSUSPreReqCheck.xml adlı bir dosya oluşturur ve dosyayı %TEMP% dizinine kaydeder. |
  
Kurulum sorunları  
-----------------
  
#### WSUS 3.0 Kurulumu sırasında IIS yeniden başlatılır
  
WSUS 3.0 Kurulumu bildirimde bulunmaksızın IIS'yi yeniden başlatır, bu da kuruluşunuzda varolan Web sitelerini etkileyebilir. IIS çalışmıyorsa, WSUS 3.0 kurulumu bu işlevi başlatır.
  
#### Varolan bir WSUS veritabanına yönelik açık bağlantılar varsa yükleme başarısız olabilir
  
Varolan bir yüklemeden WSUS 3.0'a yükseltiyorsanız ve hala varolan WSUS veritabanına yönelik açık bağlantılar varsa (örneğin, SQL Server Management Studio açıksa), yükleme işlemi başarısız olabilir. Lütfen tüm bağlantıları kapatın ve WSUS 3.0'ı yeniden yükleyin.
  
#### WSUS kurulumu veritabanı dosyaları için yanlış dizini gösterir
  
WSUS kurulumunda, **Yüklemeye Hazır** ekranı yanlış olarak veritabanının bulunduğu konumun üst dizinini veritabanı konumu olarak bildirir. Örneğin, varsayılan konum %systemdrive%\\WSUS\\UpdateServicesDbFiles olmasına karşın, bu konum hatalı olarak %systemdrive%\\WSUS şeklinde görünür.
  
#### WSUS, Çok Dilde Kullanıcı arabirimi dil paketine sahip ve İngilizce dışında varsayılan dili olan bir makineye yüklenirse, Yardım İngilizce yerine varsayılan dilde görüntülenir
  
WSUS, Çok Dilde Kullanıcı arabirimi dil paketine sahip ve İngilizce dışında varsayılan dili olan bir makineniz varsa, geçerli kullanıcınızın yerel ayarı İngilizce olduğunda da WSUS yükleyebileceksiniz. UI İngilizce olarak görüntülenir ancak Yardım'ın İngilizce'de görüntülenmesini sağlamak için geçici bir çözüm kullanmanız gerekir. İngilizce dilindeki Yardım .chm dosyasını (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) ana belge dizinine (*WSUSInstallDir*\\documentation\\WSUS30Help.chm) kopyalayın. Bu noktada Yardım tüm dillerde doğru olarak görüntülenecektir.
  
Yükseltme sorunları  
-------------------
  
#### WSUS 3.0 RC'den WSUS 3.0 RTM'ye yükseltme WSUS Web sitesine SSL sertifikasının atanmamasına neden olur
  
WSUS 3.0 RC'den WSUS 3.0 RTM'ye yükseltirken WSUS Web sitesi silinir ve yeniden oluşturulur. Sonuç olarak artık WSUS Web sitesine atanmış bir SSL sertifikası olmayacaktır. Yükseltmeden sonra sertifikayı yeniden atamanız gerekecektir.
  
#### Başarısız olan bir yükseltme işleminden kurtarma
  
WSUS 2.0'dan WSUS 3.0'a yükseltiyorsanız ve herhangi bir nedenle yükseltme başarısız olursa, WSUS 2.0'ı yeniden yüklemeniz ve veritabanını yedekten geri yüklemeniz gerekir.
  
#### Önceki bir yüklemeden kalma bir WSUS 3.0 veritabanı varsa WSUS 2.0'dan WSUS 3.0'a yükseltme yapılamaz
  
Daha önce WSUS 3.0'ı yükleyip ardından WSUS 2.0'ı yeniden yüklediyseniz, WSUS 3.0'ı yeniden yüklemeyi denemeden önce makinedeki WSUS 3.0 veritabanını silmeniz gerekir.
  
#### WSUS 3.0'a yükseltmeden önce bilgisayar adının değiştirilmesi yükseltmenin başarısız olmasına yol açabilir
  
WSUS 2.0'ı yükledikten sonra ve WSUS 3.0'a yükseltmeden önce bilgisayar adını değiştirirseniz, yükseltme başarısız olabilir.
  
ASPNET ve WSUS Administrators gruplarını kaldırıp yeniden eklemek için aşağıdaki komut dosyasını kullanın. Daha sonra, yükseltmeyi yeniden çalıştırın.
  
*&lt;VeritabanıKonumu&gt;* yerine veritabanının yüklü olduğu klasörü, *&lt;İçerikDizini&gt;* yerine de yerel depolama klasörünü kullanmanız gerekir.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Kurulum, önceki bir veritabanı yedeğinin üzerine yazabilir
  
WSUS 3.0 kurulumu, veritabanını kurulum sırasında belirtilen dizine ekler. Varsayılan olarak, bu dizin *%systemdrive%*\\WSUS\\UpdateServicesDbFiles konumundadır. Bu dizinde önceden bir veritabanı yedeği varsa, yeni veritabanı eskisinin üzerine yazılır. Yöneticiler, veritabanının bulunduğu bilgisayara güncelleştirmeleri uygulamadan önce veritabanı dosyalarını yedeklemelidir.
  
#### WSUS 2.0'da, MSDE'den SQL Server 2000 veya SQL Server 2005 geçiş yaptıysanız, bir kayıt defteri değerini değiştirmeniz gerekir.
  
Bir WSUS 2.0 yüklemeniz varsa ve SQL Server 2000 veya SQL Server 2005'ten geçiş yaptıysanız, **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** değerini 1'den 0'a değiştirmeniz gerekir. WSUS 3.0'a yükseltmeden önce böyle yapmazsanız yükseltmeniz başarısız olur.
  
#### WSUS 2.0 kurulumu başlatılır ve iptal edilirse, WSUS kayıt defteri anahtarını siler
  
WSUS 2.0 kurulumunu başlatır ve ardından iptal ederseniz, WSUS kayıt defteri anahtarı silinir. WSUS 3.0 zaten yüklüyse, bu durum sorun yaratabilir. WSUS 2.0'ı kaldırma işlemini başlatır, işlemi iptal eder ve ardından da WSUS 2.0'dan WSUS 3.0'a yükseltme işlemini başlatırsanız aynı sorun oluşur.
  
#### WSUS 3.0'ı kaldırır ve günlük dosyalarını geride bırakırsanız, yeniden yükleme sonrasında bu dosyalar doğru izinlere sahip olamayabilir
  
WSUS 3.0'ı kaldırırken, yüklemeyle ilgili günlük dosyalarını saklama seçeneğiniz vardır. WSUS 3.0'ı yeniden yüklediğinizde, eski günlük dosyaları izinlerini kaybeder (genellikle yalnızca WSUS Administrators için). Bu günlük dosyalarıyla ilgili izinleri geri yüklemelisiniz.
  
#### WSUS 3.0 RC'den sonra Windows SharePoint Services yüklenmişse, WSUS 3.0 RTM'ye yükseltme geçici bir çözüm kullanılarak başarılı olur
  
WSUS 3.0 RC'yi yükleyip ardından aynı makineye Windows SharePoint Services'ı yüklediyseniz, yalnızca özel bağlantı noktasına (bağlantı noktası 8530) yüklemeyi seçerek WSUS 3.0 RTM'ye yükseltebilirsiniz. Bu yükleme işlemini komut satırından gerçekleştirmek için, bir komut kabuğu açın ve şu komutu girin: **WSUSSetup /q / g/ DEFAULT\_WEBSITE=0**. (Yükleme işlemini kullanıcı arabirimini kullanarak gerçekleştirmek için, **WSUSSetup /g DEFAULT\_WEBSITE=0** yazın.)
  
WSUS, Çok Dilde Kullanıcı Arabirimi dil paketi yüklü bir makineye yüklüyse, Yardım kullanıcının geçerli dili yerine varsayılan dilde görüntülenir
  
#### WSUS 2.0 istemcilerinde Uygulanamaz durumlu güncelleştirmeler varsa, güncelleştirmeler, WSUS 3.0'a yükseltildikten sonra kısa bir süre için "Bilinmeyen" olarak görünür
  
Bir WSUS 2.0 sunucusunun Uygulanamaz güncelleştirmelere sahip istemcileri varsa, sunucu WSUS 3.0'a yükseltildikten sonra kısa bir süre için "Bilinmeyen" olarak görünür. İstemcinin bir sonraki tarama yapışında güncelleştirme durumu Uygulanamaz'a dönecektir.
  
Bilinen Sorunlar  
----------------
  
#### Birden fazla karşıdan yükleme hatası veya yinelenen istemci eşitleme hatası sorunlarını giderme
  
WSUS 3.0 istemcileri birden fazla karşıdan yükleme hatası bildirirse veya istemciler uzun süre WSUS 3.0 sunucusuyla eşitleme yapamazsa, istemci karşıdan yükleme önbelleğiniz bozulmuş olabilir. Bu durumdan kurtarmak için, istemci karşıdan yükleme önbelleğini dosya sisteminden silmeyi deneyebilirsiniz.
  
İstemci karşıdan yükleme önbelleğini silmek için:
  
1.  İstemci bilgisayarda şu konumdaki tüm dosyaları ve alt dizinleri silin: **%windir%\\SoftwareDistribution\\Download**  
2.  İstemci bilgisayarı WSUS 3.0 ile yeniden eşitleyerek güncelleştirmeyi yüklemeyi deneyin. Bu yükleme denemesi aşağıdaki hatayı vererek başarısız olmalıdır: **WU\_E\_DM\_NOTDOWNLOADED, "Güncelleştirme karşıdan yüklenmedi."**  
3.  Bu hatadan sonra, istemci bilgisayar karşıdan yüklemeyi otomatik olarak yeniden başlatır ve kurulum işlemi devam edebilir.
  
#### Eşitleme başarısız olursa eşitlemeyi yeniden deneyin
  
Eşitleme başarısız olursa, sorun gidermeye yönelik ilk eyleminiz sunucuyu eşitlemeyi yeniden denemek olmalıdır. Sonraki eşitlemeler başarısız olursa, [Windows Server Update Services 3.0 İşletme Kılavuzu'ndaki](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072) sorun giderme bilgilerini kullanın.
  
#### WSUS 3.0 yapılandırmasını doğrudan veritabanında değiştirme desteklenmez
  
Windows Server Update Services yapılandırma verilerini bir SQL Server veritabanında depolar. Ancak, yapılandırma verilerini doğrudan veritabanına erişerek değiştirme desteklenmez. WSUS 3.0 yapılandırmasını doğrudan veritabanına erişerek değiştirmeye çalışmayın. WSUS 3.0 yapılandırmasını WSUS 3.0 konsolunu kullanarak veya WSUS 3.0 API'lerini çağırarak değiştirmelisiniz.
  
#### Disk kotaları etkinse karşıdan yükleme hataları hızlı bir şekilde bildirilmez
  
Disk kotaları etkinleştirilmişse ve kota sınırına ulaşılmışsa, WSUS sunucusundaki güncelleştirme karşıdan yükleme hataları uygun zamanlamayla bildirilmeyebilir. Bu sorunun oluşmaması için, disk kotalarını devre dışı bırakın veya kotayı artırın.
  
#### WSUS 3.0 ürünü SSL kullanılarak dağıtılırsa, istemci bilgisayarlar 0x8024400a hata koduyla başarısız olabilir
  
İstemci bilgisayarlar WSUS 3.0 sunucusuyla SSL kullanarak iletişim kurduklarında bazen "0x8024400a" hata koduyla başarısız olabilirler. Bu sorunu gideren bir güncelleştirme için, bkz: [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593).
  
#### WSUS kaldırıldığında WSUS Administrators etki alanı hesabı silinmez
  
WSUS Administrators grubu etki alanı denetleyicilerinde bir etki alanı hesabı olarak (yerel hesap değil) oluşturulur; WSUS kaldırılırken bu hesabın silinmesi durumunda bu etki alanı hesabını kullanan tüm yüklemeler devre dışı kalır. Bu nedenle, WSUS kaldırıldığında WSUS Administrators etki alanı hesabı silinmez.
  
#### Akış aşağı bir sunucu akış yukarı bir sunucuya dönüştürüldüğünde, katalog sitesi güncelleştirmelerinin yeniden alınması gerekir
  
Akış aşağı bir sunucuyu akış yukarı bir sunucu olarak yükselttiğinizde, tüm katalog sitesi güncelleştirmelerini de yeniden almanız gerekir. Aksi halde, site yeni katalog sitesi güncelleştirmesi düzeltmelerini bu sunucuya eşitleyemez.
  
#### IIS'yi SSL ile kullanıyorsanız, "Güvenli Kanal Kullanılmasını İste" işaretli değilse hala şifrelenmemiş erişim kullanılabilir
  
Bir sertifika yükleyerek IIS'yi SSL kullanacak şekilde ayarlarsanız, "Güvenli Kanal Kullanılmasını İste" seçeneği işaretli değilse siteye şifrelenmemiş HTTP kullanılarak erişilmesi hala mümkündür. Daha fazla bilgi için, bkz: [Şifrelemeyi Etkinleştirme](http://go.microsoft.com/fwlink/?linkid=70601) (http://go.microsoft.com/fwlink/?LinkId=70601).
  
#### %windir%\\TEMP klasöründe okuma/yazma izni olmazsa katalog sitesi alma başarısız olabilir
  
Bir katalog sitesi alma işlemi gerçekleştirirken, Network Service hesabının %windir%\\TEMP klasöründe okuma/yazma izni yoksa, alma işlemi aşağıdakine benzer bir hata iletisiyle başarısız olabilir: "Sunucu isteği işleyemedi. ---&gt; 'C:\\WINDOWS\\TEMP\\*GeçiciDosyaAdı*.dll' dosyası bulunamadı."
  
#### WSUS 3.0 ile WSUS 2.0 kullanan bir akış aşağı çoğaltma sunucusu arasında eşitleme yaparken performans yavaş olabilir
  
Akış yukarı bir sunucuya WSUS 3.0 yüklerseniz ve WSUS 2.0 çalıştıran bir akış aşağı çoğaltma sunucuyla eşitlemeye çalışırsanız, performans sorunlarıyla karşılaşabilirsiniz. Bu sorunu gidermek için, bkz: [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669).
  
#### Posta sunucusu kapalıysa veya sunucuya ulaşılamıyorsa e-posta bildirimi hiçbir uyarı olmaksızın başarısız olur
  
Ağın e-posta sunucusu çevrimdışıysa, WSUS 3.0 e-posta bildirimleri göndermede sessiz bir şekilde başarısız olur. Bununla birlikte, olay günlüğüne 10052 (HealthCoreEmailNotificationRed) numaralı olayı yazar.
  
#### Akış yukarı sunucuda değiştirilen ayarlar anında akış aşağı sunucuya yansıtılmıyor
  
Akış yukarı sunucunun yapılandırması değiştirildiğinde, bu yapılandırma değişikliklerinin gerçekten etkili olması biraz zaman alabilir. Örneğin, akış yukarı sunucuda yeni bir dil seçmek gibi bir ayar değişikliği yapar ve anında akış aşağı sunucuda bir eşitleme tetiklerseniz değişiklik görünmez. Bunun yerine, bir sonraki zamanlanmış eşitlemede akış aşağı sunucuya yansıtılır. Bekleme süresi akış yukarı sunucuda bulunan güncelleştirme sayısına bağlı olarak artar.
  
#### WSUS 3.0 kaldırıldığında veritabanı örneği kaldırılmaz
  
WSUS 3.0 kaldırılırsa, veritabanı örneği kaldırılmaz. Örnek birden fazla uygulama tarafından paylaşılıyor olabilir ve kaldırılması diğer uygulamaların başarısız olmasına neden olur.
  
Windows İç Veritabanı uygulamasının kaldırılması gerekiyorsa, aşağıdaki komutlar kullanılarak kaldırılabilir:
  
(32-bit platformlarda)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(64-bit platformlarda)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Windows Server 2008 sisteminden Windows İç Veritabanı Service Pack 2'yi kaldırmak istiyorsanız, bunu Sunucu Yöneticisi'ni kullanarak yapabilirsiniz.
  
Ancak, uygulamanın kaldırılması varsayılan .mdf ve .ldf dosyalarını kaldırmayabilir ve bu da sonraki bir WSUS 3.0 yüklemesinin başarısız olmasına neden olur. Bu dosyalar %windir%\\SYSMSI\\SSEE dizininden silinebilir.
  
#### Bir akış aşağı sunucu akış yukarı sunucusunu değiştirirse, "Bilinmiyor" durum güncelleştirmeleri "Uygun Değil" olarak bildirilir
  
Bir akış aşağı sunucu farklı bir akış yukarı sunucudan eşitlemeye başlarsa, durumu "Bilinmiyor" olan güncelleştirmeler yeni akış yukarı sunucuda "Uygun Değil" olarak bildirilir. Bu durum geçicidir ve akış aşağı sunucu istemcileri kendisiyle eşitleme yaptıktan sonra durumunu yeniden bildirdiğinde düzeltilir.
  
#### Bir WSUS 3.0 çoğaltma sunucusu aynı ada sahip birden fazla bilgisayarı yönetiyorsa, raporlama toplaması başarısız olur
  
Bir WSUS 3.0 çoğaltma sunucusu aynı ada sahip birden fazla bilgisayarı yönetiyorsa, raporlama toplaması başarısız olur. Sonuç olarak, kök WSUS sunucusunda bulunan raporlar tam olmaz. Bu sorun, çoğaltma sunucuda yinelenen bilgisayar girişlerinin biri dışındaki tümü silindiğinde çözümlenir.
  
#### Sunucu Temizleme Sihirbazı bir uzak konsoldan birden fazla sunucu üzerinde çalıştırıldığında, bir sunucuda zaman aşımına uğrarsa tüm sunuculara olan bağlantılar kaybolur
  
Sunucu Temizleme Sihirbazı'nı uzak bir konsoldan birden fazla sunucu üzerinde çalıştırmak mümkündür. Ancak, temizleme işlemi sunuculardan birinde zaman aşımına uğrarsa, konsol sunucuların tümüne olan bağlantılarını kaybeder. Herhangi bir veri kaybı olmaz, ancak yöneticinin sunucuların her biri için uzak bağlantıyı sıfırlaması gerekir.
  
#### Sunucu Temizleme Sihirbazı dosyaları üç ay sonra değil, otuz gün sonra siler
  
Sunucu Temizleme Sihirbazı'ndaki bazı metinler yanlıştır. Şöyle yazar: "Süresi dolan ve üç aydır onaylanmayan güncelleştirmeleri sil ve üç aydır onaylanmayan eski güncelleştirme düzeltmelerini sil." Doğru süre üç ay değil, otuz gündür.
  
#### Bağlantının ardı ardına hızla başlatılıp durdurulması, Yapılandırma Sihirbazı'nda "hata yok" hata iletisine neden olur
  
WSUS'yi yapılandırırken, akış yukarı sunucuyla (Microsoft Update ya da intranetteki akış yukarı sunucu) ilgili temel bilgileri aktarmak için sunucuya bağlanmanız gerekir. Önce **Bağlanmaya Başla**'yı tıklatır ve hemen ardından **Bağlanmayı Durdur**'u tıklatırsanız, yanlış bir ifade olarak "Eşitleme hatası oluşmadı" hata iletisini alırsınız.
  
#### Windows Vista RTM kullanan WSUS istemcileri artık Microsoft Update'te güncelleştirme arayabilir
  
Önceki WSUS sürümlerinde, Windows Vista RTM kullanan istemciler güncelleştirmeleri yalnızca WSUS sunucusundan alabiliyordu. WSUS 3.0 RTM ile, Vista istemcileri artık güncelleştirmeleri Microsoft Update'ten de alabilmektedir. Vista istemcilerini, Denetim Masası'ndan Windows Update'i başlatıp ardından **Güncelleştirmeleri Microsoft Update kaynağından çevrimiçi olarak denetle** köprüsünü tıklatarak Microsoft Update'e yönlendirebilirsiniz. **Tüm Windows Update özelliklerine erişimi kaldır** Grup İlkesi seçeneği etkinleştirilmişse, Windows Update köprüyü görüntülemez.
  
Windows Server 2008 üzerinde WSUS 3.0  
-------------------------------------
  
#### Desteklenen Sürümler
  
WSUS 3.0, Windows Server 2008 sisteminin hem 32-bit hem de 64-bit sürümlerini destekler.
  
#### Önkoşullar
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Gereksinim</th>
<th style="border:1px solid black;" >Ayrıntılar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS)</td>
<td style="border:1px solid black;">İşletim sisteminden yükleme. Aşağıdaki bileşenlerin etkinleştirildiğinden emin olun:
Windows Kimlik Doğrulaması
Statik İçerik
ASP.NET
6.0 Yönetim Uyumluluğu
IIS Metatabanı Uyumluluğu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x86)</td>
<td style="border:1px solid black;">Windows Server 2008 üzerinde gerekmez; işletim sisteminin bir parçası olarak zaten yüklenir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Yönetim Konsolu 3.0</td>
<td style="border:1px solid black;">Windows Server 2008 üzerinde gerekmez; işletim sisteminin bir parçası olarak zaten yüklenir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Bu, WSUS kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70410) Microsoft Report Viewer Redistributable 2005 sayfasına bakın.</td>
</tr>
</tbody>
</table>
  
#### Konu 1: WSUS 3.0 çalıştırılmadan önce IIS 7.0 yapılandırma dosyasının güncelleştirilmesi gerekir
  
Windows Server 2008 üzerinde WSUS 3.0 çalıştırılmadan önce IIS yapılandırma dosyası güncelleştirmelidir. Aşağıdaki adımları uygulamanız gerekir:
  
1. IIS yapılandırma dosyasını açın: %WINDIR%\\system32\\inetsrv\\applicationhost.config
  
2. &lt;System.webServer&gt;&lt;modules&gt; etiketinde &lt;add name="CustomErrorMode"&gt; varsa bunu silin.
  
3. &lt;System.webServer&gt;&lt;modules&gt; etiketine &lt;remove name="CustomErrorMode"&gt; ekleyin.
  
Etiketin son hali aşağıdaki gibi görünmelidir:
  
```  
 &lt;System.webServer&gt; &lt;modules&gt; &lt;remove name="CustomErrorMode"&gt; &lt;/modules&gt; &lt;/System.webServer&gt;  
```
  
#### Sorun 2: WSUS 3.0'ı, Windows Server 2008 Beta 3 üzerindeki özel bağlantı noktası üzerine yüklemek isterseniz, Web sitesini yeniden oluşturmanız gerekir
  
WSUS 3.0'ı, Windows Server 2008 Beta 3 üzerine yüklemeyi düşünüyorsanız ve WSUS'yi 8530 özel bağlantı noktasını kullanmak için yapılandırmak istiyorsanız, WSUS yükleme programını başlatmadan önce 8530 bağlantı noktası üzerinde "WSUS Yönetimi" adında bir Web sitesi oluşturmanız gerekir.
  
Windows Small Business Server 2003 Üzerinde WSUS 3.0  
----------------------------------------------------
  
#### Konu 1: IIS sanal kökü belirli IP adresleri veya etki alanı adlarıyla kısıtlanmışsa, WSUS 3.0 sunucusu kendini güncelleştiremez
  
Bazı Windows Small Business Server yüklemelerinde, varsayılan IIS Web sitesi "IP adresi ve etki alanı adı kısıtlamaları" kullanmak üzere yapılandırılmış olabilir. Bu durumda, sunucudaki Windows Update İstemcisi kendini güncelleştiremeyebilir.
  
#### Konu 2: WSUS 3.0'ı Small Business Server üzerine yükleme — Tümleştirme sorunları
  
-   Windows Small Business Server 2003, Internet'e erişmek için ISA proxy sunucu kullanıyorsa, aşağıdakilerin **Ayarlar** kullanıcı arabiriminde yazılması gerekir: proxy sunucu ayarları, proxy sunucu adı ve bağlantı noktası.  
-   ISA, Windows Kimlik Doğrulaması kullanıyorsa, proxy sunucu kimlik bilgileri "ETKİALANI\\kullanıcı" biçiminde yazılmalı ve kullanıcı Internet Users grubunun üyesi olmalıdır.
  
#### Konu 3: Windows SBS sihirbazlarını kullanmadan ağınıza bir alt ağ eklediyseniz, bu yordamı gerçekleştirmeniz gerekir
  
WSUS sunucusu kurulum işlemi sunucuya iki IIS sanal kökü yükler: SelfUpdate ve ClientWebService. Kurulum ayrıca, varsayılan Web sitesinin (80 numaralı bağlantı noktasında) giriş dizinine, istemci bilgisayarların varsayılan Web sitesi üzerinden kendi kendilerini güncelleştirmelerini sağlayan bazı dosyalar yerleştirir. Varsayılan olarak, varsayılan Web sitesi localhost veya sunucuya iliştirilmiş belirli alt ağlar dışındaki tüm IP adreslerinin erişimini reddedecek şekilde yapılandırılır. Sonuç olarak, localhost üzerinde veya bu belirli alt ağlar üzerinde olmayan istemci bilgisayarlar kendi kendini güncelleştiremez. Microsoft Windows Small Business Server 2003 (Windows SBS) sihirbazlarını kullanmadan ağınıza bir alt ağ eklediyseniz, bu yordamı gerçekleştirmeniz gerekir.
  
1.  Sunucu Yönetimi'nde, **Gelişmiş Yönetim**'i genişletin, **Internet Information Services**'ı genişletin, **Web Siteleri**'ni genişletin, **Varsayılan Web Sitesi**'ni genişletin, **Selfupdate** sanal dizinini sağ tıklatın ve sonra **Özellikler**'i tıklatın.  
2.  **Dizin Güvenliği**'ni tıklatın.  
3.  **IP adresi ve etki alanı adı kısıtlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim Ver**'i tıklatın.  
4.  **Tamam**'ı tıklatın, **ClientWebService** sanal dizinini sağ tıklatın ve sonra **Özellikler**'i tıklatın.  
5.  **Dizin Güvenliği**'ni tıklatın.  
6.  **IP adresi ve etki alanı adı kısıtlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim Ver**'i tıklatın.
  
#### Telif Hakkı
  
Bu belge, son ticari sürümünden önce önemli ölçüde değişmiş olabilecek bir yazılım sürümünün bir ön sürümünü desteklemektedir ve Microsoft Corporation'ın gizli ve tescilli bilgilerini içerir. Alıcı ile Microsoft arasındaki bir açıklamama sözleşmesine uygun olarak açıklanmaktadır. Bu belge yalnızca bilgilendirme amaçlıdır ve Microsoft bu belgede, ne açıkça ne de üstü kapalı olarak herhangi bir garanti vermez. URL ve diğer Internet Web sitesi başvuruları da dahil olmak üzere işbu belgedeki bilgiler önceden haber verilmeksizin değiştirilebilir. Bu belgenin kullanımından veya kullanımından doğacak sonuçlardan kaynaklanabilecek tüm risk kullanıcıya aittir. Aksi belirtilmedikçe, buradaki örneklerde adı geçen şirketler, kuruluşlar, ürünler, etki alanı adları, e-posta adresleri, logolar, kişiler, yerler ve olaylar gerçek dışıdır. Herhangi bir gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla bir ilişki amaçlanmamaktadır ve bunun amaçlandığı sonucuna varılamaz. İlgili tüm telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakkı kapsamındaki haklara hiçbir sınırlama getirilmeksizin, bu belgenin hiçbir bölümü, Microsoft Corporation'dan yazılı izin alınmadan yeniden üretilemez, yeniden kullanılabileceği bir sisteme yerleştirilemez veya böyle bir sistemde saklanamaz veya herhangi bir biçimde veya herhangi bir araç (elektronik, mekanik, fotokopi, kayıt veya diğer) kullanılarak veya herhangi bir amaçla iletilemez.
  
Microsoft'un bu belgenin içeriğini kapsayan patentleri veya patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından sağlanan herhangi bir yazılı lisans sözleşmesinde açıkça belirtilmedikçe, bu belgenin size sağlanmış olması bu patentler, ticari markalar, telif hakları ve diğer fikri mülkiyet hakları için size herhangi bir lisans da verilmiş olduğu anlamına gelmez.
  
© 2007 Microsoft Corporation. Tüm hakları saklıdır.
  
Microsoft, SQL Server, Windows ve Windows Server, Microsoft Corporation'ın Amerika Birleşik Devletleri ve/veya diğer ülkelerdeki ticari markaları veya tescilli ticari markalarıdır.
  
Diğer tüm ticari markalar ilgili sahiplerine aittir.
