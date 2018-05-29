---
TOCTitle: WSUS Service Pack 1 için Benioku Dosyası
Title: WSUS Service Pack 1 için Benioku Dosyası
ms:assetid: '937ecfe9-e8e0-41ac-85f7-4b65956f3d1e'
ms:contentKeyID: 18155206
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708486(v=WS.10)'
---

WSUS Service Pack 1 için Benioku Dosyası
========================================

Bu belgede, Windows Server Update Services Service Pack 1'i (WSUS SP1) etkilediği bilinen sorunlar açıklanır. WSUS SP1 bilgilerinin hemen ardından, önceden özgün WSUS benioku notlarında yer alan tüm bilgileri bulabilirsiniz. Bu bilgiler, WSUS'u yüklemeye yönelik önerileri ve gereksinimleri içerir. WSUS SP1'i karşıdan yüklemek için, bkz: [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=67516).

WSUS SP1'deki Yenilikler
------------------------

WSUS SP1, WSUS'un güvenliğini, güvenilirliğini, ölçeklenebilirliğini, uyumluluğunu ve performansını artıran bir hizmet paketi sürümüdür. Yeni özellik ve geliştirmeler şunlardır:

-   Windows Vista istemci desteği: Windows Vista çalışan bilgisayarlar WSUS SP1 Server kullanılarak güncelleştirilebilir.
-   Daha fazla istemci dili desteği: Tüm Office ve Windows Vista dilleri desteklenir.
-   WMSDE'nin yeni sürümü: WMSDE örneği, WSUS SP1 tarafından WMSDE SP4'e yükseltilir (WSUS RTM, WMSDE SP3 kullanır).
-   Performans geliştirmeleri: WSUS SP1, kullanıcı arabirimi yanıt sürelerini kısaltan çeşitli performans geliştirmeleri içerir.
-   Tüm düzeltmeler: WSUS SP1, WSUS RTM sonrasında yayımlanan tüm değişiklikleri ve düzeltmeleri içerir.
-   SQL Server 2005 desteği.

WSUS SP1 Yükseltmesine Başlamadan Önce
--------------------------------------

WSUS SP1 yükseltmesi sırasında aşağıdaki sorunlarla karşılaşabilirsiniz. Bu konunun özgün sürümündeki “Başlamadan Önce” bölümünde özetlenen sorunlar ve gereksinimlerin bu bölümde açıklanmadığını ve hala geçerli olduğunu unutmayın. Örneğin, özgün “Başlamadan Önce” bölümünde özetlenen kurulum gereksinimleri yine geçerlidir.

**Not**   WSUS 2.0'a SP1 uygulandıktan sonra, hizmet paketi kaldırılamaz. SP1'i kaldırmak, ürünü tümüyle kaldırır.

**Önemli**   Bu belge, kayıt defterini düzenlemeyle ilgili bilgiler içermektedir. Kayıt defterini değiştirmeden önce yedeklediğinizden emin olun. Bir sorun çıkması durumunda kayıt defterini nasıl geri yükleyeceğinizi bildiğinizden emin olun. Kayıt defterini yedekleme, geri yükleme ve değiştirme hakkında daha fazla bilgi için, Microsoft Bilgi Bankası'nda yer alan aşağıdaki makaleye bakın:

