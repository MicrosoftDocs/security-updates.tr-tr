---
TOCTitle: 'Microsoft Windows Server Update Services 3.0 SP1 için Sürüm Notları'
Title: 'Microsoft Windows Server Update Services 3.0 SP1 için Sürüm Notları'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18155298
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708525(v=WS.10)'
---

Microsoft Windows Server Update Services 3.0 SP1 için Sürüm Notları
===================================================================

Bu sürüm notlarında, Microsoft® Windows® Server Update Services (WSUS) 3.0 Service Pack 1'i etkilediği bilinen sorunlar açıklanmakta ve uygulamanın yüklenmesiyle ilgili öneriler ve gereksinimler belirtilmektedir. Bu notlar aşağıdaki bölümleri içermektedir:

-   WSUS 3.0 SP1 sunucu yüklemesi için sistem gereksinimleri
-   WSUS 3.0 SP1 sunucu yüklemesi için yapılandırma gereksinimleri
-   WSUS 3.0 SP1 uzak konsol yüklemesi için sistem gereksinimleri
-   İstemci yüklemesi için sistem gereksinimleri
-   WSUS SP1 sunucu yüklemesi için yazılım gereksinimleri
-   WSUS 3.0 SP1 sunucu yüklemesi için en az disk alanı gereksinimleri
-   WSUS 3.0 SP1 yükseltme gereksinimleri
-   Kurulum komut satırı parametreleri
-   Kurulum sorunları
-   Yükseltme sorunları
-   Bilinen sorunlar
-   Windows Server® 2008 üzerinde WSUS 3.0 SP1
-   Windows Small Business Server 2003 üzerinde WSUS 3.0 SP1

WSUS 3.0 SP1 sunucu yüklemesi için sistem gereksinimleri
--------------------------------------------------------

#### WSUS 3.0 SP1, Windows Server 2008 ve Windows Server 2003 Service Pack 1 üzerinde desteklenir

WSUS 3.0 SP1 sunucusu Windows Server 2008 ve Windows Server 2003 Service Pack 1 üzerinde desteklenmektedir.

#### Windows 2000 Server, WSUS 3.0 SP1 sunucuları için desteklenmez

Microsoft Windows® 2000 Server, WSUS 3.0 SP1 sunucuları için desteklenen bir işletim sistemi değildir.

#### WSUS 3.0 SP1, Terminal Hizmetleri çalıştıran sunucularda desteklenmez

WSUS 3.0 SP1, Terminal Hizmetleri çalıştıran sunucularda çalışabilse de, bunun yapılması desteklenmemekte veya önerilmemektedir. WSUS 3.0 SP1, uzak SQL Server uygulamalarını kullanan yapılandırmalarda Terminal Hizmetlerini çalıştıran bir sunucuda çalışmaz. Terminal Hizmetleri lisans sunucusu üzerindeki tüm uzak özel eylemler (yükleme dahil) sistem hesabı olarak çalıştırılacağı ve sunucunun sistem hesabının uzak SQL Server üzerinde gereken izinleri olmayabileceği için yükleme başarısız olabilir.

WSUS 3.0 SP1 sunucu yüklemesi için yapılandırma gereksinimleri
--------------------------------------------------------------

#### IIS yüklü olmalıdır

WSUS 3.0 SP1, Windows Server 2008 veya Microsoft Windows Server 2003 üzerinde varsayılan olarak yüklü olmayan Internet Information Services'ı (IIS) gerektirir. WSUS 3.0 SP1'i IIS olmadan yüklemeyi denerseniz, Windows Server Update Services Kurulumu IIS'nin yüklü olmadığını bildiren bir hata iletisi görüntüler.

#### IIS uygulaması IIS 5.0 yalıtım modunda çalışıyorsa, yükleme başarısız olur

Sunucuyu Windows 2000 Server'dan Windows Server 2003'e yükselttiyseniz, IIS uygulaması IIS 5.0 uyumluluk modunda çalışıyor olabilir. IIS 5.0 yalıtım modunu IIS Yöneticisi'nde de etkinleştirmek mümkündür. Bu işlem yüklemenin başarısız olmasına neden olur. WSUS 3.0 SP1'i yüklemeden önce IIS 5.0 yalıtım modunu devre dışı bırakmanız gerekir.

#### Herhangi bir IIS bileşeni 64 bit platforma 32 bit uyumluluk modunda yüklenirse, WSUS 3.0 SP1 yüklemesi başarısız olabilir

Tüm IIS bileşenlerinin 64 bit platformlara yerel modda yüklenmesi gerekir. Herhangi bir IIS bileşeni 32 bit uyumluluk modundaysa, yükleme başarısız olabilir.

#### Proxy sunucular yalnızca HTTP'yi veya HTTP ve HTTPS'yi destekleyebilir

WSUS 3.0 SP1'de proxy sunucunun yalnızca HTTP'yi desteklemesi olasıdır. WSUS sunucusunu Yapılandırma Sihirbazı'ndan veya Yönetim konsolundan yapılandırmadan önce komut satırı (**wsusutil configuresslproxy**) aracılığıyla, HTTPS çalıştıran ikinci bir proxy sunucu yapılandırmalısınız.

#### Bağlantı noktası 80 üzerinde iki veya daha fazla Web sitesi zaten çalışıyorsa, WSUS'u yüklemeden önce biri dışında tümünü silin

Bağlantı noktası 80 üzerinde çalışan iki veya daha fazla Web sitesi (örneğin, Windows® SharePoint® Services) varsa, WSUS'u yüklemeden önce biri dışında tümünü silmeniz gerekir. Bunu yapmazsanız, sunucunuzun istemcileri kendisini güncelleştirmeyebilir.

#### WSUS 3.0 SP1'i yüklerken, virüsten koruma programlarını devre dışı bırakmanız gerekebilir

