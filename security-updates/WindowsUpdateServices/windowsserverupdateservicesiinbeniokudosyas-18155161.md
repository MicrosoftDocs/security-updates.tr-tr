---
TOCTitle: Windows Server Update Services için BeniOku Dosyası
Title: Windows Server Update Services için BeniOku Dosyası
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18155161
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720505(v=WS.10)'
---

Windows Server Update Services için BeniOku Dosyası
===================================================

Bu belgede, Windows Server Update Services'ı (WSUS) etkilediği bilinen sorunlar açıklanır. Ayrıca, WSUS'u yüklemeye yönelik öneriler ve gereksinimlere yer verilir.

| ![](images/Cc720505.note(WS.10).gif)Not                                                                                                                            |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu belgenin karşıdan yüklenebilir bir kopyası Microsoft Yükleme Merkezi'nde [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126) adresinde bulunabilir. |

Başlamadan Önce
---------------

#### Sorun 1: IIS yüklü olmalıdır

Microsoft® Windows Server™ Update Services (WSUS), Internet Information Services'ın (IIS) yüklü olmasını gerektirir. Ancak, Microsoft Windows Server 2003 ve Microsoft Windows® 2000 Server'da, IIS varsayılan olarak yüklü değildir; bu nedenle, Windows Server Update Services Setup devam edemeyebilir ve IIS'nin yüklü olmadığını bildiren bir hata iletisi görüntülenebilir.

IIS'yi yüklemek için:

1.  Denetim Masası'nı açın.
2.  **Program Ekle veya Kaldır**'ı çift tıklatın.
3.  **Windows Bileşenlerini Ekle/Kaldır**'ı tıklatın.
4.  **Bileşenler** listesinde, **Uygulama Sunucusu**'nu tıklatın.
5.  **Ayrıntılar**'ı tıklatın.
6.  **ASP.NET** onay kutusunu seçin. **network COM+ access** seçeneğini etkinleştirdiğinizde, Internet Information Services (IIS) otomatik olarak seçilir.
7.  **Internet Information Services (IIS)** seçeneğini belirleyin ve sonra da **Ayrıntılar**'ı tıklatarak IIS isteğe bağlı bileşenlerinin o listesini görüntüleyin.
8.  Yüklemek istediğiniz tüm isteğe bağlı bileşenleri seçin. World Wide Web Hizmeti isteğe bağlı bileşeni, Active Server Pages bileşeni ve Uzaktan Yönetim (HTML) gibi önemli alt bileşenler içerir. Bu alt bileşenleri görüntülemek ve seçmek için, World Wide Web Hizmeti'ni ve ardından Ayrıntılar'ı tıklatın. Windows Bileşen Sihirbazı'na dönünceye kadar Tamam'ı tıklatın.
9.  **İleri**'yi tıklatın ve Windows Bileşen Sihirbazı'nı tamamlayın.
10. IIS'yi yükledikten sonra, Windows Server Update Services Setup'ı çalıştırın.

#### Sorun 2: Windows 2000 Server çalışan sunuculara WSUS yüklenebilmesi için, en az bir Web sitesinin IIS'de bulunması gerekir

Windows Server Update Services Setup çalıştırıldığında IIS'de hiçbir site yoksa, Setup bir Web sitesi oluşturamayabilir. Bu, örneğin IIS'deki tek siteniz bir Software Update Services (SUS) 1.0 sitesiyse ve WSUS'u yüklemeden önce bu siteyi silerseniz oluşabilir.

Bu durumda, Internet Information Services (IIS) Yöneticisi ek bileşenini kullanarak yeni bir Web sitesi oluşturmanız gerekir. Bunu yaptıktan sonra, WSUS Setup sırasında bu siteyi seçebilir veya yeni bir site belirtebilirsiniz.

WSUS'u yüklemeye çalıştığınızda hiçbir site olmadığı için Setup başarısız olduysa, IIS Yöneticisi ek bileşenini açın ve "Web Sitesi \#1" adlı siteyi silin. Daha sonra, yukarıda açıklanan adımları uygulayarak Setup'ı yeniden çalıştırın.

#### Sorun 3: Gerekli bileşenleri yükleme

#### Yazılım gereksinimleri

