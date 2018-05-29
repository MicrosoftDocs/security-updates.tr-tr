---
TOCTitle: Etki Alanı Denetleyicisi ve Veritabanı Sunucusu Kurma
Title: Etki Alanı Denetleyicisi ve Veritabanı Sunucusu Kurma
ms:assetid: 'd20f8305-9f9e-4760-bfbf-82824db60d1f'
ms:contentKeyID: 18125273
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747681(v=WS.10)'
---

Etki Alanı Denetleyicisi ve Veritabanı Sunucusu Kurma
=====================================================

Kök sertifika sunucusu veya lisans sunucusu yüklemeden önce, SQL Server 2000 Service Pack 3 (SP3) veya Microsoft® SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A gibi bir veritabanı sunucusu ve Active Directory kullanarak uygun etki alanı ve veritabanı desteğini sağladığınızdan emin olun. Üretim ortamınız gerekli bileşenleri zaten çalıştırıyor olabilir, ancak sınama amacıyla üretim ortamınızı kullanmamanız önerilir.

Aşağıdaki yordamlar sunucu tarafında sınama amaçları için yalıtılmış bir ağdaki tek bir bilgisayara hem etki alanı denetleyicisini hem de veritabanı sunucusunu kurar.

| ![](/security-updates/images/Cc747681.note(WS.10).gif)Not                                                                                                                                                                                                                                                         |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu örnekte, veritabanı sunucusu etki alanı denetleyicisinde çalışmaktadır. Üretim ortamında, diğer bileşenleri etki alanı denetleyicisinde barındırmanız genellikle önerilmez. Altyapının tamamını en az sayıda bilgisayara yükleyebilmek için bu örnekte Active Directory ve veritabanı sunucusu aynı bilgisayara yüklenir. |

