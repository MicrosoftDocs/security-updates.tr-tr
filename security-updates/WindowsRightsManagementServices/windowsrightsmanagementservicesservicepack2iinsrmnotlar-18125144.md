---
TOCTitle: Windows Rights Management Services Service Pack 2 için Sürüm Notları
Title: Windows Rights Management Services Service Pack 2 için Sürüm Notları
ms:assetid: '78067886-681f-49a6-b43d-bfd08a369b69'
ms:contentKeyID: 18125144
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747637(v=WS.10)'
---

Windows Rights Management Services Service Pack 2 için Sürüm Notları
====================================================================

*Sürüm Tarihi: Aralık 2006*

Başlamadan Önce
---------------

Microsoft® Windows® Rights Management Services (RMS) Service Pack 2 (SP2) ürününü yüklemeden önce aşağıdaki bilgileri gözden geçirin. Bu sürüm notlarının içerdiği bilgiler RMS SP2 sunucusu için geçerlidir; RMS istemcisi için geçerli değildir. RMS istemcileri hakkında bilgi için Rights Management Services'e ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) bakın.

#### Sistem gereksinimleri

RMS SP2'yi çalıştırmaya yönelik donanım gereksinimleri aşağıdaki tabloda listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Gereksinim</th>
<th style="border:1px solid black;" >Öneri</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Bir Pentium III işlemcili (800 MHz veya daha hızlı) bilgisayar</td>
<td style="border:1px solid black;">İki Pentium 4 işlemcili (1500 MHz veya hızlı) bilgisayar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">256 MB RAM</td>
<td style="border:1px solid black;">512 MB RAM</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">20 GB boş sabit disk alanı</td>
<td style="border:1px solid black;">40 GB boş sabit disk alanı</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Not                                                |  
|---------------------------------------------------------------------------------------------------------------------|  
| RMS SP2 sunucusu, 32-bit bilgisayarlar için tasarlanmıştır. 64-bit bilgisayara yüklenirse, öykünme modunda çalışır. |
  
RMS SP2 çalışan sunucular için yazılım gereksinimleri aşağıdaki tabloda listelenmektedir.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bileşen</th>
<th style="border:1px solid black;" >Gereksinim</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">İşletim sistemi</td>
<td style="border:1px solid black;">RMS SP2 için, Web Edition dışında Microsoft Windows Server® 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rights Management Services SP2</td>
<td style="border:1px solid black;">RMS SP2'ye yükseltebilmeniz için RMS Service Pack 1 (SP1) yüklü olmalıdır. Bu gereksinim RMS SP2 istemcisi için geçerli değildir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Dosya sistemi</td>
<td style="border:1px solid black;">NTFS dosya sistemi önerilir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Gerekli bileşenler</td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (MSMQ da denir); Active Directory® dizin hizmeti tümleştirmesi etkinleştirilmiş olarak.<br />
<br />
</li>
<li>Internet Information Services (IIS); ASP.NET etkinleştirilmiş olarak.<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

| ![](images/Cc747637.note(WS.10).gif)Not                                                                                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS SP2'yi uzaktan yönetime olanak verecek şekilde yapılandırırsanız, RMS SP2 Yönetimi hizmetine bağlanacak bilgisayarın Internet Explorer 6.0 veya sonraki bir sürümünü kullanması gerekir. |

RMS SP2 çalışan sunucular için alt yapı gereksinimleri aşağıdaki tabloda listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bileşen</th>
<th style="border:1px solid black;" >Gereksinimler</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Dizin hizmetleri</td>
<td style="border:1px solid black;">Windows Server 2000 Service Pack 3 (SP3) veya daha sonraki bir sürümünü çalıştıran etki alanı denetleyicilerinde Active Directory, RMS'nin yüklü olduğu etki alanında olmalıdır. Lisans almak ve içerik yayımlamak için RMS'yi kullanan tüm kullanıcıların ve grupların Active Directory'de yapılandırılmış bir e-posta adresi bulunmalıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Veritabanı sunucusu</td>
<td style="border:1px solid black;">RMS SP2, işlem yapmak için bir veritabanı ve depolanmış yordamlara ihtiyaç duyar. Microsoft SQL Server™ 2000 SP3a veya sonrası ya da Microsoft SQL Server 2005 kullanabilirsiniz. Sınama veya diğer bağımsız bilgisayar dağıtımı için, Microsoft SQL Server Desktop Engine (MSDE 2000) Release A veya Microsoft SQL Server 2005 Express Edition kullanılabilir.</td>
</tr>
</tbody>
</table>
  