Aşağıdaki tabloda, desteklenen her bir işletim sistemi için gerekli yazılımlar gösterilmektedir. WSUS Setup'ı çalıştırmadan önce, WSUS sunucusunun bu gereksinimler listesine uygun olduğunu doğrulayın. Bu güncelleştirmeden biri yükleme tamamlandığında bilgisayarın yeniden başlatılmasını gerektiriyorsa, yeniden başlatma işlemini, WSUS'u yüklemeden önce gerçekleştirmelisiniz.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >İşletim Sistemi</th>
<th style="border:1px solid black;" >Gereksinimler</th>
<th style="border:1px solid black;" >Yüklemeler</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Tüm işletim sistemleri</td>
<td style="border:1px solid black;">Microsoft Internet Information Services (IIS) 5.0</td>
<td style="border:1px solid black;">İşletim sisteminden yükleyin.
Bkz: Sorun 1: IIS yüklü olmalıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Tüm işletim sistemleri</td>
<td style="border:1px solid black;">Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0</td>
<td style="border:1px solid black;">Windows Server 2003 işletim sistemleri için, Microsoft Yükleme Merkezi'ndeki <a href="http://go.microsoft.com/fwlink/?linkid=47251">Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0 ve WinHTTP 5.1 Windows Server 2003 Güncelleştirmesi</a> (KB842773) sayfasına bakın (http://go.microsoft.com/fwlink/?LinkId=47251).
Windows Server 2000 işletim sistemleri için, Microsoft Yükleme Merkezi'ndeki <a href="http://go.microsoft.com/fwlink/?linkid=46794">Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0 ve WinHTTP 5.1 Windows Server 2000 Güncelleştirmesi</a> (KB842773) sayfasına bakın (http://go.microsoft.com/fwlink/?LinkId=46794).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1</a>
Alternatif olarak, <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> sitesine giderek Kritik Güncelleştirmeler ve Hizmet Paketlerini tarayın; Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1'i yükleyin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft SQL ile %100 uyumlu veritabanı yazılımı</td>
<td style="border:1px solid black;">Yok</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft SQL ile %100 uyumlu veritabanı yazılımı</td>
<td style="border:1px solid black;">Microsoft SQL Server 2000 kullanmıyorsanız, Microsoft SQL Server 2000 Desktop Engine'i (MSDE 2000) yükleyebilirsiniz. Bu işlem için birkaç adım gerçekleştirilmesi gerekir. Daha fazla bilgi için, aşağıdaki Windows 2000'e MSDE Yükleme bölümüne bakın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft Internet Explorer 6.0 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework Sürüm 1.1 Yeniden Dağıtılabilir Paketi</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework Sürüm 1.1 Yeniden Dağıtılabilir Paketi</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Alternatif olarak, <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> sitesine giderek Kritik Güncelleştirmeler ve Hizmet Paketlerini tarayın; Windows Server 2000 için Microsoft .NET Framework 1.1 Service Pack 1'i yükleyin.</td>
</tr>
</tbody>
</table>
 