WSUS 3.0 SP1'i yüklerken, başarılı bir yükleme gerçekleştirebilmek için önce virüsten koruma programlarını devre dışı bırakmanız gerekebilir. Virüsten koruma programını devre dışı bıraktıktan sonra, WSUS'u yüklemeden bilgisayarı yeniden başlatın. Bilgisayarın yeniden başlatılması, yükleme işleminin dosyalara erişmesi gerektiğinde dosyaların kilitlenmesini önler. Yükleme tamamlandıktan sonra, virüsten koruma programınızı yeniden etkinleştirdiğinizden emin olun. Virüsten koruma programınızı ve sürümü devre dışı bırakıp yeniden etkinleştirmek için gerekli adımları öğrenmek üzere virüsten koruma programı satıcınızın Web sitesini ziyaret edin.

| ![](/security-updates/images/Cc708525.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu geçici çözüm, bilgisayarınızı veya ağınızı kötü amaçlı kullanıcıların veya virüs gibi kötü amaçlı yazılımların saldırılarına karşı daha açık hale getirebilir. Bu geçici çözümü önermiyoruz, ancak karar size ait olmak üzere geçici çözümü uygulayabilmeniz için bu bilgileri sağlıyoruz. Bu geçici çözümü kullanmak sizin sorumluluğunuzdadır. |

| ![](/security-updates/images/Cc708525.note(WS.10).gif)Not                                                                                                                                                                                                                                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Virüsten koruma programı, bilgisayarınızı virüslere karşı korumaya yardımcı olmak amacıyla tasarlanmıştır. Virüsten koruma programınız devre dışı kaldığında, güvenmediğiniz kaynaklardan gelen dosyaları yüklememeli veya açmamalı, güvenmediğiniz Web sitelerini ziyaret etmemeli ya da e-posta eklerini açmamalısınız. |

#### WSUS 3.0 SP1, SQL Server'da iç içe tetikleyiciler seçeneğinin açık olmasını gerektirir

İç içe tetikleyiciler seçeneği varsayılan olarak açıktır; ancak, SQL Server yöneticisi tarafından kapatılabilir.

Bir SQL Server veritabanını Windows Server Update Services veri deposu olarak kullanmayı düşünüyorsanız, WSUS 3.0 SP1 yöneticisi WSUS 3.0 SP1'i yüklemeden ve kurulum sırasında veritabanını belirtmeden önce, SQL Server yöneticisinin sunucudaki iç içe tetikleyiciler seçeneğinin açık olduğunu doğrulaması gerekir.

WSUS 3.0 SP1 Kurulumu veritabanına özgü bir seçenek olan RECURSIVE\_TRIGGERS seçeneğini açar; ancak, sunucu genelinde bir seçenek olan iç içe tetikleyiciler seçeneğini açmaz.

İç içe tetikleyiciler seçeneğinin açık olup olmadığını görmek için şunu kullanın:

**sp\_configure 'nested triggers'**

İç içe tetikleyiciler seçeneğini SQL Server'da açmak için SQL Server çalıştıran bilgisayarda bir toplu iş dosyasından şunu çalıştırın:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Sunucunuzda SQL Server Management Studio yoksa, SQL komut dosyalarını komut satırından çalıştırabilirsiniz. Microsoft SQL Server 2005 Command Line Query Utility'yi [Microsoft Yükleme Merkezi'nden edinebilirsiniz](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728). (Bu sayfa İngilizce içeriğe sahip olabilir.) Başlamak için, **sqlcmd** komutunu çalıştırın.

SQL komut dosyalarını Windows İç Veritabanı için çalıştırmak istiyorsanız, aynı yükleme sayfasından SQL Server Native Client'ı da yüklemeniz gerekir.

#### Uzak SQL sınırlamaları ve gereksinimleri

WSUS 3.0 SP1, uygulamanın geri kalanını içeren bilgisayardan ayrı bir bilgisayar üzerinde veritabanı yazılımı çalıştırma konusunda destek sağlar. Uzak SQL yüklemesini yapılandırmak için bazı gereksinimler vardır:

-   Uzak SQL çiftinin arka uç makinesi için etki alanı denetleyicisi olarak yapılandırılmış bir sunucuyu kullanamazsınız.
-   Uzak SQL yüklemesinin ön uç sunucusu olacak bilgisayar üzerinde Terminal Sunucusu çalıştırılmıyor olması gerekir.
-   Arka uç bilgisayarlarda veritabanı yazılımı olarak en azından, Windows Server 2003 çalıştıran bilgisayarlar için Microsoft SQL Server 2005 Service Pack 1 ([Microsoft Yükleme Merkezi'nde](http://go.microsoft.com/fwlink/?linkid=66143) http://go.microsoft.com/fwlink/?LinkId=66143 adresinden edinilebilir), Windows Server® 2008 çalıştıran bilgisayarlar için de SQL Server 2005 Service Pack 2 kullanmanız gerekir.
-   Hem ön uç hem de arka uç bilgisayarın Active Directory etki alanına katılması gerekir; katılmazsa, farklı etki alanlarında olduklarında, WSUS kurulumunu çalıştırmadan önce etki alanları arasında güven kurmanız gerekir.
-   Bir uzak SQL yapılandırmasına zaten WSUS 2.0 yüklediyseniz ve bunu WSUS 3.0 SP1'e yükseltmek istiyorsanız, WSUS 2.0'ı arka uç bilgisayardan kaldırmalı (Denetim Masası'ndaki **Program Ekle veya Kaldır**'ı kullanarak) ve varolan veritabanının korunduğundan emin olmalısınız. Ardından, SQL Server 2005 SP1'i veya SP2'yi yüklemeli ve varolan veritabanını yükseltmelisiniz. Son olarak, ön uç bilgisayara WSUS 3.0 SP1'i yüklemelisiniz.

WSUS 3.0 SP1 uzak konsol yüklemesi için sistem gereksinimleri
-------------------------------------------------------------

WSUS 3.0 SP1 uzak konsolu aşağıdaki platformlara yüklenebilir:

-   Windows Server 2008
-   Windows Vista® veya sonrası
-   Windows Server 2003 SP1 veya sonrası
-   Windows XP SP2 veya sonrası

İstemci yüklemesi için sistem gereksinimleri
--------------------------------------------

Otomatik Güncelleştirmeler WSUS istemci yazılımıdır. Aşağıdaki işletim sistemlerinden herhangi birinde WSUS ile birlikte kullanılabilir:

-   Windows Vista veya sonrası
-   Windows Server 2008 veya sonrası
-   Microsoft Windows Server 2003, herhangi bir sürümü
-   Microsoft Windows XP Professional SP2 veya sonrası
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 veya Windows 2000 Advanced Server SP4

WSUS 3.0 SP1 sunucu yüklemesi için yazılım gereksinimleri
---------------------------------------------------------

Aşağıdaki tablo, Windows Server 2003 SP1 platformları için gerekli yazılımları gösterir. Windows Server 2008 için gereken yazılımlar Windows Server 2008 üzerindeki WSUS 3.0 SP1 yapılandırmasının işlendiği bölümde ele alınacaktır.

WSUS 3.0 SP1 kurulumunu çalıştırmadan önce, WSUS 3.0 SP1 sunucusunun gereksinim listesini karşıladığından emin olun. Bu güncelleştirmelerden herhangi biri yükleme tamamlandığında bilgisayarı yeniden başlatmayı gerektirirse, WSUS 3.0 SP1'i yüklemeden önce yeniden başlatma gerçekleştirmelisiniz.

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
<td style="border:1px solid black;">İşletim sisteminden yükleyin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=68935) Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x64) sayfasına bakın. 64 bit platformlar için <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70637) Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x64) sayfasına bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 için Microsoft Yönetim Konsolu 3.0</td>
<td style="border:1px solid black;">Bu, WSUS 3.0 SP1 kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70412) Windows Server 2003 için Microsoft Yönetim Konsolu 3.0 (KB907265) sayfasına bakın. 64 bit platformlar için <a href="http://go.microsoft.com/fwlink/?linkid=70638">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70638) Windows Server 2003 x64 Edition için Microsoft Yönetim Konsolu 3.0 (KB907265) sayfasına bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Bu, WSUS 3.0 SP1 kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70410) Microsoft Report Viewer Redistributable 2005 sayfasına bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (isteğe bağlı)</td>
<td style="border:1px solid black;">Önceden SQL Server'ın uyumlu bir sürümünü yüklemediyseniz, WSUS 3.0 SP1 sizin için Windows İç Veritabanı uygulamasını yükler. Tam bir SQL Server veritabanı kullanmayı planlıyorsanız, (en azından) Windows Server 2003 üzerinde SQL Server 2005 SP1 (<a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Yükleme Merkezi'nde</a> http://go.microsoft.com/fwlink/?LinkId=66143 adresinden edinilebilir) veya Windows Server 2008 üzerinde SQL Server 2005 SP2 (<a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Yükleme Merkezi'nde</a> http://go.microsoft.com/fwlink/?LinkId=84823 adresinden edinilebilir) kullanmanız gerekir.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc708525.note(WS.10).gif)Not                                                                                                                                                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 2.0 önceden yüklenmişse ve SQL Server 2000 kullanıyorsa, SQL Server Desktop Engine 2000 veya SQL Server 2005 SP1 öncesi (veya Windows Server 2008 üzerinde SQL Server 2005 SP2) herhangi bir SQL Server veritabanı kullanıyorsa, WSUS 3.0 SP1 yükleme programı Windows® İç Veritabanı uygulamasını yükler ve veritabanını buna geçirir. |
  