RMS, Microsoft SQL Server 2000 ve Microsoft SQL Server 2005 çalışan veritabanı sunucuları için tasarlanmış ve sınanmıştır. RMS, aşağıdaki ölçütlere uyan diğer veritabanı sunucularında da çalışabilir:
  
-   Microsoft .NET Framework 1.1 tarafından sağlanan ADO.NET arabirimlerini desteklemelidir.  
-   Microsoft SQL Server'ın kullandığı yapılandırılmış sorgu dili olan Transact-SQL ile uyumlu olmalıdır, çünkü RMS başlatma komut dosyaları ve depolanmış RMS yordamları Transact-SQL kullanır.  
-   Microsoft SQL Server'a özgü tüm uzantıları desteklemelidir.  
-   .NET Framework'ün System.Data.SqlClient alanının yöntem çağrılarına yanıt verebilmelidir.  
-   System.Data.SqlClient ad alanı ile ilişkili işlevsellik sağlamalıdır.  
-   Windows Kimlik Doğrulaması Modu'nu kullanmalıdır.
  
Veritabanı sunucusunun yukarıdaki ölçütleri karşılayıp karşılamadığını öğrenmek için, ilgili veritabanının satıcısına başvurun.
  
Aşağıdaki tabloda, RMS ile farklı etkinlikler gerçekleştirmek için gereken kullanıcı hakları ve izinleri listelenmiştir.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Etkinlik</th>
<th style="border:1px solid black;" >Hesap gereksinimleri</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS'yi yükleme</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS kök kümesi sağlama</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı ve Active Directory arama ve yazma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS lisans kümesi sağlama</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı ve Active Directory araması</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Yeni bir yapılandırma veritabanı kullanırken sağlama</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı ve SQL Server çalışan bilgisayarda okuma, yazma ve oluşturma</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Varolan bir yapılandırma veritabanını kullanırken sağlama</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı ve veritabanı sunucusunu çalıştıran bilgisayarda okuma ve yazma</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS'yi yönetme</td>
<td style="border:1px solid black;">Yerel bilgisayar yönetici kimlik bilgilerine sahip etki alanı kullanıcısı</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.note(WS.10).gif)Not                                                                                                                                                                                             |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Windows Server yapılandırması, Active Directory, Message Queuing, IIS ve dosya sistemleri hakkında daha fazla bilgi için, Windows Server 2003 TechCenter'a ([http://go.microsoft.com/fwlink/?LinkId=78135](http://go.microsoft.com/fwlink/?linkid=78135)) bakın. |
  
RMS'yi küme dağıtımında kullanıyorsanız, aşağıdaki tabloda listelenen öğeleri dikkate aldığınızdan emin olun.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Koşul</th>
<th style="border:1px solid black;" >Öneri</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS, çok sayıda masaüstü tarafından kullanılacak</td>
<td style="border:1px solid black;">RMS SP2 istemcisini yüklemek için Systems Management Server (SMS) veya Grup İlkesi kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Çok sayıda istemci isteği</td>
<td style="border:1px solid black;">İstekleri küme çapında dağıtmak için bir yük dengeleme sunucusu, Windows Server işletim sistemindeki Ağ Yük Dengeleme hizmetini veya donanım yük dengeleme özelliğini kullanın.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Extranet ve intranet isteklerine hizmet vermek için sanal IP adresi kullanan iki ağ bağdaştırıcısı</td>
<td style="border:1px solid black;">Sanal IP adresini extranete göstermek üzere yapılan Etki Alanı Adı Sistemi (DNS) kaydının, adresi intranet'e göstermek için de yapıldığından emin olun.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747637.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| DNS kaydı intranet için yapılmazsa, içeriden yapılan istemci lisans istekleri başarısız olur. DNS ayarlarını değiştiremiyorsanız, kümedeki her sunucunun ana bilgisayarlar tablosunu, küme URL'si kümenin sanal IP adresine eşlenecek şekilde değiştirebilirsiniz. DNS kaydı RMS sağlama işleminden önce yapılmalıdır. Hizmeti zaten sağladıysanız, sunucudan RMS'yi kaldırmalı ve sağlama işlemini yinelemelisiniz. |
  
#### Bu sürümde desteklenen istemciler
  
Hizmet paketi olmayan RMS istemcisi, RMS SP1 veya RMS SP2, Microsoft Windows 2000, Windows XP ve Windows Server 2003 çalıştıran herhangi bir bilgisayara yüklenebilir. Önceki Windows işletim sistemleri bu sürüm tarafından desteklenmez.
  