Bu gereksinimlerin yanı sıra, WSUS, gerekirse sunucunuza ASP.NET 1.1 sürümünü de yükleyebilir veya bu sürümü yapılandırabilir. (WSUS Setup, ASP.NET'i yapılandırır.)

#### Windows 2000'e MSDE Yükleme

WSUS için Windows 2000 kullanıyorsanız ve Microsoft SQL Server 2000'e erişiminiz yoksa, WSUS Setup'ı çalıştırmadan önce Microsoft SQL Server 2000 Desktop Engine'i (MSDE) yüklemelisiniz. WSUS sunucunuzda MSDE zaten yüklüyse, WSUS için özel bir örneğini kurmanız gerekmez. WSUS kurulumu sırasında varolan örneğin adını belirtmeniz yeterlidir.

Windows 2000 Server'a MSDE dört adımda yüklenebilir. İlk olarak, MSDE arşivini karşıdan yüklemeniz ve WSUS sunucunuza genişletmeniz gerekir. Daha sonra, bir komut isteminde komut satırı seçeneklerini kullanarak MSDE Setup'ı çalıştırın, sa parolasını ayarlayın ve örnek adı olarak WSUS atayın. Ardından, MSDE yüklemesi tamamlandığında, WSUS örneğinin bir NT hizmeti olarak çalıştığını doğrulamalısınız. Son olarak, WSUS sunucunuzu korumak için MSDE'ye bir güvenlik paketi eklemeniz gereklidir.

#### Adım 1: MSDE arşivini karşıdan yükleme ve genişletme

MSDE arşivini karşıdan yüklemeniz ve WSUS sunucunuza genişletmeniz gerekir. Bkz: [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Adım 2: MSDE'yi yükleme

Komut isteminde komut satırı seçeneklerini kullanarak MSDE Setup'ı çalıştırın, sa parolasını ayarlayın ve örnek adı olarak WSUS atayın. MSDE yüklemesi tamamlandığında, WSUS örneğinin bir NT hizmeti olarak çalıştığını doğrulamalısınız.

MSDE'yi yüklemek için, sa parolasını ayarlayın ve bir örnek adı atayın:

1.  Komut isteminde, “Adım 1: MSDE arşivini karşıdan yükleme ve genişletme” bölümünde belirtilen MSDE yükleme klasörüne gidin.
2.  Aşağıdakini yazın: **setup sapwd="***parola***" instancename=WSUS**
    Burada *parola*, MSDE'nin bu örneğinde sa hesabı için bir güçlü parola ve **instancename** parametresi de veritabanı örneğinin adıdır. Alternatif olarak, WSUS veritabanınız için varsayılan örnek adını ("WSUS" yerine) kullanabilirsiniz. Bunu yaparsanız, komut satırı parametrenizde **instancename=WSUS** yazmanız gerekmez. Bu komut, MSDE kurulum programını başlatır, sa parolasını ayarlar ve MSDE'nin bu örneğini belirttiğiniz değer olarak adlandırır.

#### Adım 3: MSDE'nin WSUS örneğinin yüklü olduğunu doğrulama

MSDE'nin WSUS örneğini gördüğünüzden emin olmanız gerekir.

1.  **Başlat**'ı ve sonra **Çalıştır**'ı tıklatın.
2.  **Aç** kutusuna **services.msc** yazın ve **Tamam**'ı tıklatın.

Hizmetler listesini aşağı kaydırın ve (örnek adı olarak "WSUS" kullandıysanız) MSSQL$WSUS veya (varsayılan örnek adını kullandıysanız) MSSQLSERVER adlı bir hizmetin bulunduğunu doğrulayın.

#### Adım 4: MSDE örneğini başlatın.

MSDE yüklemesinin sonunda, örneği başlatmanız gerekir. Örnek adı olarak "WSUS" kullandıysanız, "MSSQL$WSUS" hizmetini başlatırsınız. Varsayılan örnek adını kullandıysanız, MSSQLSERVER hizmetini başlatırsınız. Bu hizmet başlatılmazsa, WSUS, veritabanı örneğini kullanamaz.

#### Adım 5: MSDE'yi güncelleştirin.

[MS03-031 bülteninde tanımlanan güvenlik güncelleştirmesini karşıdan yüklemeniz ve kurmanız gerekir: SQL Server İçin Toplu Düzeltme Eki](http://go.microsoft.com/fwlink/?linkid=47364) adlı bültende açıklanan güvenlik düzeltme ekini karşıdan yüklemeniz ve kurmanız gerekir.

Güvenlik güncelleştirmesini karşıdan yüklemek için, bkz. [SQL Server 2000 (32-bit) Güvenlik Düzeltme Eki MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Sorun 4: En az disk alanı gereksinimleri

Windows Server Update Services'ı yüklemek için en az disk alanı gereksinimleri aşağıdaki gibidir:

-   Sistem bölümünde 1 gigabayt (GB)
-   Veritabanı dosyalarının depolanacağı birimde 2 GB
-   İçerik izdüşüm sayılarına bağlı olarak 6 GB

#### Sorun 5: WSUS'un en son sürümü yüklenmeden önce, daha eski sürümleri Program Ekle veya Kaldır kullanılarak kaldırılmalıdır

Windows Update Services Beta 1 veya Beta 2'nin yüklü olduğu bir sunucuya Windows Server Update Services'ı yüklemeyi planlıyorsanız, öncelikle Denetim Masası'ndaki Program Ekle veya Kaldır'ı kullanarak önceki sürümünü kaldırmanız gerekir.

#### Sorun 6: WSUS, SQL Server'da iç içe tetikleyiciler seçeneğinin etkinleştirilmiş olmasını gerektirir

Bu seçenek varsayılan olarak etkindir; ancak, bir SQL Server yöneticisi tarafından devre dışı bırakılabilir.

Windows Server Update Services veri deposu olarak bir SQL Server veritabanı kullanmayı planlıyorsanız, WSUS yöneticisi WSUS'u yükleyip kurulum sırasında veritabanını belirtmeden önce, sunucudaki iç içe tetikleyiciler seçeneğinin etkinleştirilmiş olduğunun SQL Server yöneticisi tarafından doğrulanması gerekir.

WSUS Setup, veritabanına özgü bir seçenek olan RECURSIVE\_TRIGGERS seçeneğini etkinleştirir; ancak, bir sunucu genel seçeneği olan iç içe tetikleyiciler seçeneğini etkinleştirmez.

İç içe tetikleyicilerin etkin olup olmadığını görmek için aşağıdaki komutu kullanın:

**sp\_configure 'nested triggers'**

SQL Server'da iç içe tetikleyiciler seçeneğini etkinleştirmek için, SQL Server çalışan bilgisayarda bir toplu iş dosyasından aşağıdaki komutu çalıştırın:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Sorun 7: WSUS Setup komut satırı parametreleri

WSUS'un katılımsız yüklemesini gerçekleştirebilirsiniz. Daha fazla bilgi ve komut satırı parametreleri için, [Microsoft Windows Server Update Services'ı Dağıtma](http://go.microsoft.com/fwlink/?linkid=41777) belgesinde "Ek A: Katılımsız Yükleme" bölümüne bakın.

Bilinen Sorunlar
----------------

#### Sorun 1: IIS Kilitleme Sihirbazı

Windows 2000 Server çalışan bir bilgisayarda Internet Information Services (IIS) çalıştırıyorsanız, Microsoft TechNet'teki IIS Lockdown Aracı sayfasından IIS Lockdown Wizard'ın en son sürümünü (URLScan içerir) yükleyin. Microsoft, IIS sunucularınızın güvenliğini sağlamak için bu aracı yüklemenizi önerir. IIS Kilitleme Sihirbazı, güvenlik riski oluşma olasılığını azaltmak için IIS'nin gerek duyulmayan özelliklerini kapatma yöntemiyle çalışır.

| ![](images/Cc720505.note(WS.10).gif)Not                                                                                                                                  |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| WSUS Setup bu bileşenleri yüklemez. Bunları el ile yüklemelisiniz. Windows Server 2003 çalışan bilgisayarlara IIS Lockdown aracını yüklemeniz gerekmez, çünkü bu işlevsellik yerleşik olarak bulunur. |

#### Sorun 2: WSUS yapılandırmasının doğrudan veritabanından değiştirilmesi desteklenmez

Windows Server Update Services, yapılandırma verilerini bir veritabanında (MSDE veya SQL Server veritabanında) depolar. Ancak, doğrudan veritabanına erişilerek yapılandırma verilerinin değiştirilmesi desteklenmez. Yöneticiler WSUS yapılandırmasını bu yolla değiştirmeye çalışmamalıdır. WSUS yapılandırmanızı değiştirmenin yolu, WSUS konsolunu kullanmak veya WSUS API'lerini çağırmaktır.

#### Sorun 3: WSUS yönetim sitesine erişmek için Active komut dizileri etkinleştirilmiş olmalıdır

Yöneticinin iş istasyonunda, Internet Explorer'ı kullanarak WSUS yönetim sitesine erişebilmeniz için ilk olarak Internet Explorer'ı Active komut dizilerine izin verecek biçimde yapılandırmanız gerekir.

#### Sorun 4: WSUS Setup sırasında IIS yeniden başlatılır

Windows Server Update Services Setup, önceden bildirmeden IIS'yi yeniden başlatır. Bu, kuruluşunuzdaki varolan Web sitelerini etkileyebilir.

#### Sorun 5: WSUS veya SMS yönetim noktalarının (MP) sanal dizin erişimini değiştirme

Varsayılan olarak, Windows Server Update Services'ın içerik sanal dizinine erişim anonim olarak ayarlanır. Bu ayarı kimlik doğrulaması istenecek biçimde değiştirirseniz, istemciler kimlik doğrulama hatası alır ve güncelleştirmeleri karşıdan yüklemek üzere erişim girişimleri reddedilir. Bu, açık kimlik doğrulaması gerektiğinde Winhttp.dll dosyasının yanlış kimlik doğrulama bağlamını kullanması sonucu kimlik doğrulaması girişiminin başarısız olmasına neden olduğu bilinen bir sorundur. Bu sorunu engellemek için, WSUS sunucusunun ve SMS MP'lerin IIS sanal dizinlerine anonim erişim sağlayacak biçimde ayarlandığından emin olun.

#### Sorun 6: Windows Small Business Server 2003'e WSUS yüklerken, varsayılan Web sitesinin WSUS sanal kök dizini erişim ayarları, WSUS istemcilerinin kendilerini sunucudan güncelleştirmesine olanak verecek biçimde değiştirilmelidir.

WSUS Server, varsayılan Web sitesinin giriş dizini altına SelfUpdate ve ClientWebService adlı iki sanal kök dizini ve bazı dosyalar yükler (80 numaralı bağlantı noktasını kullanarak). Bu, istemcilerin varsayılan Web sitesi üzerinden kendilerini güncelleştirebilmelerini sağlar. Varsayılan olarak, Windows Small Business Server 2003'te, varsayılan Web sitesi sunucudakiler dışındaki bir IP veya localhost adresine erişimi reddedecek biçimde yapılandırılmıştır. Bu, SelfUpdate ve ClientWebService sanal kök dizinlerin erişimlerinin reddedileceği ve istemcilerin kendilerini güncelleştirmeyeceği anlamına gelir. Kendilerini güncelleştirecek istemcilere erişim izni atamak için, varsayılan Web sitesinin SelfUpdate ve ClientWebService sanal kök dizinlerinde aşağıdaki adımları tamamlayın.

1.  Sanal kök dizinde sırasıyla **Özellikler**'i, **Dizin Güvenliği**'ni, **IP adresi ve etki alanı adı sınırlamaları**'nı ve sonra da **Düzen**'i tıklatın.
2.  **Erişim İzni Verilsin**'i seçin ve **Tamam**'ı tıklatın. Tüm özellik sayfalarını kapatın.

#### Sorun 7: Small Business Server'a WSUS Yükleme - Tümleştirme Sorunları

-   Windows Small Business Server 2003 Internet'e erişmek için bir ISA proxy sunucu kullanıyorsa, **Ayarlar** kullanıcı arabirimine aşağıdaki değerlerin el ile girilmesi gerekir: proxy sunucu ayarları, proxy sunucu adı ve bağlantı noktası.
-   ISA'da Windows Kimlik Doğrulaması kullanılıyorsa, proxy sunucunun kimlik bilgileri "ETKİALANI\\kullanıcı" biçiminde girilmelidir (Kullanıcı, "Internet Users" grubunun üyesidir).

#### Sorun 8: Bilgisayar bir bilgisayar grubundan bir başkasına taşınırken, yeni grupta da yönetim konsolunda göründüğü gibi görünmesi için bir saat geçmesi gerekebilir

Bilgisayar bir hedef gruba ilk kez atandığında, bilgisayardaki veriler grup bilgileriyle değiştirilir. Bu veriler düzenli olarak veya saatte bir yenilenir. Bu nedenle, bilgisayarı bir bilgisayar grubundan bir başkasına taşıdığınızda, bu bilgilerin istemcide yenilenmesi ve WSUS yönetim konsolunda değişmiş olarak görüntülenmesi bir saat kadar zaman alabilir.

#### Sorun 9: WSUS'u bir üye sunucuya yükledikten sonra üye sunucuyu bir etki alanı denetleyicisi konumuna yükseltmek isterseniz, ilk olarak WSUS'u kaldırmalısınız

WSUS'u bir üye sunucuya yükledikten sonra üye sunucuyu bir etki alanı denetleyicisi konumuna yükseltmek isterseniz, aşağıdaki adımları izlemelisiniz:

1.  WSUS'u kaldırın.
2.  Sunucuyu bir etki alanı denetleyicisi konumuna yükseltin.
3.  WSUS'u yeniden yükleyin.

#### Sorun 10: WSUS Server'ı bir etki alanı denetleyicisi konumundan üye sunucusu konumuna indirgemek isterseniz, ilk olarak WSUS'u kaldırmalısınız

WSUS Server'ı bir etki alanı denetleyicisinde çalıştırıyorsanız ve etki alanı denetleyicisini bir üye sunucu konumuna indirgemek isterseniz, aşağıdaki adımları izlemelisiniz:

1.  Veritabanını koruyarak WSUS'u kaldırın.
2.  ASPNET adlı bir kullanıcı hesabı oluşturun.
3.  Komut istemine **aspnet\_regiis -i** yazın.
4.  WSUS'u yeniden yükleyin ve korunan veritabanını kullanın.

#### Sorun 11: WSUS yüklendikten sonra .NET Framework 1.0 veya 2.0 yüklenirse, WSUS yönetim konsolu görünmez

Bunun nedeni, .NET Framework 1.0'ın IIS ile kaydettirilmesi ve WSUS Server için .NET Framework 1.1 gerekmesidir. Bu sorunu gidermek için, aspnet\_regiis.exe dosyasını açın ve aşağıdaki komutları çalıştırın (burada *Web sitesi kimliği*, aşağıdaki kayıt defteri anahtarının içerdiği değerdir:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Web sitesi kimliği*&gt;\\ROOT\\Content

#### Sorun 12: Uzak SQL sınırlamaları

WSUS, geri kalan bilgisayarlardan farklı bir WSUS uygulamasındaki bilgisayarda veritabanı yazılımı çalıştırmak için sınırlı destek sağlar.

-   Bir uzak SQL çiftinde, ön uç bilgisayar olarak Windows 2000 Server'ı kullanamazsınız.
-   Etki alanı denetleyicisi olarak yapılandırılmış bir sunucuyu uzak SQL çiftinin ön uç veya arka uç sunucusu olarak kullanamazsınız.
-   Arka uç sunucusunda veritabanı yazılımı için WMSDE veya MSDE kullanamazsınız.
-   Uzak sunucuda Terminal Services yüklü ve uygulama modunda çalışıyorsa, uzak SQL Server (WSUS veritabanı olarak kullanılan) hata veriyor. Terminal Services sunucusuna SQL Server yüklerken, şunları yapmanız gerekir:
    1.  Kurulumu çalıştırmadan önce, bir komut istemi açın ve şu komutu yazın: **change user /install**
    2.  SQL Server Setup'ı çalıştırın.
    3.  Kurulumu çalıştırdıktan sonra, komut istemine şunu yazın: **change user /execute**
-   Uzak SQL Server WSUS veritabanını kurmak için, hem ön uç hem de arka uç bilgisayarda Local Administrators güvenlik grubunun üyesi olmalısınız.
-   Uzak SQL ile ilgili sorunlar hakkında daha fazla bilgi için, [Microsoft Windows Server Update Services'ı Dağıtma](http://go.microsoft.com/fwlink/?linkid=41777) belgesinde "Ek C: Uzak SQL" bölümüne bakın.

#### Sorun 13: Kopya aşağı akım sunucusu, ana yukarı akım sunucusundan daha az onaylanabilir

Kopya aşağı akım sunucusu, ana yukarı akım sunucusundan daha az onaylanabilir. Bunun nedeni, içeriğin yukarı akım sunucusuna karşıdan yüklenmesi tamamlanıncaya kadar yükleme onaylarının aşağı akım sunucusuna iletilmemesidir.

#### Sorun 14: Eşitleme başarısız olursa eşitlemeyi yeniden deneyin

Eşitleme başarısız olursa, bir hata iletisi alabilirsiniz. Bu durumda, önce eşitlemeyi denemeniz gereklidir.

#### Sorun 15: WSUS Administration konsoluna erişmeye çalıştığınızda, System.IO.FileNotFoundException hata iletisi görüntülenir

Aşağıdaki hata iletisini alırsanız, Network Service veya ASP.NET hesabındaki izinleri ayarlamanız gerekebilir:

System.IO.FileNotFoundException: *xxxxxx*.dll adlı dosya veya derleme ya da bağımlılıklarından biri bulunamadı

Burada *xxxx*, rasgele bir addır.

Windows Server 2003 işletim sistemlerinde bu sorunu gidermek için, Network Service hesabına %systemroot%\\Temp için okuma/yazma erişimi atayın. Windows 2000 Server'da, ASP.NET hesabına %systemroot%\\Temp için okuma/yazma erişimi atayın.

#### Sorun 16: SQL Güvenlik Güncelleştirmesi MS03-031 (KB815495)

Bu güncelleştirmeyi istemciye yükleme işlemi başarısız olsa da güncelleştirme WSUS sunucusunda yüklü olarak gösterilebilir Bu, paketin istemciye yeniden sunulmasına neden olur. Güncelleştirmeyi sunucuda onaylamayarak bu soruna geçici bir çözüm bulabilirsiniz.

#### Sorun 17: RTM yükseltmesi sırasında IIS ayarları kaybolur.

WSUS'un önceki bir sürümü (örneğin, RC) yüklü olan bir sunucuya WSUS RTM yüklerseniz, WSUS RTM önceki sürümü kaldırarak yeni sürümü yükler. Bu, IIS'deki WSUS ile ilişkili sanal kök dizinlerin ve dosyaların silineceği anlamına gelir.

WSUS'u varsayılan Web sitesine yüklediyseniz, WSUS sanal kök dizinlerinde belirlediğiniz WSUS ile ilgili ayarlar kaybolur. Örneğin, WSUS güvenliğini sağlamak üzere SSL için WSUS sanal kök dizinleri yapılandırdıysanız, WSUS'un RTM sürümünü yükledikten sonra bunları yeniden yapılandırmanız gerekir. Not: WSUS konsolunda SSL'nin etkinleştirilmediğine yönelik bir bildirim alırsınız.

WSUS'u varsayılan Web sitesi dışında bir Web sitesine yüklediyseniz, WSUS Web sitesi düzeyindeki tüm ek ayarlar kaybolur.

#### Sorun 18: Ana bilgisayar üstbilgilerini kullanma

IIS'de varsayılan Web sitesine (WSUS Web sitesine) ana bilgisayar üstbilgisi değerleri atamak isterseniz, varsayılan Web sitesindeki IP adresleri listesine ana bilgisayar üstbilgisi değeri olmadan “Tümü Atanmamış” veya atanmış bir IP adresi eklemelisiniz. Bu değer, varsayılan olmayan Web sitesine de eklenmelidir

**Uyarı**: Bu işlem Windows® SharePoint® Services ve Exchange işlevselliğini bozabilir.

#### Sorun 19: Internet Explorer güvenliğini artırmanın etkinleştirilmiş olduğu bilgisayarlarda, WSUS konsol URL'sinin Güvenilen siteler ve Yerel intranet Web içeriği bölgelerine eklenmesi gerekir

Bir bilgisayarda Internet Explorer güvenliğini artırma özelliği (Microsoft Windows Server 2003'te Internet Explorer Artırılmış Güvenlik Yapılandırması bileşeni olarak da bilinir) etkinleştirilmişse ve WSUS konsolunu Güvenilen siteler ve Yerel intranet Web içeriği bölgelerine eklemezseniz, WSUS konsolunda her sayfa açtığınızda kullanıcı kimlik bilgileri sorulur.

WSUS konsolunu **Yerel intranet** ve **Güvenilen siteler** Web içeriği bölgelerine eklemek için:

1.  **Internet Seçenekleri**'ni açın (örneğin, **Başlat**'ı tıklatın, **Denetim Masası**'nın üzerine gelin ve **Internet Seçenekleri**'ni tıklatın.
2.  **Güvenlik** sekmesinde, **Yerel intranet**'i tıklatın, **Siteler**'i tıklatın, **Gelişmiş**'i tıklatın, URL'yi ekleyin (http://*WSUSSunucuadı*/WSUSAdmin) ve sonra da **Tamam**'ı tıklatın.
3.  **Güvenilen siteler**'i tıklatın, **Siteler**'i tıklatın, WSUS konsolu URL'sini ekleyin, **Tamam**'ı tıklatın ve sonra yeniden **Tamam**'ı tıklatarak **Internet Seçenekleri**'nden çıkın.

#### Sorun 20: WSUS Sürüm Adayı'ndan yükseltme başarısız

WSUS Sürüm Adayı'ndan yükseltme kendi kendini güncelleştirme ağacı sorunu yüzünden başarısız olabilir. Siz yükseltmeyi denediğiniz anda birden fazla istemci kendini güncelleştirirse bu oluşabilir.

Bu sorunu çözmek için:

1.  İstemcilerin bağlanamayacağından emin olmak için, WSUS sunucusunun ağ ile bağlantısını kesin.
2.  Komut isteminde aşağıdakini yazın: **iisrestart /reset** ve ardından ENTER tuşuna basın.
3.  Yükseltmeyi çalıştırın.

#### Sorun 21: SUS 1.0'dan gelen bazı onaylar WSUS'ye geçiş yapamayabilir.

SUS 1.0'dan WSUS'ye geçiş yaparken, SUS 1.0 sunucusundaki bazı onaylar WSUS sunucusuna geçiş yapamayabilir. Bunun nedeni SUS 1.0 için kullanılabilir olan bazı güncelleştirmelerin WSUS için artık kullanılamaz olmasıdır. Bunun yanında WSUS, SUS'den daha fazla güncelleştirme desteklediği için, geçiş işlemi tamamlandıktan sonra WSUS sunucunuzda onaylanmamış önemli güncelleştirmeler olabilir.

Microsoft, SUS 1.0'dan geçiş yaptıktan sonra WSUS sunucunuzdaki onaylanmamış güncelleştirme grubunu gözden geçirmenizi kesinlikle önerir.

SUS 1.0'dan WSUS'ye geçiş yapma hakkında daha fazla bilgi için, http://go.microsoft.com/fwlink/?LinkId=48042 adresinden [Software Update Services'dan Windows Server Update Services'a Adım Adım Geçiş Kılavuzu](http://go.microsoft.com/fwlink/?linkid=48042) sayfasına bakın.

#### Sorun 22: WMSDE'yi SQL Server'a geçiş yaptıysanız, WSUS 2.0 Service Pack 1'e yükseltme yapmadan önce bu kayıt defteri girişini düzeltin.

WSUS 2.0 to Service Pack 1' yükseltmeyi planlıyorsanız ve WMSDE yüklemenizi SQL Server'a (uzak veya yerel) geçirdiyseniz, aşağıdaki kayıt defteri girişini değiştirdiğinizden emin olun:

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled

1 değeri 0 olarak değiştirilmelidir.

#### Sorun 23: Uzak SQL yüklemesinden WSUS 2.0 Service Pack 1'e geçiş yapma

Uzak SQl yapılandırmalı WSUS 2.0 Service Pack 1'e geçiş yaparken aşağıdaki adımları uygulayın:

1) Ön yüzde kurulum paketini herhangi bir anahtar olmadan çalıştırın ve yükseltmeyi seçin

2) Arka yüzde kurulum paketini herhangi bir anahtar olmadan çalıştırın ve yükseltmeyi seçin

#### Telif Hakkı

Bu belgedeki bilgiler, belirtilen sorunlara yönelik olarak, Microsoft Corporation'ın belgenin yayımlandığı tarihteki görüşlerini gösterir. Microsoft'un değişen piyasa koşullarına yanıt vermesi gerektiğinden, bu belgenin Microsoft'un bir taahhüdü olarak yorumlanmaması gerekir; Microsoft, belge yayımlandıktan sonra sunulan bilgilerin doğruluğunu garanti edemez.

Bu belge yalnızca bilgi verme amaçlıdır. MICROSOFT BU BELGEDEKİ BİLGİLER İÇİN AÇIK, ZIMNİ VEYA YASAL HİÇBİR GARANTİ VERMEZ.

Tüm geçerli telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakları kapsamındaki haklar saklı kalmak kaydıyla, Microsoft Corporation'ın yazılı açık izni olmadan bu belgenin hiçbir bölümü herhangi bir biçimde, herhangi bir yöntemle (elektronik, mekanik, fotokopi, kayıt veya başka şekilde) veya herhangi bir amaçla çoğaltılamaz, aktarılamaz, bir geri alma sisteminde saklanamaz veya bu tür bir sisteme konamaz.

Bu belgeye konu olan malzemeye ilişkin olarak Microsoft'un patentleri, patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından sağlanan herhangi bir yazılı lisans sözleşmesinde açıkça belirtilmedikçe, bu belgenin size sağlanmış olması bu patentler, ticari markalar, telif hakları ve diğer fikri mülkiyet hakları için size herhangi bir lisans da verilmiş olduğu anlamına gelmez.

Aksi belirtilmediği sürece, burada adı geçen şirketlerin, kuruluşların, ürünlerin, etki alanı adlarının, e-posta adreslerinin, logoların, kişilerin, yerlerin ve olayların gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla herhangi bir ilişkisi yoktur.

© 2005 Microsoft Corporation. Tüm hakları saklıdır.

Microsoft, SQL Server, Windows ve Windows Server, Microsoft Corporation'ın ABD'de ve/veya diğer ülkelerdeki kayıtlı ticari markaları veya ticari markalarıdır.

Burada adı geçen gerçek şirket ve ürünlerin adları, ilgili sahiplerinin ticari markaları olabilir.