WSUS 3.0 SP1 sunucu yüklemesi için en az disk alanı gereksinimleri  
------------------------------------------------------------------
  
Aşağıda Windows Server Update Services'ı yüklemek için gereken en az disk alanı verilmiştir:
  
-   Sistem bölümünde 1 GB  
-   Veritabanı dosyalarının depolanacağı birim için 2 GB  
-   İçeriğin depolanacağı bölüm için 20 GB
  
| ![](/security-updates/images/Cc708525.Important(WS.10).gif)Önemli                                  |  
|---------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0 SP1, sıkıştırılmış sürücülere yüklenemez. Seçtiğiniz sürücünün sıkıştırılmış olmamasına dikkat edin. |
  
WSUS 3.0 SP1 yükseltme gereksinimleri  
-------------------------------------
  
#### WSUS yüklemenizin düzgün çalıştığından emin olun ve yükseltmeden önce WSUS veritabanını yedekleyin
  
Önceki bir sürümden WSUS 3.0 SP1'e yükseltiyorsanız, geçerli yüklemenizin düzgün çalıştığından emin olun ve yükseltmeden önce WSUS veritabanını yedekleyin.
  
1.  Olay günlüklerindeki yakın zamanlarda olmuş hatalara, karşıdan akış ve karşıya akış sunucuları arasındaki eşitleme sorunlarına veya yanıt vermeyen istemci sorunlarına bakın. Devam etmeden önce bu sorunların giderildiğinden emin olun.  
2.  WSUS veritabanında düzgün dizin oluşturulduğundan emin olmak için DBCC CHECKDB komutunu çalıştırabilirsiniz. DBCC CHECKDB hakkında daha fazla bilgi için [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948) sayfasına bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)  
3.  WSUS veritabanını yedekleyin.
  
#### WSUS tarafından kullanılan bağlantı noktasını elle değiştirdiyseniz, yükseltmeden önce bunu kaldırın
  
WSUS için bağlantı noktasını değiştirirken, el ile değiştirmeyi denemek yerine her zaman wsusutil yardımcı programını kullanın. Bağlantı noktasını el ile değiştirip Software Update Services 1.0'ı daha önce WSUS 2.0'a yükselttiyseniz:
  