| ![](images/Cc747637.Caution(WS.10).gif)Dikkat                                                                |  
|-------------------------------------------------------------------------------------------------------------------------------------------|  
| Hizmet paketi olmayan RMS istemcisi kullanıyorsanız istemci, RMS SP1 sunucusu veya daha sonrakilere karşı çevrimiçi yayımlama kullanamaz. |
  
İşlev Değişiklikleri  
--------------------
  
RMS SP2'de pek çok yeni özellik bulunmaktadır:
  
-   [Ormanlar arasında gelişmiş grup genişletmesi](#bkmk_cif1)  
-   [Veritabanı günlüğü değişiklikleri](#bkmk_cif2)  
-   [Daha büyük sunucu toplu iş boyutları](#bkmk_cif3)  
-   [Microsoft SQL Server 2005 uyumluluğu](#bkmk_cif4)
  
<span id="BKMK_CIF1"></span>
#### Ormanlar Arasında Gelişmiş Grup Genişletmesi
  
#### Bu özellik ne yapıyor?
  
RMS'deki ormanlar arasında grup genişletmesi özelliği, RMS'nin Active Directory Evrensel grup üyeliğini, grup üyeliklerinin iki orman arasında çoğaltılmadığı farklı bir ormana genişletmesini sağlar. Bir ormandaki kullanıcı başka bir ormandaki kullanıcıya haklarla korunan içerik gönderdiğinde, RMS'de bir bulma işlemi gerçekleştirilerek kullanıcının içeriğe erişimi olduğu doğrulanır. Bu doğrulama işlemi, uzak ormanın RMS hizmet bağlantı noktasını (SCP) bulmak üzere LDAP sorgusu kullanılarak bir ormandan diğerine yönelik olarak gerçekleştirilir. Uzak ormanın SCP'si bulunduğunda, RMS hizmeti hesabı, grup genişletme kanalına bir istek gönderir. Bu istek, uzak ormana bir kullanıcının grup üyesi olup olmadığını sorar.
  
#### Bu özellik kimler içindir?
  
Bu yeni özellik, birden çok orman bulunan bir Active Directory ortamında Evrensel grup üyelikleri ormanlar arasında çoğaltılmayan RMS müşterilerine yöneliktir.
  
#### Bu değişiklik neden önemlidir?
  
Yeni orman güven genişletme protokolü, birden çok orman bulunan bir Active Directory ortamını dağıtan müşteriler için güvenilirliği artıracaktır.
  
#### Neler farklı şekilde çalışmaktadır?
  
RMS SP2 öncesinde, ormanlar arasında grup genişletmesi, .NET uzak çağrıları kullanılarak gerçekleştiriliyordu. Bu sürümde, ormanlar arasında grup genişletmesi protokolü, orman güveni grup genişletme kanalına yönelik SOAP/HTTP istekleri kullanılarak bir ASP.NET Web hizmetine dönüştürülmüştür.
  
| ![](images/Cc747637.note(WS.10).gif)Not                                                                                                                                                         |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Geri uyumluluk için, .NET uzak çağrıları RMS SP2'de hala desteklenmektedir. Ancak, ormanlar arasında grup genişletmesi özelliğinden tam olarak yararlanılabilmesi için, tüm RMS kümelerinde en azından RMS SP2 çalışmalıdır. |
  
#### RMS SP2'ye hangi ayarlar eklendi veya değiştirildi?
  
Yeni RMS grup genişletme kanalı, RMS SP2'de varsayılan olarak en güvenli ayarlarla yapılandırılarak yalnızca yerel RMS Service ve Administrators gruplarının erişimine izin verilir. Bir hesaba erişim izni vermek için, wwwroot\\\_wmcs\\GroupExpansion\\GroupExpansion.asmx adresinde bulunan grup genişletme kanalındaki erişim denetim listesini değiştirmelisiniz.
  
| ![](images/Cc747637.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                             |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Her bir Active Directory ormanındaki RMS hizmet hesabının, kümede bulunan tüm RMS sunucularındaki grup genişletme kanallarına erişimi olduğunu doğrulayın. Hesapların erişimi yoksa, grup genişletmesi başarısız olur. Alternatif olarak, her bir ormanda aynı hesabı oluşturup hesaplara aynı parolayı atayabilirsiniz. Bu durumda, grup genişletme kanalına tek bir hesap eklemeniz yeterli olacaktır. |
  
Message Queuing hizmetine gönderilemeyen hata iletileri konusunda bilgilendirilmeniz için RMS SP2'ye yeni olaylar eklenmiştir. Bu yeni olay günlükleri, bir ileti dijital olarak imzalanamadığında veya doğrulanamadığında sizi bilgilendiren olaylar içerir. Doğrulama sorunlarına örnek olarak hatalı biçimlendirilmiş bir ileti, eksik veya hatalı bir karma ya da imza gösterilebilir.
  
<span id="BKMK_CIF2"></span>
#### Veritabanı Günlüğü Değişiklikleri
  
#### Bu özellik ne yapıyor?
  
RMS, tüm RMS iletişimini Message Queuing kullanarak günlük veritabanına gönderen bir günlük dinleyici hizmeti kullanır. RMS kümesi iletileri Message Queuing hizmetine gönderir ve günlük dinleyici hizmeti de bu iletileri Message Queuing sırasından alarak günlük veritabanına yazar.
  
#### Bu özellik kimler içindir?
  
Bu özellik, RMS günlük dinleyici hizmetini kullanan mevcut RMS kullanıcıları ve RMS günlük dinleyici hizmetini kullanmayı düşünen yeni RMS SP2 kullanıcılarına yöneliktir.
  
#### Bu değişiklik neden önemlidir?
  
RMS'nin önceki sürümlerinde, RMS günlük sırası, erişim denetim listeleri kullanılarak korunuyordu; ancak kimlik doğrulaması etkin değildi. Kimlik doğrulaması gerçekleştirilmediği için, kötü amaçlı bir kullanıcı RMS Günlüğü sırasına hatalı iletiler yazabilirdi.
  
#### Neler farklı şekilde çalışmaktadır?
  
RMS SP2'de, RMS kümesi tarafından Message Queuing kullanılarak gönderilen iletiler için ek kimlik doğrulaması gerçekleştirilir. İleti sırasına yetkisiz erişimi engelleyen erişim denetim listelerinin yanı sıra, bir ileti orijinalliği doğrulama düzeneği kullanılarak Message Queuing sırası da korunur. Message Queuing hizmetine bir ileti gönderildiğinde, RMS kanalları iletinin karmasını oluşturur ve RMS kümesinin özel anahtarını kullanarak iletiyi dijital olarak imzalar. Günlük Dinleyici Hizmeti ilk olarak iletinin kendi karmasını hesaplar ve bu değeri iletinin içerdiği karma ile karşılaştırır. Karma değerleri aynıysa, Günlük Dinleyici Hizmeti daha sonra kümenin ortak anahtarını ve iletideki karma değerini kullanarak imzayı doğrular. Karma değerleri aynıysa ve imza doğrulanırsa, ileti, günlük veritabanına gönderilir. Doğrulama adımları başarılı olmazsa, ileti Message Queuing sırasından kalıcı olarak silinir ve Olay Görüntüleyicisi'ndeki Uygulama günlüğüne bir olay uyarısı yazılır.
  
#### RMS SP2'ye hangi ayarlar eklendi veya değiştirildi?
  
Message Queuing hizmetine gönderilemeyen hata iletilerini belirtecek biçimde tasarlanmış yeni olaylar RMS SP2'ye eklenmiştir. Bu yeni olaylar Uygulama günlüğüne yazılır ve dijital olarak imzalanamayan veya dijital imzaları doğrulanamayan iletileri içerir. Doğrulama sorunlarına örnek olarak hatalı biçimlendirilmiş bir ileti, eksik veya hatalı bir karma ya da imza gösterilebilir.
  
<span id="BKMK_CIF3"></span>
#### Daha Büyük Sunucu Toplu İş Boyutları
  
#### Bu özellik ne yapıyor?
  
RMS'deki toplu iş uygulaması, her lisans için bağımsız bir istek göndermek yerine, birden çok isteğin tek bir istek olarak RMS kümesine gönderilebilmesini sağlayarak performansı artırır.
  
#### Bu özellik kimler içindir?
  
Daha büyük sunucu toplu iş boyutları desteği, haklarla korunan içerik için aynı anda birden çok lisans edinmesi gereken RMS etkin uygulamalar içindir.
  
#### Bu değişiklik neden önemlidir?
  
RMS toplu iş uygulaması, AcquireLicense RMS kanalına tek bir istek yayımlayarak bir veya daha fazla Yayımlama Lisansı'na göre birden çok Hak Hesabı Sertifikası (RAC) için Kullanım lisansı edinilebilmesini sağlar. Toplu iş boyutu 1'den büyük değilse, RMS etkin uygulamanın her bir kullanıcı için ayrı bir Kullanım lisansı istemesi gerekir.
  
#### Neler farklı şekilde çalışmaktadır?
  
RMS SP2 öncesi sürümlerde, RMS kümesi en fazla 1 toplu işi destekliyordu. En fazla boyut 1'den daha büyük bir sayıya ayarlandığında, küme bu sayıyı yok sayıyordu. RMS SP2 ile birlikte, en fazla toplu iş boyutu 100'e kadar artırılabilir.
  
| ![](images/Cc747637.note(WS.10).gif)Not      |  
|---------------------------------------------------------------------------|  
| Yalnızca AcquireLicense RMS kanalı toplu iş istekleri için destek içerir. |
  
RMS SP2'de, toplu iş istekleri de göz önüne alınarak hata bildirimi geliştirilmiştir. Örneğin, on isteği toplu iş olarak gönderirseniz ve ikinci ve üçüncü istekler başarısız olursa, her başarısız olan istek için olay günlüğüne bir olay yazılır.
  
<span id="BKMK_CIF4"></span>
#### Microsoft SQL Server 2005 Uyumluluğu
  
#### Bu özellik ne yapıyor?
  
RMS SP2'de, Microsoft SQL Server 2005 veritabanı sunucusu olarak kullanılarak, ek bir yapılandırmaya gerek kalmadan RMS yapılandırma ve günlük veritabanları desteklenebilir.
  
#### Bu özellik kimler içindir?
  
RMS SP2 ile birlikte Microsoft SQL Server 2005 desteği, RMS veritabanı olarak Microsoft SQL Server 2005 kullanmak isteyen müşterilere yöneliktir.
  
#### Bu değişiklik neden önemlidir?
  
RMS'nin önceki sürümlerinde, sysmessages tablosunda kullanılan bazı parametrelerin veri türleri Microsoft SQL Server 2005 biçim belirtimiyle uyumlu değildi. Daha fazla bilgi için, Microsoft Bilgi Bankası'ndaki 913372 numaralı makaleye bakın ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)).
  
#### Neler farklı şekilde çalışmaktadır?
  
RMS SP2'den önceki sürümlerde, SQL RAISERROR deyimleri yalnızca RMS kullanıcısı bir hata oluştuğu konusunda bilgilendirmek için kullanılıyordu. RAISERROR deyimi sysmessages tablosunu sorgulayarak, bu tabloda depolanan RMS hata iletilerini alır. RMS SP2, SQL hatalarını doldurmak için farklı bir teknik kullanır; bu nedenle, sysmessages tablosuna artık bağımlı değildir.
  
| ![](images/Cc747637.note(WS.10).gif)Not                                                                                                                                                                                        |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| RMS SP1'den RMS SP2'ye yükseltiyorsanız, sysmessages tablosu artık hata iletileri için sorgulanmaz; ancak hata iletileri, sysmessages tablosunda saklanmaya devam eder. RMS SP2'nin temiz yüklemesi sysmessages tablosundaki yeni girdileri eklemeyecektir. |
  
Bilinen Sorunlar  
----------------
  
Aşağıdaki bölümlerde, bu RMS sürümüyle ilgili bilinen sorunlar belirtilmektedir.
  
#### Yardım dosyasında hala RMS Service Pack 1'e başvuruluyor
  
RMS SP2 yüklemesinin içerdiği yardım dosyası RMS SP1'e başvurmaya devam etmektedir. RMS SP2 hakkında bilgi için, Rights Management Services'e ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) bakın.
  
#### Windows Update, RMS SP2 istemcisi x64 tabanlı veya Itanium tabanlı bilgisayarlara yüklenemiyor
  
RMS veya RMS SP1 istemcisi x64 tabanlı bir bilgisayara yüklenirse ve istemciyi Windows Update sitesinden RMS SP2 istemcisine (x64) yükseltmeye çalışırsanız, yükleme başarısız olur. RMS istemcilerinin 32-bit sistemler için geliştirilen önceki sürümleri x64 tabanlı bilgisayarlarda çalışıyordu, ancak RMS SP2 istemcisine (x64) yükseltilemezler. Önceki RMS istemcisini kaldırdıktan sonra güncelleştirmeyi yeniden başlatmanız gerekir. Windows Update, işletim sistemi sürümünü algılar ve uygun RMS SP2 istemcisini önerir. Aynı durum Itanium tabanlı bilgisayarlar için de geçerlidir.
  
#### Yeniden sağlama işlemi hiçbir zaman günlük dinleyici hizmetini başlatamıyor
  
Kümenin sağlaması kaldırıldığında, günlük dinleyici hizmeti, bu hizmeti Durduruldu durumunda bırakamaz. Hizmetin tümüyle durdurulması için bilgisayarı yeniden başlatmalısınız.
  
#### Güvenilen yayımlama etki alanı yazılım tabanlı değilse kaldırılamıyor
  
Yazılım tabanlı olmayan bir özel anahtar uygulamasıyla alındıktan sonra, güvenilen yayımlama etki alanı silinemez. Yazılım tabanlı olmayan bir özel anahtarı alma işlemi, Windows Rights Management Services Yönetim Konsolu'ndan yapılmamalıdır. Özel anahtarı alma ve verme konusunda yönergeler için uygun donanım sağlayıcısına başvurun.
  
#### Microsoft .NET Framework 2.0, RMS sunucusuna yüklendiğinde IIS sanal köklerini değiştiriyor
  
RMS SP2, .NET Framework sürüm 1.1 ile sağlanan ASP.NET komut dosyası eşlemesini kullanır. Sonraki sürümlerde sağlanan eşleme RMS SP2 ile uyumlu değildir. Ancak, her iki sürüm, diğer bağımlı uygulamaları engellemeden birlikte bulunabilir. Sunucunuzda .NET Framework 1.1 ve .NET Framework 2.0 veya daha sonraki sürümü yüklüyse, RMS SP2 yükleme ve sağlama işlemlerinin başarılı bir şekilde tamamlanmasından sonra RMS kümesi düzgün çalışmayabilir. Bunun nedeni, RMS sanal köklerinin ASP.NET komut dosyası eşleme 2.0 sürümü yerine 1.1 sürümü ile kaydettirilmesi gerekmesidir. RMS sanal köklerini ASP.NET komut dosyası eşleme 1.1 sürümüyle kaydettirmek için, komut isteminde aşağıdaki komutu çalıştırın:
  
**%windir%\\Microsoft.NET\\Framework\\v1.1.4322&gt;aspnet\_regiis.exe -s W3SVC/1/ROOT/\_wmcs**
  
Bu komutu çalıştırmak, RMS sanal köklerini düzgün bir şekilde kaydettirir ve RMS SP2'nin sunucuda çalışmasını sağlar.
  
#### Active Directory Windows 2000 Özgün işlev düzeyi kullanılırsa grup üyeliği kaybolabilir
  
Active Directory alt yapı düzeyleri Windows 2000 özgün işlev düzeyine yükseltilmiş bir ortamda RMS'yi dağıtırken, RMS, gizli dağıtım listelerinin grup üyeliğini genişletmeye çalıştığında Active Directory nesnelerinin memberOf özniteliğini okuyamayabilir. RMS'nin memberOf özniteliğini okumasını sağlamak için RMS Hizmeti hesabı, pre-Windows 2000 Compatible Access grubunun üyesi olan bir etki alanı hesabı kullanmalıdır. Daha fazla bilgi için, bkz: Microsoft Bilgi Bankası makalesi 812841 ([http://go.microsoft.com/fwlink/?LinkId=78152](http://go.microsoft.com/fwlink/?linkid=78152)).
  
#### Günlük dinleyici hizmeti, veritabanı erişilebilir olduğunda Message Queuing iletilerini Eski İleti Sırası'na gönderir.
  
Günlük dinleyici hizmetinin veritabanına ulaşamadığı durumlar olabilir (örneğin, veritabanı çalışır durumda değildir ya da ağ bağlantı sorunları olabilir). Bu durumda, iletiler bir Eski İleti Sırası'na gönderilir. Bu iletileri kurtarmanın (yani, günlük veritabanına göndermenin) tek yolu, RMS Yönetim Araç Seti ile birlikte gelen RMS Sıra Kurtarma aracını kullanmaktır. RMS Yönetim Araç Seti'ni karşıdan yüklemek için, bkz: [http://go.microsoft.com/fwlink/?LinkId=33841](http://go.microsoft.com/fwlink/?linkid=33841).
  
| ![](images/Cc747637.note(WS.10).gif)Not                                                                                                                                                           |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Recover ve RecoverandPurge öğeleri LogRecoveryCmd'den kaldırılmıştır. Böylece, tüm iletilerin günlük veritabanına gönderilmeden önce Message Queuing hizmeti üzerinden yönlendirilmesi ve kimliklerinin doğrulanması sağlanır. |
  
#### Microsoft SQL Server 2005'ten önce RMS SP2'yi yükseltmelisiniz
  
RMS SP2'ye ve Microsoft SQL Server 2000'den Microsoft SQL Server 2005'e yükseltirken, ilk olarak RMS'yi yükseltin. Böylece, Microsoft SQL Server yükseltmesiyle ilgili uyumluluk sorunları engellenebilir.
  
#### RMS SP2, adında kesme işareti (') bulunan Web sitelerinde sağlanamıyor
  
RMS SP2'yi adında kesme işareti (') bulunan bir Web sitesinde sağlamaya çalışırsanız, sağlama işlemi **Geçersiz parametre** hata iletisini vererek başarısız olur. RMS SP2'yi Web sitesinde sağlamak için, Web sitesinin adındaki kesme işaretini kaldırın.
  
#### Windows Server 2003 64 bit sürümünü çalıştıran sunucularda ASP.NET 1.1 sürümünü etkinleştirme
  
RMS Yardımı'ndaki "Sistem Gereksinimleri" konusunda, .NET Framework 1.1'in nasıl yükleneceği ve Internet Information Services (IIS) yüklendikten sonra ASP.NET 1.1'in nasıl çalıştırılacağı hakkında ayrıntılı bilgiler sağlanır. Ancak IIS'yi yüklemeden önce .NET Framework 1.1'i yüklerseniz, ASP.NET 1.1 Web hizmeti uzantılarında listelenmeyecektir ve belgede verilen yordam yararlı olmayacaktır. IIS'yi .NET Framework 1.1 yüklemesinden sonra yüklediyseniz, ASP.NET'i etkinleştirmek için komut isteminde aşağıdaki komutu çalıştırın:
  
**%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis.exe -i –enable**
  
.NET Framework'ün 1.1'den sonraki bir sürümünü kullanırken, varolan IIS komut dosyası eşlemelerini sıfırlamamak için bu komutta **-i** yerine **-ir** kullanın.
  
#### Uzak orman RMS hizmet hesabının yerel groupexpansion kanalına eklenmesi gerekiyor
  
BUILTIN\\users öğesini groupexpansion kanalındaki ACL'den kaldıran bir güvenlik sorunu giderilmiştir. Bu, ormanlar arasında grup genişletmesi senaryolarını geçersiz kılabilir. Bu sorunu gidermek için, aşağıdaki adımları tamamlayın:
  
**RMS hizmet hesabını uzak ormana ekleme**  
1.  Orman1'de (burada Orman1, ilk ormandaki RMS kök kümesidir) inetpub\\wwwroot\\\_wmcs dizinine gidin.
  
2.  **GroupExpansion** klasörünü sağ tıklatın ve sonra da **Özellikler**'i tıklatın.
  
3.  **GroupExpansion Özellikleri** penceresinde, **Güvenlik** sekmesini tıklatın, *Orman2\\RmsHizmetHesabı* girdisini (örneğin, rmil31\\rmsvc) ekleyin; burada Orman2, ikinci ormandaki RMS kök kümesidir.
  
4.  **Tamam**'ı tıklatın.
  
5.  **Çalıştır**'ı tıklatın, **iisreset** yazın ve**Tamam**'ı tıklatın.
  
#### .NET Framework'ü yükseltmek veri kaybına neden olabilir
  
RMS yüklenip sağlaması yapıldıktan sonra .NET Framework (CLR) 1.1 sürümü yükseltilirse, vroots, .NET Framework 2.0 sürümünü kullanacak biçimde ayarlanır. Bu durumda, günlük veritabanına hiçbir bilgi kaydedilmez. Bu da veri kaybına neden olur. Aşağıdaki eylemlerden birini gerçekleştirin:
  
-   RMS'yi yükleyip sağlamasını yapmadan önce .NET Framework'ü yükseltin.  
-   vroots'u, .NET Framework yükseltildikten sonra 1.1 sürümünü kullanacak biçimde sıfırlayın.
  
Bu sürümdeki belge değişiklikleri  
---------------------------------
  
Aşağıda, bu sürümde değiştirilen konuların listesi yer almaktadır:
  
-   Passport Tabanlı Hak Hesabı Sertifikalarına Güvenmek için ([http://go.microsoft.com/fwlink/?LinkId=70369](http://go.microsoft.com/fwlink/?linkid=70369))  
-   RMS için Yazılım Gereksinimleri ([http://go.microsoft.com/fwlink/?LinkId=70371](http://go.microsoft.com/fwlink/?linkid=70371))  
-   RMS İstemcisi Nasıl Dağıtılır? ([http://go.microsoft.com/fwlink/?LinkId=70373](http://go.microsoft.com/fwlink/?linkid=70373))  
-   RMS Komut İstemi Yüklemesi ([http://go.microsoft.com/fwlink/?LinkId=70374](http://go.microsoft.com/fwlink/?linkid=70374))  
-   RMS Çekirdek Yapılandırma Veritabanı Tabloları ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70375))  
-   RMS Yapılandırma Veritabanı Sertifika Tabloları ([http://go.microsoft.com/fwlink/?LinkId=70376](http://go.microsoft.com/fwlink/?linkid=70376))  
-   RMS Günlük Veritabanı Tabloları ([http://go.microsoft.com/fwlink/?LinkId=70377](http://go.microsoft.com/fwlink/?linkid=70377))  
-   Ölçeklendirme Gereksinimlerini Değerlendirme [http://go.microsoft.com/fwlink/?LinkId=70378](http://go.microsoft.com/fwlink/?linkid=70378))  
-   RMS Dağıtımının Güvenliğini Sağlama ([http://go.microsoft.com/fwlink/?LinkId=70379](http://go.microsoft.com/fwlink/?linkid=70379))  
-   Yetki Alma Hizmetini Etkinleştirme ([http://go.microsoft.com/fwlink/?LinkId=70380](http://go.microsoft.com/fwlink/?linkid=70380))  
-   Dış RMS Kullanıcıları için Planlama [http://go.microsoft.com/fwlink/?LinkId=70381](http://go.microsoft.com/fwlink/?linkid=70381))  
-   Mobil Aygıtlar ve Sunucu Hizmetleri için RMS Sunucusu Desteğini Etkinleştirme ([http://go.microsoft.com/fwlink/?LinkId=70382](http://go.microsoft.com/fwlink/?linkid=70382))
  
#### Telif Hakkı
  
*Bu belgedeki bilgiler, belirtilen sorunlara yönelik olarak, Microsoft Corporation'ın belgenin yayımlandığı tarihteki görüşlerini gösterir. Microsoft'un değişen piyasa koşullarına yanıt vermesi gerektiğinden, bu belgenin Microsoft'un bir taahhüdü olarak yorumlanmaması gerekir; Microsoft, belge yayımlandıktan sonra sunulan bilgilerin doğruluğunu garanti edemez.*
  
*Bu belge yalnızca bilgi verme amaçlıdır. MICROSOFT BU BELGEDEKİ BİLGİLER İÇİN AÇIK, ZIMNİ VEYA YASAL HİÇBİR GARANTİ VERMEZ.*
  
*Tüm geçerli telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakları kapsamındaki haklar saklı kalmak kaydıyla, Microsoft Corporation'ın yazılı açık izni olmadan bu belgenin hiçbir bölümü herhangi bir biçimde, herhangi bir yöntemle (elektronik, mekanik, fotokopi, kayıt veya başka şekilde) veya herhangi bir amaçla çoğaltılamaz, aktarılamaz, bir geri alma sisteminde saklanamaz veya bu tür bir sisteme konamaz.*
  
*Bu belgeye konu olan malzemeye ilişkin olarak Microsoft'un patentleri, patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından yazılı bir lisans sözleşmesinde açıkça belirtilmediği sürece, bu belgeyi bulundurmak, size patent, ticari marka, telif hakkı ve diğer fikri mülkiyet haklarını kullanma yetkisi vermez.*
  
*Aksi belirtilmediği sürece, örneklerde adı geçen şirketler, kuruluşlar, ürünler, etki alanı adları, e-posta adresleri, logolar, kişiler, yerler ve olaylar hayal ürünüdür ve hiçbir gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla ilgili olarak kullanılmaları veya böyle bir sonuç çıkarılması amaçlanmamıştır.*
  
*© 2006 Microsoft Corporation. Tüm hakları saklıdır.*
  
*Active Directory, Microsoft, MS-DOS, Visual Studio, Windows, Windows Server, SQL Server ve Windows NT, Microsoft Corporation'ın ABD'de ve/veya diğer ülkelerdeki kayıtlı ticari markaları veya ticari markalarıdır.*
  
*Burada sözü edilen gerçek şirketler ve ürünler, ilgili firmaların ticari markaları olabilir.*