Veritabanı sunucunuz olarak MSDE 2000'i kullanmayı seçerseniz, bunun hiçbir ağ arabirimini desteklemediğini ve MSDE 2000 kullanım koşullarının, bir MSDE 2000 veritabanını değiştirmek için SQL Server istemci araçlarını kullanmanıza izin vermediğini bilmeniz gerekir. Bu sınırlama nedeniyle, günlük bilgilerini görüntüleyemeyecek veya yapılandırma veritabanında depolanmış verileri değiştiremeyeceksiniz. Bu nedenle, MSDE 2000'nin yalnızca sınama ortamlarında RMS veritabanlarını desteklemek üzere kullanılması önerilmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Altyapı Bileşeni</th>
<th style="border:1px solid black;" >Etki Alanı Denetleyicisi ve Veritabanı Sunucusu Kurma Adımları</th>
<th style="border:1px solid black;" >Üretim Ortamında Dağıtım Notları</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">İşletim sistemi</td>
<td style="border:1px solid black;">RMS donanım gereksinimlerini karşılayan ancak henüz ağa bağlı olmayan bir bilgisayara, Windows 2000 Server SP3 veya daha ileri bir sürüm ya da Windows Server 2003 yükleyin. Bölümde NTFS dosya sistemini kullanın.</td>
<td style="border:1px solid black;">Her zaman en son hizmet paketlerini ve güncelleştirmeleri yüklemeniz önerilir. NTFS olarak biçimlendirilmiş bölümleri kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ağ bağlantısı</td>
<td style="border:1px solid black;">Internet bağlantısı sağlayan, ancak üretim ortamından yalıtılmış bir ağa bağlanın.</td>
<td style="border:1px solid black;">Internet bağlantısı uygun bir güvenlik duvarına sahip olmalıdır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IP adresi</td>
<td style="border:1px solid black;">Bu bilgisayara statik bir IP adresi atayın.</td>
<td style="border:1px solid black;">Sunucular için her zaman statik IP adresleri kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Active Directory</td>
<td style="border:1px solid black;">Yerel yönetici olarak oturum açın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Başlat'ı ve <strong>Çalıştır</strong>'ı tıklatın, <strong>Aç</strong> kutusuna <code>dcpromo</code> yazın ve sonra <strong>Tamam</strong>'ı <strong>tıklatın</strong>.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Active Directory Yükleme Sihirbazı başlatıldığında, yeni bir ormanda yeni bir etki alanı oluşturmak için sihirbazı izleyin ve aşağıdaki seçenekler dışında varsayılan seçenekleri kabul edin:
Etki alanı adını belirtin, örneğin, contoso.com.
Sihirbazın DNS'yi bilgisayarda yapılandırmasına izin verin.
Tüm etki alanı denetleyicileri Windows 2000 veya daha ileri bir sürümü çalıştırıyorsa <strong>Yalnızca Windows 2000 sunucularıyla uyumlu izinler</strong> seçeneğini belirleyin.
Yerel yönetici için sağlam bir parola belirtin.</td>
<td style="border:1px solid black;">RMS'yi uygulamak için yeni etki alanları gerekiyorsa, bunları Active Directory'de oluşturun.
Tüm hesaplar için her zaman sağlam parolalar kullanın.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">İstendiğinde bilgisayarı yeniden başlatın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Şu işlemleri sırasıyla yaparak işlevsel düzeyi doğrulayın: <strong>Active Directory Kullanıcıları ve Bilgisayarları</strong> eklentisini açın, etki alanı adını sağ tıklatın, <strong>Özellikler</strong>'i tıklatın ve sonra <strong>Etki alanı çalışma modu</strong> kutusundaki ayarı doğrulayın. Windows 2000'den daha önceki herhangi bir etki alanı denetleyicisi yoksa, etki alanının <strong>Yerel mod</strong>'da çalışmasını sağlamak için <strong>Modu değiştir</strong>'i tıklatın.
Not: Windows Server 2003'te, <strong>Etki alanı işlem modu</strong> ayarı <strong>Etki alanı işlev düzeyi</strong> ayarıyla değiştirilmiştir.</td>
<td style="border:1px solid black;">En iyi güvenlik ve yönetilebilirlik elde etmek üzere, RMS desteği için Windows 2000 karma işlev düzeyini kullanmamalısınız.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Kullanıcı hesapları</td>
<td style="border:1px solid black;">RMS için RMS hizmet hesabı olarak kullanılacak bir etki alanı kullanıcı hesabı oluşturun; örneğin, ContosoRMS@contoso.com. Sağlam bir parola belirtin. Kullanıcı için bir e-posta adresi belirttiğinizden emin olun. E-posta adresi Active Directory'de belirtilmemişse, kullanıcı RMS'den lisans ve sertifika alamaz.
Not: RMS hizmet hesabı, RMS'yi yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz.</td>
<td style="border:1px solid black;">Active Directory'de RMS hizmet hesabı tarafından kullanılacak ayrı bir hesap oluşturmalısınız. E-posta adresi ekleyin. Hesaba herhangi bir özel izin vermeyin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQL Server 2000</td>
<td style="border:1px solid black;">Veritabanını yüklemek istediğiniz sunucuya oturum açın. Bu, etki alanı denetleyicisiyle aynı sunucuysa, etki alanı yöneticisi olarak oturum açmalısınız.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Veritabanı sunucusu yazılımını yüklemek için veritabanı yazılımınızla gelen yönergeleri izleyin.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Veritabanı sunucusunu yüklemek için aşağıdaki, sunuculara yönelik en iyi uygulama yöntemlerini kullanın:
<ul>
<li>Veritabanı sistem yöneticisi hesabı için bir ad ve bir kuruluş adı sağlayın; örneğin, Contoso.<br />
<br />
</li>
<li>Sağlam bir sistem yöneticisi parolası belirtin.<br />
<br />
</li>
<li>Tümleşik Windows kimlik doğrulama yöntemlerini kullanın.<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Tümleşik Windows Kimlik Doğrulama Modu kullanmalısınız. Veritabanı sunucunuzu bu modda çalıştıramıyorsanız, RMS kurulumunda yapılması gerekebilecek değişiklikleri belirlemek için etki alanı yöneticinizle ve veritabanı sunucusu yöneticinizle bağlantı kurun.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Veritabanı hizmetinin durdurulduğunu doğrulayın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Veritabanı sunucunuz için yazılım güncelleştirmelerini yükleyin. Parola sorulduğunda, kurulum sırasında belirttiğiniz parolayı kullanın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Bilgisayarı yeniden başlatın. Veritabanı hizmetinin başlatıldığını doğrulayın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Kullanıcı hesaplarının Active Directory'de geçerli e-posta adresi özniteliklerine sahip olduğunu doğrulayın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">RMS'yi yönetecek (ve kök sertifika ve lisans sunucularını sağlayacak) etki alanı kullanıcısının gerekli veritabanı sunucusu izinlerine sahip olduğundan emin olun. Veritabanı sunucunuz olarak SQL Server kullanıyorsanız, <strong>SQL Server Enterprise Manager</strong> eklentisini kullanan kullanıcı için oturum açma tanıtıcısı ekleyebilirsiniz. Eklentide, sunucu ve sunucu grubunu genişletin ve sonra <strong>Security</strong> öğesini genişletin. <strong>Logins</strong> öğesini tıklatın, kullanıcının etki alanı hesabı için yeni oturum açma bilgileri ekleyin, <strong>Server Roles</strong> sekmesini tıklatın ve sonra <strong>Server Administrators</strong> onay kutusunu işaretleyin.</td>
<td style="border:1px solid black;">Önemli: Lisans almak ve içerik yayımlamak için RMS'yi kullanan tüm kullanıcıların ve grupların, hesaplarındaki Active Directory Kullanıcıları ve Grupları MMC eklentisinde, kullanıcı <strong>Özellikleri</strong>'nin <strong>Genel</strong>.sekmesinde yapılandırılmış bir e-posta adresi bulunmalıdır.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet bağlantısı
(isteğe bağlı)</td>
<td style="border:1px solid black;">Tarayıcınızın ve sunucunuzun (gerekli proxy sunucusu yapılandırmaları da dahil), TCP/IP ve LMHOSTS/HOSTS ayarlarınızın Internet'e erişmek için düzgün yapılandırıldığını doğrulayın. http://uddi.microsoft.com adresine giderek bunu sınayın. Bu sayfayı açabiliyorsanız, RMS, Microsoft Kayıt Hizmeti'ne bağlanabilir.</td>
<td style="border:1px solid black;">Internet erişimini doğrulamak için http://uddi.microsoft.com adresine gidin.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Yazılım güncelleştirmeleri</td>
<td style="border:1px solid black;">Bu bilgisayarda yüklü olan yazılımlar için en son güncelleştirmeleri (www.microsoft.com adresindeki en son Windows güncelleştirmeleri de dahil olmak üzere) yükleyin ve kurun.</td>
<td style="border:1px solid black;">Her zaman en son hizmet güncelleştirmelerini yükleyin ve kurun.</td>
</tr>
</tbody>
</table>
  
Yukarıdaki adımların tümünü uyguladıktan sonra, RMS'yi çalıştıracak bilgisayarlarda başlangıç kurulumunu (önkoşul yazılımları yüklemek de dahil) gerçekleştirmeye hazırsınızdır.