1.  Henüz WSUS 3.0 yüklemediyseniz, veritabanını ve içeriğini koruyarak WSUS 2.0'ı kaldırın. (WSUS 3.0'ı zaten yüklediyseniz, veritabanını ve içeriğini koruyarak uygulamayı kaldırın.)  
2.  SUS 1.0'ı kaldırma uygulaması tarafından erişebilecek şekilde geçici olarak yeniden etkinleştirerek Varsayılan Web Sitesini başlatın.  
3.  SUS 1.0'ı kaldırın.  
4.  WSUS 3.0'ı yükleyin.
  
#### Software Update Services 1.0'ın kaldırılması gerekir
  
Aynı makinede Software Update Services 1.0 yüklüyse, WSUS 3.0 SP1'in yüklenmesi başarısız olur. WSUS 3.0 SP1'i yüklemeden önce Software Update Services 1.0'ı kaldırmanız gerekir.
  
#### 64 bit işletim sisteminde WSUS 2.0'dan WSUS 3.0 SP1'e yükseltmek olası değildir
  
WSUS 2.0, 64 bit işletim sistemlerinde desteklenmez. 64 bit işletim sistemlerinde WSUS 2.0'dan WSUS 3.0 SP1'e yükseltmek olası değildir.
  
Kurulum komut satırı parametreleri  
----------------------------------
  