[Microsoft Windows kayıt defterinin açıklaması](http://support.microsoft.com/kb/256986) (http://support.microsoft.com/kb/256986/)

#### Sorun 1: Veritabanı yedeklemesi için yeterli disk alanınız olmasını sağlayın

WSUS RTM'den yükseltme sırasında, WSUS SP1 Kurulumu otomatik olarak WSUS veritabanının bir yedek kopyasını oluşturur. WSUS sunucusunun dosya sisteminde WSUS veritabanının yedeğini depolamak için yeterli disk alanı bulunmasını sağlamazsanız WSUS SP1 Kurulumu başarısız olur.

**Yeterli disk alanı olup olmadığını belirlemek için**
1.  Windows Gezgini'ni açın ve WSUS veritabanının depolandığı klasöre gidin. WSUS varsayılan olarak veritabanını şu konuma yükler:

    
        ```
2.  **CTRL** tuşunu basılı tutarak **SUSDB.MDF** ve **SUSDB\_log.LDF** dosyalarını seçin, sonra da sağ tıklatıp **Özellikler**'i seçin.

3.  **Dosyalar** iletişim kutusunda, **Diskteki boyutu** değerini okuyun. WSUS SP1'in yüklenebilmesi için diskinizde en az bu boyutta boş alan olmalıdır.

4.  **Başlat** menüsünde, **Bilgisayarım**'ı tıklatın. WSUS'un yüklü olduğu diskte yeterli miktarda boş disk alanı olduğundan emin olun.

WSUS SP1 Kurulumu herhangi bir nedenle başarısız olursa, yedekleme veritabanını el ile geri yükleyin. WSUS veritabanını geri yükleme yönergeleri için, bkz: [WSUS Operations Guide](http://technet2.microsoft.com/windowsserver/en/library/05f2e884-ae62-4c90-9681-6c9f2f3c9fd91033.mspx).

#### Sorun 2: WSUS SP1 yalnızca WSUS RTM'yi yükseltir

WSUS SP1, yalnızca WSUS RTM'yi yükseltmek için kullanılabilir. Şimdilik, WSUS Release Candidate sürümünden yükseltme desteği bulunmamaktadır. WSUS Release Candidate veya WSUS'un önceki bir derlemesini kullanıyorsanız, bu derlemeleri kaldırdıktan sonra WSUS SP1'i çalıştırmanız gerekir.

#### Sorun 3: WSUS SP1 yükseltmesi sırasında sunucunuzdaki IIS hizmeti durdurulur

WSUS SP1 yükseltme yükleyicisi, yükseltme işlemi sırasında sunucunuzdaki Internet Information Services (IIS) hizmetini durdurur. Bu, sunucunuzdaki IIS yüklemesi tarafından barındırılan hiçbir Web sitesinin yükseltme işlemi boyunca kullanılamayacağı anlamına gelir. IIS, yükseltme sonunda otomatik olarak başlatılır.

#### Sorun 4: Yükseltme sırasında, WSUS API'lerini çağıran uygulamaları çalıştırmamalısınız

WSUS Uygulama Arabirimi (API) çağrıları WSUS SP1 yükleyicisiyle çakışarak yükseltme işleminin başarısız olmasına neden olur (yükseltme işlemini tamamlamak için sunucunuzu yeniden başlatmanızın istendiği bir ileti alırsınız).

#### Sorun 5: WSUS SP1'e yükseltirken, virüsten koruma programlarınızı devre dışı bırakmanız gerekebilir

WSUS SP1'i uygulayarak WSUS'u yükselttiğinizde, yükseltme işlemini başarıyla gerçekleştirmek veya hizmet paketini uygulamak için virüsten koruma programlarını devre dışı bırakmanız gerekebilir. Virüsten koruma programlarını devre dışı bıraktıktan sonra, Windows Server çalışan bilgisayarı yeniden başlatmadan yükseltmeyi veya hizmet paketini uygulamayın. Bu yordam, güncelleştirme işleminin erişmesi gereken dosyaların kilitlenmesini engeller. Yükleme tamamlandıktan sonra, virüsten koruma programınızı yeniden etkinleştirmeyi unutmayın. Virüsten koruma programınızı ve sürümünüzü devre dışı bırakma ve yeniden etkinleştirme adımları için, virüsten koruma programı satıcınızın Web sitesini ziyaret edin.

| ![](/security-updates/images/Cc708486.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu geçici çözüm, ağınızdaki bilgisayarı kötü amaçlı kullanıcıların veya virüsler gibi kötü amaçlı yazılımların gerçekleştirdiği saldırılara karşı daha savunmasız bırakabilir. Bu geçici çözüm önerilmez, ancak geçici çözümü isterseniz kullanabilmeniz için bu bilgiler sağlanmaktadır. Bu geçici çözümü kullanmak kendi sorumluluğunuzdadır. |

| ![](/security-updates/images/Cc708486.note(WS.10).gif)Not                                                                                                                                                                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Virüsten koruma programı, bilgisayarınızın virüslerden korunmasına yardımcı olacak biçimde tasarlanmıştır. Virüsten koruma programınız devre dışı bırakıldığında, güvenmediğiniz kaynaklardan karşıdan dosya yüklememeli veya açmamalı, güvenmediğiniz Web sitelerini ziyaret etmemeli veya e-posta eklerini açmamalısınız. |

#### Sorun 6: Bir proxy sunucu kullanıyorsanız, SP1 yükseltmesi, proxy yapılandırmasının kullanıcı adını ve parolasını temizleyebilir.

Bir proxy sunucu kullanıyorsanız, SP1 yükseltmesi bazı durumlarda proxy yapılandırmasının kullanıcı adını ve parolasını temizleyebilir. Bu, güncelleştirmelerin Microsoft sunucularından eşitlenmesi işleminin bir “geçersiz parametre” hatası oluşturmasına neden olabilir. Bu sorunu gidermek için, proxy yapılandırmasının kullanıcı adını ve parolasını sıfırlayıp sunucunuzu yeniden eşitleyin.

#### Sorun 7: Başarısız olan bir yükseltme sonrasında WSUS sunucunuzu tutarlı bir duruma geri yüklemek ve yükseltmeyi yeniden denemek üzere yükseltme işlemini kurtarın.

WSUS SP1'e yükseltme işlemi başarısız olursa, WSUS yüklemeniz tutarsız veya kararsız bir durumda kalabilir. WSUS SP1'e yükseltmeyi yeniden denemek için, WSUS yüklemenizi tutarlı bir duruma getirmelisiniz. Bunu yapmak için, yükseltme işleminin başında oluşturulan yedek veritabanını kullanarak WSUS sunucunuzu yükseltme öncesi durumuna geri yükleyebilirsiniz.

Yükseltmenin başarısız olması durumunda, aşağıdaki adımları izleyerek WSUS SP1'e yükseltmeyi yeniden deneyin:

**WSUS SP1'e yükseltmeyi yeniden denemek için**
1.  WSUSSetup\_%timestamp%.log dosyasının içeriğini inceleyerek, yedek veritabanının konumunu belirleyin. Bu dosya aşağıdaki klasörde bulunur:

    -   %programfiles%\\Update Services\\LogFiles

2.  Aşağıdaki komutu kullanarak, yedek veritabanı WSUS bilgisayarına geri yükleyin:

    -   osql.exe -S &lt;VeritabanıÖrneği&gt; -E -Q "USE master ALTER DATABASE SUSDB SET SINGLE\_USER WITH ROLLBACK IMMEDIATE RESTORE DATABASE SUSDB FROM DISK=N'&lt;VeritabanıYedeklemesininYolu&gt;' WITH REPLACE ALTER DATABASE SUSDB SET MULTI\_USER"
    -   &lt;VeritabanıÖrneği&gt; ve &lt;VeritabanıYedeklemesininYolu&gt; yerine, sizin yüklemeniz için geçerli değerleri kullanın.
    -   &lt;VeritabanıÖrneği&gt; için, aşağıdaki kayıt defteri anahtarındaki değeri kullanın:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\SqlServerName
    -   &lt;VeritabanıYedeklemesininYolu&gt; için, 1. adımda belirlediğiniz değeri kullanın.

3.  WSUS'u kaldırın; ancak WSUS veritabanını, günlük dosyalarını ve güncelleştirme dosyalarını kaldırmak isteyip istemediğiniz sorulduğunda bu dosyaları saklayın. (**Microsoft Windows Server Update Services'ı Kaldır**'daki hiçbir seçeneğin işaretli olmamasını sağlayın.)

4.  WSUS RTM'yi yeniden yükleyin (özgün sürümü, WSUS SP1'i değil). İstendiğinde, varolan veritabanını kullanın. Bu, WSUS sisteminizi tutarlı bir duruma döndürür.

5.  WSUS SP1'i yükleyin.

**Not**    Yukarıda açıklanan 1. adımda yedeklediğiniz veritabanını WSUS SP1'in temiz yüklemesinde kullanamazsınız. Veritabanı şeması değiştiği için, WSUS SP1'e yükseltilmedikçe bu veritabanı uyumlu değildir.

#### Sorun 8: WMSDE veritabanı geçirilmişse, WSUS SP1 yükseltmesi bazı durumlarda başarısız olabilir

Çözüm, bir yerel veya uzak SQL sunucusuna geçiş yapmanıza bağlı olarak değişir.

#### Bir yerel SQL 2000 sunucusuna geçirilen WMSDE veritabanı

WSUS SP1 kurulum paketinin güncelleştirilecek bir WMSDE veritabanı bulunmadığını algılaması için bir kayıt defteri anahtarının değeri değiştirilmelidir.

WMSDE'yi bir yerel SQL 2000 sunucusuna geçirdiyseniz, WSUS SP1'e yükseltmeye çalışmadan önce kayıt defterinde aşağıdaki değişikliği yapmalısınız:

-   Aşağıdaki kayıt defteri anahtarının "1" olan değerini "0" olarak değiştirin:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled  

#### Bir uzak SQL 2000 sunucusuna geçirilen WMSDE veritabanı

WSUS SP1 kurulum paketinin güncelleştirilecek bir WMSDE veritabanı bulunmadığını algılaması için iki kayıt defteri anahtarının değeri değiştirilmelidir. Güncelleştirmenin ilk olarak arka uç sunucuda ve ardından ön uç sunucuda başlatılması gerekir.  

WMSDE'yi bir uzak SQL sunucusuna geçirdiyseniz, WSUS SP1'e yükseltmeye çalışmadan önce kayıt defterinde aşağıdaki değişiklikleri yapmalısınız:

1.  Aşağıdaki kayıt defteri anahtarının "1" olan değerini "0" olarak değiştirin:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 
2.  Aşağıdaki kayıt defteri anahtarının "0x80" olan değerini "0x20" olarak değiştirin:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\InstallType 

Bu kayıt defteri anahtarı değerlerini güncelleştirdikten sonra, yükseltme işlemini ilk olarak arka uç sunucularda ve ardından ön uç sunucularda başlatın.

#### Sorun 9: WSUS SP1, uzak SQL dağıtımları kullanılarak ayarlanmış WSUS sunucularını güncelleştirmiyor

WSUS SP1 kurulum paketini hem ön uç hem de arka uç sunucularda çalıştırmalısınız.

**Uzak SQL kullanıldığında WSUS SP1'e yükseltmek için**
1.  Kurulum paketini ön uç sunucuda anahtar kullanmadan çalıştırın ve yükseltmeyi seçin.

2.  Kurulum paketini arka uç sunucuda anahtar kullanmadan çalıştırın ve yükseltmeyi seçin.

#### Sorun 10: WSUS SP1'e yükseltmeden önce bilgisayar adını değiştirmek yükseltmenin başarısız olmasına neden olabilir

WSUS RTM'yi yükledikten sonra bilgisayar adını değiştirir ve sonra da WSUS SP1'e yükseltmeye çalışırsanız, WSUS SP1 yükseltmesi başarısız olabilir.

ASPNET ve WSUS Administrators gruplarını kaldırıp yeniden eklemek üzere aşağıdaki komut dosyasını kullanın. Daha sonra, yükseltmeyi yeniden çalıştırın.

        ```
| ![](/security-updates/images/Cc708486.note(WS.10).gif)Not           |
|--------------------------------------------------------------------------------|
| Son satırdaki &lt;İçerikDizini&gt; yerine, asıl içerik deponuzun yolunu yazın. |

WSUS Benioku Dosyasının Özgün İçeriği Aşağıda Yer Almaktadır
------------------------------------------------------------

Aşağıda, WSUS benioku dosyasının özgün içeriği yer almaktadır. WSUS SP1, aşağıdaki sorunlardan hiçbirini *gidermez*. Bu içerik, kolaylık olması için eklenmiştir.

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
<td style="border:1px solid black;">Windows Server 2003 işletim sistemleri için, Yükleme Merkezi'nde Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0 ve WinHTTP 5.1 Windows Server 2003 Güncelleştirmesi'ne (KB842773) bakın (<a href="http://go.microsoft.com/fwlink/?linkid=47251">http://go.microsoft.com/fwlink/?LinkId=47251</a>).
Windows Server 2000 işletim sistemleri için, Yükleme Merkezi'nde Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0 ve WinHTTP 5.1 Windows 2000 Güncelleştirmesi'ne (KB842773) bakın (<a href="http://go.microsoft.com/fwlink/?linkid=46794">http://go.microsoft.com/fwlink/?LinkId=46794</a>).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1</a>
Alternatif olarak, <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> sitesine giderek Kritik Güncelleştirmeler ve Hizmet Paketlerini tarayın; Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1'i yükleyin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework Sürüm 1.1 Redistributable Package</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework Sürüm 1.1 Redistributable Package</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Alternatif olarak, <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update</a> sitesine giderek Kritik Güncelleştirmeler ve Hizmet Paketlerini tarayın; Windows Server 2000 için Microsoft .NET Framework 1.1 Service Pack 1'i yükleyin.</td>
</tr>
</tbody>
</table>
 

Bu gereksinimlerin yanı sıra, WSUS, gerekirse sunucunuza ASP.NET 1.1 sürümünü de yükleyebilir veya bu sürümü yapılandırabilir. (WSUS Setup, ASP.NET'i yapılandırır.)

#### Windows 2000'e MSDE Yükleme

WSUS için Windows 2000 kullanıyorsanız ve Microsoft SQL Server 2000'e erişiminiz yoksa, WSUS Setup'ı çalıştırmadan önce Microsoft SQL Server 2000 Desktop Engine'i (MSDE) yüklemelisiniz. WSUS sunucunuzda MSDE zaten yüklüyse, WSUS için özel bir örneğini kurmanız gerekmez. WSUS kurulumu sırasında varolan örneğin adını belirtmeniz yeterlidir.

Windows 2000 Server'a MSDE dört adımda yüklenebilir. İlk olarak, MSDE arşivini karşıdan yüklemeniz ve WSUS sunucunuza genişletmeniz gerekir. Daha sonra, bir komut isteminde komut satırı seçeneklerini kullanarak MSDE Setup'ı çalıştırın, sa parolasını ayarlayın ve örnek adı olarak WSUS atayın. Ardından, MSDE yüklemesi tamamlandığında, WSUS örneğinin bir NT hizmeti olarak çalıştığını doğrulamalısınız. Son olarak, WSUS sunucunuzu korumak üzere MSDE'ye bir güvenlik düzeltme eki yüklemelisiniz.

#### Adım 1: MSDE arşivini karşıdan yükleme ve genişletme

MSDE arşivini karşıdan yüklemeniz ve WSUS sunucunuza genişletmeniz gerekir. Bkz: [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Adım 2: MSDE'yi yükleme

Komut isteminde komut satırı seçeneklerini kullanarak MSDE Setup'ı çalıştırın, sa parolasını ayarlayın ve örnek adı olarak WSUS atayın. MSDE yüklemesi tamamlandığında, WSUS örneğinin bir NT hizmeti olarak çalıştığını doğrulamalısınız.

MSDE'yi yüklemek için, sa parolasını ayarlayın ve bir örnek adı atayın:

1.  Komut isteminde, “Adım 1: MSDE arşivini karşıdan yükleme ve genişletme” bölümünde belirtilen MSDE yükleme klasörüne gidin.
2.  Aşağıdakini yazın: **setup sapwd="***parola***" instancename=WSUS**
    Burada *parola*, MSDE'nin bu örneğinde sa hesabı için bir güçlü parola ve **instancename** parametresi de veritabanı örneğinin adıdır. Alternatif olarak, WSUS veritabanınız için varsayılan örnek adını ("WSUS" yerine) kullanabilirsiniz. Bunu yapar5sanız, komut satırı parametrenizde **instancename=WSUS** yazmanız gerekmez. Bu komut, MSDE kurulum programını başlatır, sa parolasını ayarlar ve MSDE'nin bu örneğini belirttiğiniz değer olarak adlandırır.

#### Adım 3: MSDE'nin WSUS örneğinin yüklü olduğunu doğrulama

1.  **Başlat**'ı ve sonra **Çalıştır**'ı tıklatın.
2.  **Aç** kutusuna **services.msc** yazın ve **Tamam**'ı tıklatın.

Hizmetler listesini aşağı kaydırın ve (örnek adı olarak "WSUS" kullandıysanız) MSSQL$WSUS veya (varsayılan örnek adını kullandıysanız) MSSQLSERVER adlı bir hizmetin bulunduğunu doğrulayın.

#### Adım 4: MSDE örneğini başlatın.

MSDE yüklemesinin sonunda, örneği başlatmanız gerekir. Örnek adı olarak "WSUS" kullandıysanız, "MSSQL$WSUS" hizmetini başlatırsınız. Varsayılan örnek adını kullandıysanız, MSSQLSERVER hizmetini başlatırsınız. Bu hizmet başlatılmazsa, WSUS, veritabanı örneğini kullanamaz.

#### Adım 5: MSDE'yi güncelleştirme

[MS03-031: SQL Server İçin Toplu Düzeltme Eki](http://go.microsoft.com/fwlink/?linkid=47364) adlı bültende açıklanan güvenlik düzeltme ekini karşıdan yüklemeniz ve kurmanız gerekir.

Güvenlik düzetme ekini karşıdan yüklemek için, bkz: [SQL Server 2000 (32-bit) Güvenlik Düzeltme Eki MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

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

#### Sorun 1: IIS Lockdown Wizard

Windows 2000 Server çalışan bir bilgisayarda Internet Information Services (IIS) çalıştırıyorsanız, Microsoft TechNet'teki IIS Lockdown Aracı sayfasından IIS Lockdown Wizard'ın en son sürümünü (URLScan içerir) yükleyin. Microsoft, IIS sunucularınızın güvenliğini sağlamak için bu aracı yüklemenizi önerir. IIS Lockdown Wizard, IIS'nin gerekli olmayan özelliklerini kapatarak güvenlik risklerini azaltır.

| ![](/security-updates/images/Cc708486.note(WS.10).gif)Not                                                                                                                                  |
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
-   Uzak sunucuda Terminal Hizmetleri yüklüyse ve uygulama modunda çalışıyorsa, WSUS veritabanı olarak kullanılacak uzak SQL Server'ın kurulumu başarısız olur. SQL Server'ı bir Terminal Hizmetleri sunucusuna yüklerken şunları yapmalısınız:
    1.  Kurulumu çalıştırmadan önce, bir komut istemi açın ve şu komutu yazın: "change user /install"
    2.  SQL Server Setup'ı çalıştırın.
    3.  Kurulumu çalıştırdıktan sonra, komut istemine şunu yazın: "change user /execute"
-   Uzak SQL Server WSUS veritabanını kurmak için, hem ön uç hem de arka uç bilgisayarda Local Administrators güvenlik grubunun üyesi olmalısınız.
-   Uzak SQL ile ilgili sorunlar hakkında daha fazla bilgi için, [Microsoft Windows Server Update Services'ı Dağıtma](http://go.microsoft.com/fwlink/?linkid=41777) belgesinde "Ek C: Uzak SQL" bölümüne bakın.

#### Sorun 13: Kopya aşağı akım sunucusu, ana yukarı akım sunucusundan daha az onaylanabilir

Kopya aşağı akım sunucusu, ana yukarı akım sunucusundan daha az onaylanabilir. Bunun nedeni, içeriğin yukarı akım sunucusuna karşıdan yüklenmesi tamamlanıncaya kadar yükleme onaylarının aşağı akım sunucusuna iletilmemesidir.

#### Sorun 14: İlk eşitleme başarısız olursa eşitlemeyi yeniden deneyin

Eşitleme başarısız olursa, sorun giderme adımlarının ilki sunucuyu yeniden eşitlemeye çalışmak olmalıdır. Sonraki eşitlemeler başarısız olursa, WSUS Operations Guide'daki sorun giderme bilgilerini kullanın.

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

**Uyarı**: Bu işlem, Microsoft SharePoint ve Exchange işlevselliğini geçersiz kılabilir.

#### Sorun 19: Internet Explorer güvenliğini artırmanın etkinleştirilmiş olduğu bilgisayarlarda, WSUS konsol URL'sinin Güvenilen siteler ve Yerel intranet Web içeriği bölgelerine eklenmesi gerekir

Bir bilgisayarda Internet Explorer güvenliğini artırma özelliği (Microsoft Windows Server 2003'te Internet Explorer Artırılmış Güvenlik Yapılandırması bileşeni olarak da bilinir) etkinleştirilmişse ve WSUS konsolunu Güvenilen siteler ve Yerel intranet Web içeriği bölgelerine eklemezseniz, WSUS konsolunda her sayfa açtığınızda kullanıcı kimlik bilgileri sorulur.

WSUS konsolunu **Yerel intranet** ve **Güvenilen siteler** Web içeriği bölgelerine eklemek için:

1.  **Internet Seçenekleri**'ni açın (örneğin, **Başlat**'ı tıklatın, **Denetim Masası**'nın üzerine gelin ve **Internet Seçenekleri**'ni tıklatın.
2.  **Güvenlik** sekmesinde, **Yerel intranet**'i tıklatın, **Siteler**'i tıklatın, **Gelişmiş**'i tıklatın, URL'yi ekleyin (http://*WSUSSunucuadı*/WSUSAdmin) ve sonra da **Tamam**'ı tıklatın.
3.  **Güvenilen siteler**'i tıklatın, **Siteler**'i tıklatın, WSUS konsolu URL'sini ekleyin, **Tamam**'ı tıklatın ve sonra yeniden **Tamam**'ı tıklatarak **Internet Seçenekleri**'nden çıkın.

#### Telif Hakkı

Bu belgedeki bilgiler, belirtilen sorunlara yönelik olarak, Microsoft Corporation'ın belgenin yayımlandığı tarihteki görüşlerini gösterir. Microsoft'un değişen piyasa koşullarına yanıt vermesi gerektiğinden, bu belgenin Microsoft'un bir taahhüdü olarak yorumlanmaması gerekir; Microsoft, belge yayımlandıktan sonra sunulan bilgilerin doğruluğunu garanti edemez.

Bu belge yalnızca bilgi verme amaçlıdır. MICROSOFT BU BELGEDEKİ BİLGİLER İÇİN AÇIK, ZIMNİ VEYA YASAL HİÇBİR GARANTİ VERMEZ.

Tüm geçerli telif hakkı yasalarına uymak kullanıcının sorumluluğundadır. Telif hakları kapsamındaki haklar saklı kalmak kaydıyla, Microsoft Corporation'ın yazılı açık izni olmadan bu belgenin hiçbir bölümü herhangi bir biçimde, herhangi bir yöntemle (elektronik, mekanik, fotokopi, kayıt veya başka şekilde) veya herhangi bir amaçla çoğaltılamaz, aktarılamaz, bir geri alma sisteminde saklanamaz veya bu tür bir sisteme konamaz.

Bu belgeye konu olan malzemeye ilişkin olarak Microsoft'un patentleri, patent başvuruları, ticari markaları, telif hakları veya diğer fikri mülkiyet hakları olabilir. Microsoft tarafından yazılı bir lisans sözleşmesinde açıkça belirtilmediği sürece, bu belgeyi bulundurmak, size patent, ticari marka, telif hakkı ve diğer fikri mülkiyet haklarını kullanma yetkisi vermez.

Aksi belirtilmediği sürece, burada adı geçen şirketlerin, kuruluşların, ürünlerin, etki alanı adlarının, e-posta adreslerinin, logoların, kişilerin, yerlerin ve olayların gerçek şirket, kuruluş, ürün, etki alanı adı, e-posta adresi, logo, kişi, yer veya olayla herhangi bir ilişkisi yoktur.

© 2006 Microsoft Corporation. Tüm hakları saklıdır.

Microsoft, SQL Server, Windows ve Windows Server, Microsoft Corporation'ın ABD'de ve/veya diğer ülkelerdeki kayıtlı ticari markaları veya ticari markalarıdır.

Burada sözü edilen gerçek şirketler ve ürünler, ilgili firmaların ticari markaları olabilir.