WSUS komut satırı kurulum programını kullanarak katılımsız WSUS 3.0 SP1 yüklemeleri gerçekleştirebilirsiniz. Bu tabloda WSUS 3.0 SP1 kurulumu için komut satırı parametreleri gösterilmiştir.
  
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
<td style="border:1px solid black;">Ürünü kaldırır. Yüklüyse Windows İç Veritabanı örneğini de kaldırır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Yalnızca önkoşul denetimi. Ürünü yüklemez, ancak sistemi inceler ve eksik olan tüm önkoşulları bildirir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Komut satırı seçeneklerini ve açıklamalarını görüntüler.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Önceki WSUS sürümünden yükseltir. (SUS 1.0'dan yükseltmeyi deneme.) Bu seçenekteki geçerli tek parametre /q'dur (sessiz yükleme). Bu seçenekteki geçerli tek özellik DEFAULT_WEBSITE'tır.</td>
</tr>
</tbody>
</table>
  
Bu tabloda WSUS 3.0 SP1 için komut satırı özellikleri gösterilmiştir.
  
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
<td style="border:1px solid black;">İçerik dizininin yolu. Varsayılan <em>WSUSYüklemeSürücüsü</em><strong>\WSUS\WSUSContent</strong>'dır, burada <em>WSUSYüklemeSürücüsü</em> en fazla boş alana sahip yerel sürücüdür.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Windows İç Veritabanı veri dizininin yolu.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Ad, <em>SunucuAdı</em>\<em>SQLÖrneğiAdı</em> biçiminde olmalıdır. Veritabanı örneği yerel makinede bulunuyorsa, %COMPUTERNAME% ortam değişkenini kullanın. Mevcut bir örnek yoksa, varsayılan değer %COMPUTERNAME%\WSUS şeklindedir.</td>
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
<td style="border:1px solid black;">0=günlük dosyalarını koru, 1=günlük dosyalarını kaldır (/u yükleme anahtarıyla birlikte kullanılır).</td>
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
<td style="border:1px solid black;">1=Microsoft Update Geliştirme Programı'na katıl, 0=Microsoft Update Geliştirme Programı'na katılma</td>
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
| ![](/security-updates/images/Cc708525.Important(WS.10).gif)Önemli                                                                                                    |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0 SP1'i sessiz modda (/q) yüklerseniz ve makinede tüm önkoşullar yüklü değilse, yükleme işlemi WSUSPreReqCheck.xml adlı bir dosya oluşturur ve %TEMP% dizinine kaydeder. |
  
Kurulum sorunları  
-----------------
  
#### WSUS 3.0 SP1 Kurulumu sırasında IIS yeniden başlatılır
  
WSUS 3.0 SP1 Kurulumu bildirmeksizin IIS'yi yeniden başlatır, bu da kuruluşunuzdaki varolan Web sitelerini etkileyebilir. IIS çalışmıyorsa, WSUS 3.0 SP1 kurulumu onu başlatır.
  
#### Bağlantılar varolan bir WSUS veritabanına açıksa, yükleme başarısız olabilir
  
Varolan bir yüklemeden WSUS 3.0 SP1'e yükseltiyorsanız ve bağlantılar varolan WSUS veritabanı için hala açıksa (örneğin, SQL Server Management Studio açıksa), yükleme başarısız olabilir. Lütfen tüm bağlantıları kapatıp WSUS 3.0 SP1'i yeniden yükleyin.
  
#### WSUS kurulumu veritabanı dosyaları için yanlış dizin gösterir
  
WSUS kurulumunda, **Yüklemeye Hazır** ekranı yanlış olarak veritabanının bulunduğu konumun üst dizinini veritabanı konumu olarak bildirir. Örneğin, varsayılan konum %systemdrive%\\WSUS\\UpdateServicesDbFiles olmasına karşın, bu konum hatalı olarak %systemdrive%\\WSUS şeklinde görünür.
  
#### WSUS, İngilizce dışında varsayılan dili olan Çok Dilde Kullanıcı Arabirimi Paketi dil paketlerine sahip bir makineye yüklenirse, Yardım İngilizce olarak değil varsayılan dilde görüntülenir
  
İngilizce dışında varsayılan dili olan Çok Dilde Kullanıcı Arabirimi Paketi dil paketlerine sahip bir makineniz varsa, geçerli kullanıcının yerel ayarı İngilizce olduğunda WSUS'u yine de yükleyebilirsiniz. Kullanıcı arabirimi İngilizce görüntülenir, ancak Yardım'ın da İngilizce görünmesini sağlamak için bir geçici çözüm kullanmanız gerekir. İngilizce Yardım .chm dosyasını (*WSUSInstallDir*\\documentation\\mui\\0409\\WSUS30Help.chm) ana belge dizinine (*WSUSInstallDir*\\documentation\\WSUS30Help.chm) kopyalayın. Yardım'ın bundan sonra tüm dillerde düzgün görüntülenmesi gerekir.
  
Yükseltme sorunları  
-------------------
  
#### Başarısız bir yükseltmeden kurtarma
  
WSUS'un önceki bir sürümünden (WSUS 3.0, WSUS 2.0 SP1 veya WSUS 2.0) WSUS 3.0 SP1'e yükseltiyorsanız ve yükseltme herhangi bir nedenle başarısız oluyorsa:
  
1.  WSUS'un önceki sürümünü yeniden yükleyin.  
2.  Veritabanını, yükseltmeyi denemeden önce aldığınız yedekten geri yükleyin. (Çoğu durumda, WSUS da otomatik olarak yedek oluşturur. Yeri için WSUSSetup.log dosyasına bakın.)  
3.  Hatanın nedenini bulmak için günlükleri inceleyin ve sorunu düzeltin.  
4.  WSUS'u yükseltmeyi yeniden deneyin.
  
#### Önceki yüklemden bir WSUS 3.0 SP1 veritabanı varsa, WSUS 2.0'dan WSUS 3.0 SP1'e yükseltmek mümkün değildir
  
Daha önce WSUS 3.0 SP1 yüklediyseniz ve sonra WSUS 2.0'ı yeniden yüklediyseniz, WSUS 3.0 SP1'i yeniden yüklemeyi denemeden önce makinedeki WSUS 3.0 SP1 veritabanını silmeniz gerekir.
  
#### WSUS 3.0 SP1'e yükseltmeden önce bilgisayar adını değiştirmek yükseltmenin başarısız olmasına neden olabilir
  
Bilgisayarın adını WSUS 2.0'ı yükledikten sonra ve WSUS 3.0 SP1'e yükseltmeden önce değiştirirseniz, yükseltme başarısız olabilir.
  
ASPNET ve WSUS Administrators gruplarını kaldırıp yeniden eklemek için aşağıdaki komut dosyasını kullanın. Daha sonra, yükseltmeyi yeniden çalıştırın.
  
*&lt;VeritabanıKonumu&gt;* yerine veritabanının yüklü olduğu klasörü, *&lt;İçerikDizini&gt;* yerine de yerel depolama klasörünü kullanmanız gerekir.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Kurulum, önceki bir veritabanı yedeğinin üzerine yazabilir
  
WSUS 3.0 SP1 kurulumu, veritabanını *sürücü*\\WSUS şeklindeki varsayılan dizine ekler (burada *sürücü* en fazla boş alana sahip yerel NTFS sürücüsüdür). Bu dizinde bir veritabanı yedeği varsa, üzerine yazılabilir. Yöneticiler, WSUS 3.0 SP1'e yükseltmeden önce geçerli sürümün veritabanı yedeğini farklı bir konuma kaydetmelidir.
  
#### MSDE'den WSUS 2.0 üzerinde SQL Server 2000'e veya SQL Server 2005'e geçtiyseniz, bir kayıt defteri değerini değiştirmeniz gerekir
  
WSUS 2.0 yüklemeniz varsa ve SQL Server 2000'den veya SQL Server 2005'ten geçtiyseniz, **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** değerini 1'den 0'a değiştirmeniz gerekir. WSUS 3.0 SP1'e yükseltmeden önce bunu yapmazsanız, yükseltme başarısız olur.
  
#### WSUS 2.0 kurulumu başlatılır ve iptal edilirse, WSUS kayıt defteri anahtarını siler
  
WSUS 2.0 kurulumunu başlatır ve sonra iptal ederseniz, WSUS kayıt defteri anahtarı silinir. WSUS 3.0 SP1 zaten yüklüyse, bu sorunlara neden olabilir. WSUS 2.0'ı kaldırmaya başlar ve ardından işlemi iptal edip WSUS 2.0'dan WSUS 3.0 SP1'e yükseltmeyi denerseniz, aynı sorun oluşur.
  
#### WSUS 3.0 SP1'i kaldırır ve günlük dosyalarını geride bırakırsanız, yeniden yükleme sonrasında bu dosyalar doğru izinlere sahip olamayabilir
  
WSUS 3.0 SP1'i kaldırırken, yüklemeyle ilgili günlük dosyalarını saklama seçeneğiniz vardır. WSUS 3.0 SP1'i yeniden yüklediğinizde, eski günlük dosyaları izinlerini kaybeder (genellikle yalnızca WSUS Administrators için). Bu günlük dosyalarıyla ilgili izinleri geri yüklemeniz gerekir.
  
#### WSUS 2.0 istemcilerinin "Uygulanamaz" durumundaki güncelleştirmeleri varsa, WSUS 3.0 SP1'e yükselttikten kısa bir süre sonra bu güncelleştirmeler "Bilinmiyor" şeklinde görünür
  
WSUS 2.0 sunucusunun **Uygulanamaz** durumunda güncelleştirmeleri olan istemcileri varsa, sunucu WSUS 3.0 SP1'e yükseltildikten kısa bir süre sonra bu güncelleştirmeler **Bilinmiyor** durumuna sahip olarak görünür. İstemcinin bir sonraki taramasından sonra, güncelleştirme durumu **Uygulanamaz** haline geri döner.
  
Bilinen Sorunlar  
----------------
  
#### Birden çok karşıdan yükleme hatasını veya yinelenen istemci eşitleme hatalarını giderme
  
WSUS 3.0 SP1 istemcileri birden çok karşıdan yükleme hatası bildiriyorsa veya istemciler uzun bir süre WSUS 3.0 SP1 sunucusuyla eşitleme yapamıyorsa, istemci karşıdan yükleme önbelleğiniz bozulmuş olabilir. Bu durumdan kurtulmak için, istemci karşıdan yükleme önbelleğini dosya sisteminden silmeyi deneyebilirsiniz.
  
İstemci karşıdan yükleme önbelleğini silmek için:
  
1.  İstemci bilgisayardaki bu konumdaki tüm dosya ve alt dizinleri silin: **%windir%\\SoftwareDistribution\\Download**  
2.  WSUS 3.0 SP1 olan istemci bilgisayarla yeniden eşitleme yaparak yükseltmeyi yüklemeyi deneyin. Bu yükleme denemesinin şu hata ile başarısız olması gerekir: **WU\_E\_DM\_NOTDOWNLOADED, "Güncelleştirme yüklenmedi."**  
3.  Bu hatadan sonra, istemci bilgisayar karşıdan yüklemeyi otomatik olarak yeniden başlatır ve yükleme devam edebilir.
  
#### Eşitleme başarısız olursa, yeniden eşitleme yapmayı deneyin
  
Eşitleme başarısız olursa, sorun giderme eyleminizdeki ilk adım sunucuyu yeniden eşitlemeyi denemek olmalıdır. Sonraki eşitlemeler başarısız olursa, [Windows Server Update Services 3.0 Çalıştırma Kılavuzu](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072) sayfasındaki sorun giderme bilgilerini kullanın. (Bu sayfa İngilizce içeriğe sahip olabilir.)
  
#### WSUS 3.0 SP1 yapılandırmasını doğrudan veritabanında değiştirmek desteklenmez
  
Windows Server Update Services yapılandırma verilerini SQL Server veritabanına depolar. Ancak, bu veritabanına doğrudan erişerek yapılandırma verilerini değiştirmek desteklenmez. WSUS 3.0 SP1 yapılandırmasını veritabanına doğrudan erişerek değiştirmeyi denemeyin. WSUS 3.0 SP1 yapılandırmasını WSUS 3.0 SP1 konsolunu kullanarak veya WSUS 3.0 SP1 API'lerini çağırarak değiştirmelisiniz.
  
#### Disk kotaları etkinse karşıdan yükleme hataları hızlı bir şekilde bildirilmez
  
Disk kotaları etkinleştirilmişse ve kota sınırına ulaşılmışsa, WSUS sunucusundaki güncelleştirme karşıdan yükleme hataları zamanında bildirilmeyebilir. Bu sorunun oluşmaması için, disk kotalarını devre dışı bırakın veya kotayı artırın.
  
#### WSUS 3.0 SP1 ürünü SSL kullanılarak dağıtılırsa, istemci bilgisayarlar 0x8024400a hata koduyla başarısız olabilir
  
İstemci bilgisayarlar WSUS 3.0 SP1 sunucusuyla SSL kullanarak iletişim kurduklarında bazen 0x8024400a hata koduyla başarısız olabilirler. Bu sorunu gideren bir güncelleştirme için bkz: [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593). (Bu sayfa İngilizce içeriğe sahip olabilir.)
  
#### WSUS kaldırıldığında WSUS Administrators etki alanı hesabı silinmez
  
WSUS Administrators grubu etki alanı denetleyicilerinde bir etki alanı hesabı olarak (yerel hesap değil) oluşturulur; WSUS kaldırılırken bu hesabın silinmesi durumunda bu etki alanı hesabını kullanan tüm yüklemeler devre dışı kalır. Bu nedenle, WSUS'un kaldırılması WSUS Administrators etki alanı hesabını silmez.
  
#### Karşıdan akış sunucusu karşıya akış sunucusuna dönüştürüldüğünde, katalog sitesi güncelleştirmelerinin yeniden alınması gerekir
  
Karşıdan akış sunucusunu karşıya akış sunucusuna yükselttiğinizde, tüm katalog sitesi güncelleştirmelerini de yeniden almanız gerekir. Almazsanız, site yeni katalog sitesi güncelleştirmesi düzeltmelerini bu sunucuya eşitleyemez.
  
#### IIS'yi SSL ile kullanıyorsanız, "Güvenli Kanal Kullanılmasını İste" işaretli değilse şifrelenmemiş erişim hala kullanılabilir
  
Bir sertifika yükleyerek IIS'yi SSL kullanacak şekilde ayarlarsanız, **Güvenli Kanal Kullanılmasını İste** seçeneği işaretli olmadığı sürece siteye şifrelenmemiş HTTP kullanılarak erişilmesi hala mümkündür. Daha fazla bilgi için [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084) belgelerine bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)
  
#### %windir%\\TEMP klasörü için okuma/yazma izni olmazsa katalog sitesi alma başarısız olabilir
  
Bir katalog sitesi alma işlemi gerçekleştirirken, Network Service hesabının %windir%\\TEMP klasörü için okuma/yazma izni yoksa, alma işlemi aşağıdakine benzer bir hata iletisiyle başarısız olabilir: Sunucu isteği işleyemedi. ---&gt; "C:\\WINDOWS\\TEMP\\*GeçiciDosyaAdı*.dll dosyası bulunamadı."
  
#### WSUS 3.0 SP1 ile WSUS 2.0 kullanan bir karşıdan akış çoğaltma sunucusu arasında eşitleme yaparken performans yavaş olabilir
  
Bir karşıya akış sunucusuna WSUS 3.0 SP1 yüklerseniz ve WSUS 2.0 çalıştıran bir karşıdan akış çoğaltma sunucusuyla eşitlemeye çalışırsanız, performans sorunlarıyla karşılaşabilirsiniz. Bu sorunu gidermek için bkz: [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669). (Bu sayfa İngilizce içeriğe sahip olabilir.)
  
#### E-posta sunucusu kapalıysa veya sunucuya ulaşılamıyorsa e-posta bildirimi hiçbir uyarı olmaksızın başarısız olur
  
Ağın e-posta sunucusu çevrimdışıysa, WSUS 3.0 SP1 e-posta bildirimleri göndermede sessiz bir şekilde başarısız olur. Ancak, olay günlüğüne 10052 (HealthCoreEmailNotificationRed) numaralı olayı yazar.
  
#### Karşıya akış sunucusunda değiştirilen ayarlar anında karşıdan akış sunucusuna yansıtılmıyor
  
Karşıya akış sunucusunun yapılandırması değiştirildiğinde, bu yapılandırma değişikliklerinin gerçekte etkili olması biraz zaman alabilir. Örneğin, karşıya akış sunucusunda yeni bir dil seçmek gibi bir ayar değişikliği yapar ve anında karşıdan akış sunucusunda bir eşitleme başlatırsanız, değişiklik görünmez. Bunun yerine, karşıdan akış sunucusuna bir sonraki zamanlanmış eşitlemede yansıtılır. Bekleme süresi karşıdan akış sunucusunda bulunan güncelleştirme sayısına bağlı olarak artar.
  
#### WSUS 3.0 SP1 kaldırıldığında veritabanı örneği kaldırılmaz
  
WSUS 3.0 SP1 kaldırılırsa, veritabanı örneği kaldırılmaz. Örnek birden fazla uygulama tarafından paylaşılıyor olabilir ve kaldırılması diğer uygulamaların başarısız olmasına neden olur.
  
Windows İç Veritabanı uygulamasının kaldırılması gerekiyorsa, aşağıdaki komutlar kullanılarak kaldırılabilir:
  
(32 bit platformlarda)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(64 bit platformlarda)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Windows Server 2008 sisteminden Windows İç Veritabanı Service Pack 2'yi kaldırmak istiyorsanız, bunu Sunucu Yöneticisi'ni kullanarak yapabilirsiniz.
  
Ancak, uygulamanın kaldırılması varsayılan .mdf ve .ldf dosyalarını kaldırmayabilir ve bu da sonraki bir WSUS 3.0 SP1 yüklemesinin başarısız olmasına neden olur. Bu dosyalar %windir%\\SYSMSI\\SSEE dizininden silinebilir.
  
#### Bir karşıdan akış sunucusu kendi karşıya akış sunucusunu değiştirirse, "Bilinmiyor" durumlu güncelleştirmeler "Uygulanamaz" olarak bildirilir
  
Bir karşıdan akış sunucusu farklı bir karşıya akış sunucusundan eşitleme yapmaya başlarsa, durumu **Bilinmiyor** olan güncelleştirmeler yeni karşıya akış sunucusunda **Uygulanamaz** olarak bildirilir. Bu durum geçicidir ve karşıdan akış sunucusu istemcileri kendisiyle eşitleme yaptıktan sonra durumunu yeniden bildirdiğinde düzeltilir.
  
#### Sunucu Temizleme Sihirbazı bir uzak konsoldan birden fazla sunucu üzerinde çalıştırıldığında bir sunucuda zaman aşımına uğrarsa, tüm sunuculara olan bağlantılar kaybolur
  
Sunucu Temizleme Sihirbazı'nı tek bir uzak konsoldan birden fazla sunucu üzerinde çalıştırmak mümkündür. Ancak, temizleme işlemi sunuculardan birinde zaman aşımına uğrarsa, konsol sunucuların tümüne olan bağlantılarını kaybeder. Herhangi bir veri kaybı olmaz, ancak yöneticinin sunucuların her biri için uzak bağlantıyı sıfırlaması gerekir.
  
#### Bağlantıyı art arda hızla başlatıp durdurma, Yapılandırma Sihirbazı'nda "Eşitleme hatası oluşmadı" hata iletisine neden olur
  
WSUS'u yapılandırırken, karşıya akış sunucusuyla (Microsoft Update ya da intranetteki karşıya akış sunucusu) ilgili temel bilgileri aktarmak için sunucuya bağlanmanız gerekir. Önce **Bağlanmaya Başla**'yı tıklatır ve hemen ardından **Bağlanmayı Durdur**'u tıklatırsanız, yanlış bir ifade olarak "Eşitleme hatası oluşmadı" hata iletisini alırsınız.
  
Windows Server 2008 üzerinde WSUS 3.0 SP1  
-----------------------------------------
  
#### Desteklenen Sürümler
  
WSUS 3.0 SP1, hem 32 bit hem de 64 bit Windows Server 2008 sürümlerini destekler.
  
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
<td style="border:1px solid black;">İşletim sisteminden yükleyin. Aşağıdaki bileşenlerin etkinleştirildiğinden emin olun:
<ul>
<li>Windows Kimlik Doğrulaması<br />
<br />
</li>
<li>Statik İçerik<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>6.0 Yönetim Uyumluluğu<br />
<br />
</li>
<li>6.0 IIS Metatabanı Uyumluluğu<br />
<br />
</li>
</ul></td>
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
<td style="border:1px solid black;">Bu, WSUS kullanıcı arabirimini kullanmak için bir önkoşuldur. <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Yükleme Merkezi'ndeki</a> (http://go.microsoft.com/fwlink/?LinkId=70410) Microsoft Report Viewer Redistributable 2005 sayfasına bakın. (Bu sayfa İngilizce içeriğe sahip olabilir.)</td>
</tr>
</tbody>
</table>
  
#### Güvenlik Yapılandırma Sihirbazını Kullanma
  
Windows Server 2008'de, Güvenlik Yapılandırma Sihirbazı'nı (SCW) çalıştırdığınızda, WSUS rolünü seçebilir ve bağımlılıklarını etkinleştirebilirsiniz. SCW'yi çalıştırmak için **Başlat**'ı tıklatın, **Yönetimsel Araçlar**'ın üzerine gelin ve **Güvenlik Yapılandırma Sihirbazı**'nı tıklatın.
  
SCW'yi WSUS rolüyle birlikte kullanmada aşağıdaki bilinen sorunlar vardır:
  
-   **Windows İç Veritabanı hizmeti, WSUS tarafından kullanılamasa bile etkinleştirilir.** WSUS'u Windows İç Veritabanı veya SQL Server veritabanı gibi bir veritabanını kullanmak için yapılandırırsınız. WSUS, SQL Server ile birlikte yüklenmemişse ve SCW'de WSUS rolünü seçerseniz, Windows İç Veritabanı hizmeti bilgisayarda yüklüyse etkinleştirilir, ancak WSUS tarafından kullanılmaz. Windows İç Veritabanı yerine SQL Server veritabanını kullanıyorsanız, Windows İç Veritabanı hizmetini devre dışı bırakmanız gerekir.  
-   **Özel Web sitesindeki WSUS güvenlik duvarı kuralları varsayılan olarak seçilmez.** WSUS'u bir özel Web sitesine yüklerseniz (bağlantı noktası 8530 veya 8531), SCW'de WSUS rolünü seçseniz bile gerekli güvenlik duvarı kuralları otomatik olarak seçilmez. WSUS için gerekli güvenlik duvarı kurallarını, WSUS sunucusu için Güvenli Yuva Katmanı'nın (SSL) yapılandırılıp yapılandırılmadığına bağlı olarak etkinleştirmelisiniz.
  
Windows Small Business Server 2003 üzerinde WSUS 3.0 SP1  
--------------------------------------------------------
  
#### IIS sanal kökü belirli IP adresleri veya etki alanı adlarıyla sınırlanmışsa, WSUS 3.0 SP1 sunucusu kendini güncelleştiremez
  
Bazı Windows Small Business Server yüklemelerinde, varsayılan IIS Web sitesi **IP adresi ve etki alanı adı sınırlamaları** kullanmak üzere yapılandırılmış olabilir. Bu durumda, sunucudaki Windows Update İstemcisi kendini güncelleştiremeyebilir.
  
#### WSUS 3.0 SP1'i Small Business Server üzerine yükleme — Tümleştirme sorunları
  
-   Windows Small Business Server 2003, Internet'e erişmek için ISA proxy sunucu kullanıyorsa, **Ayarlar** kullanıcı arabiriminde aşağıdakilerin yazılması gerekir: **proxy sunucu ayarları, proxy sunucu adı, bağlantı noktası**.  
-   ISA, Windows Kimlik Doğrulaması kullanıyorsa, proxy sunucu kimlik bilgileri *ETKİALANI*\\*kullanıcı* biçiminde yazılmalı ve kullanıcı Internet Users grubunun üyesi olmalıdır.
  
#### Windows SBS sihirbazlarını kullanmadan ağınıza bir alt ağ eklediyseniz, bu yordamı gerçekleştirmeniz gerekir
  
WSUS sunucusu kurulum işlemi sunucuya iki IIS sanal kökü yükler: SelfUpdate ve ClientWebService. Kurulum ayrıca, varsayılan Web sitesinin (80 numaralı bağlantı noktasında) giriş dizini altına, istemci bilgisayarların varsayılan Web sitesi üzerinden kendi kendilerini güncelleştirmelerini sağlayan bazı dosyalar yerleştirir. Varsayılan olarak, varsayılan Web sitesi, localhost veya sunucuya iliştirilmiş belirli alt ağlar dışındaki tüm IP adreslerine erişimi reddedecek şekilde yapılandırılır. Sonuç olarak, localhost üzerinde veya bu belirli alt ağlar üzerinde olmayan istemci bilgisayarlar kendi kendini güncelleştiremez. Microsoft Windows Small Business Server 2003 (Windows SBS) sihirbazlarını kullanmadan ağınıza bir alt ağ eklediyseniz, bu yordamı gerçekleştirmeniz gerekir:
  
1.  Sunucu Yönetimi'nde, sırasıyla **Gelişmiş Yönetim**'i, **Internet Information Services**'ı, **Web Siteleri**'ni ve **Varsayılan Web Sitesi**'ni genişletin ve **Selfupdate** sanal dizinini sağ tıklatıp ardından **Özellikler**'i tıklatın.  
2.  **Dizin Güvenliği**'ni tıklatın.  
3.  **IP adresi ve etki alanı adı sınırlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim İzni Verilsin**'i tıklatın.  
4.  **Tamam**'ı tıklatın, **ClientWebService** sanal dizinini sağ tıklatın ve sonra **Özellikler**'i tıklatın.  
5.  **Dizin Güvenliği**'ni tıklatın.  
6.  **IP adresi ve etki alanı adı sınırlamaları** altında, **Düzenle**'yi tıklatın ve sonra **Erişim İzni Verilsin**'i tıklatın.
  
Telif Hakkı  
-----------
  
URL ve diğer Internet Web sitesi başvuruları da dahil olmak üzere bu belgedeki bilgiler önceden haber verilmeksizin değiştirilebilir. Aksi belirtilmedikçe, buradaki örneklerde adı geçen şirketler, kuruluşlar, ürünler, etki alanı adları, e-posta adresleri, logolar, kişiler, yerler ve olaylar gerçek dışıdır. Herhangi bir gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla bir ilişki amaçlanmamaktadır ve bunun amaçlandığı sonucuna varılamaz. İlgili tüm telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakkı kapsamındaki haklara hiçbir sınırlama getirilmeksizin, bu belgenin hiçbir bölümü, Microsoft Corporation'dan açık yazılı izin alınmadan yeniden üretilemez, yeniden kullanılabileceği bir sisteme yerleştirilemez veya böyle bir sistemde saklanamaz veya herhangi bir biçimde veya herhangi bir araç (elektronik, mekanik, fotokopi, kayıt veya diğer) kullanılarak veya herhangi bir amaçla iletilemez.
  
Microsoft'un bu belgenin içeriğini kapsayan patentleri veya patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından sağlanan herhangi bir yazılı lisans sözleşmesinde açıkça belirtilmedikçe, bu belgenin size sağlanmış olması bu patentler, ticari markalar, telif hakları ve diğer fikri mülkiyet hakları için size herhangi bir lisans da verilmiş olduğu anlamına gelmez.
  
© 2007 Microsoft Corporation. Tüm hakları saklıdır.
  
Microsoft, SQL Server, Windows ve Windows Server, Microsoft Corporation'ın Amerika Birleşik Devletleri ve/veya diğer ülkelerdeki tescilli ticari markaları veya ticari markalarıdır.
  
Diğer tüm ticari markalar ilgili sahiplerine aittir.
