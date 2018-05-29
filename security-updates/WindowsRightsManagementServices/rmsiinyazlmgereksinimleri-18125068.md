---
TOCTitle: RMS için Yazılım Gereksinimleri
Title: RMS için Yazılım Gereksinimleri
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18125068
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720201(v=WS.10)'
---

RMS için Yazılım Gereksinimleri
===============================

RMS sunucuları çalıştırmak için yazılım gereksinimleri aşağıdaki tabloda listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Yazılım</th>
<th style="border:1px solid black;" >Gereksinim</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">İşletim sistemi</td>
<td style="border:1px solid black;">Web Edition dışındaki tüm Microsoft Windows Server® 2003 sürümleri.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dosya sistemi</td>
<td style="border:1px solid black;">NTFS dosya sistemi önerilir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">İşletim Sistemi bileşenleri</td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (MSMQ da denir); Active Directory® Dizin Hizmeti Tümleştirmesi etkinleştirilmiş olarak.<br />
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
<tr class="even">
<td style="border:1px solid black;">Active Directory® dizin hizmeti</td>
<td style="border:1px solid black;">Etki alanı denetleyicilerinin Windows Server 2000 Service Pack 3 (SP3) veya daha sonraki sürümünü çalıştırdığı Active Directory etki alanında RMS yüklü olmalıdır. İçerik kullanmak ve yayımlamak için RMS'yi kullanan tüm kullanıcıların ve grupların Active Directory'de yapılandırılmış bir e-posta adresi bulunmalıdır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Veritabanı sunucusu</td>
<td style="border:1px solid black;">RMS, işlem yapmak için bir veritabanı ve depolanmış yordamlara ihtiyaç duyar. Microsoft SQL Server 2000 SP3a veya sonrası ya da Microsoft SQL Server 2005 kullanabilirsiniz. Sınama veya diğer tek bilgisayar dağıtımı için, Microsoft SQL Server Desktop Engine (MSDE 2000) SP3 veya Microsoft SQL Server 2005 Express Edition kullanılabilir.</td>
</tr>
</tbody>
</table>
  
Birden çok Active Directory ormanının bulunduğu bir ortamda RMS'yi dağıtıyorsanız, grup üyeliğinin tüm Genel Kataloglar'a çoğaltılabilmesi için Active Directory Evrensel Grupları'nı kullanmanız gerekir. Evrensel Gruplar oluşturmak için, etki alanınızın işlev düzeyi en azından Windows 2000 Özgün olarak ayarlanmalı ve orman işlev düzeyi Windows Server 2003'e yükseltilmelidir.
  
MSDE 2000 veya Microsoft SQL Server 2005 Express Edition herhangi bir ağ arabirimini desteklemediği için, MSDE 2000 veya Microsoft SQL Server 2005 Express Edition'ın RMS veritabanlarını yalnızca sınama ortamlarında desteklemek için kullanılması önerilir. Ayrıca, MSDE 2000 veya Microsoft SQL Server 2005 Express Edition'ın kullanım koşulları, MSDE 2000 veya Microsoft SQL Server 2005 Express Edition veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınızı belirtir. Bu sınırlama, günlük bilgilerini görüntüleyememenize veya yapılandırma veritabanında saklanan verileri değiştirememenize neden olur.
  
Sunucunuzda ASP.NET 1.1 sürümü kurulu değilse, Windows Server 2003'ün 32 bit'lik ve Windows Server 2003'ün 64 bit'lik sürümlerinden hangisini kullandığınıza bağlı olarak kurulum işlemi değişiklik gösterebilir.
  
Windows Server 2003'ün 32 bit'lik sürümünü kullanıyorsanız, ASP.NET 1.1 sürümünü kurmak ve etkinleştirmek için aşağıdaki adımları izleyin:
  
1.  **Denetim Masası**'nda **Program Ekle veya Kaldır**'ı açın ve **Windows Bileşenlerini Ekle/Kaldır**'ı tıklatın.  
2.  **Uygulama sunucusu**'nu ve ardından **Ayrıntılar**'ı tıklatın.  
3.  Windows Bileşen Sihirbazı'nda **ASP.NET**'i seçin.  
4.  ASP.NET 1.1 yüklüyse, ancak IIS Web hizmeti uzantısı olarak kabul edilmiyorsa:  
    -   Internet Bilgi Hizmetleri Yöneticisi'ni açın.  
    -   **IIS Web hizmeti uzantısı**'nı tıklatın, ASP.NET v1.1.4322'i seçin ve **İzin Ver**'i tıklatın.
  
Windows Server 2003'ün 64 bit'lik sürümünü kullanıyorsanız, ASP.NET 1.1 sürümünü kurmak ve etkinleştirmek için aşağıdaki adımları izleyin:
  
1.  ASP.NET 1.1'i yükleyecek olan NET Framework 1.1'i yükleyin. Microsoft .NET Framework Sürüm 1.1 Redistributable Package'ı Microsoft Yükleme Merkezi'nden ([http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=69985)) yükleyebilirsiniz.  
2.  Internet Bilgi Hizmetleri Yöneticisi'ni açın.  
3.  IIS Web hizmeti uzantısı'nı tıklatın, ASP.NET v1.1.4322'i seçin ve İzin Ver'i tıklatın.
  
RMS'yi Windows Server 2003'ün 64 bit'lik sürümünde çalıştırıyorsanız, IIS'nin RMS ile birlikte çalışması için aşağıdaki adımları izlemeniz gerekir:
  
1.  **Başlat**'ı ve ardından **Çalıştır**'ı tıklatın  
2.  **Aç** penceresine aşağıdaki komutu yazın ve ENTER'a basın:
  
**"cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
RMS, .NET Framework sürüm 2.0 için tasarlanmamıştır. Yan yana yükleme desteklenmekle birlikte, ASP.NET'in ASP.NET v1.1.4322 kullanacak biçimde yapılandırıldığından emin olmalısınız. Yan yana yüklemenin başarılı olmasını sağlamak için iki seçeneğiniz vardır:
  
-   RMS sunucusunu yüklemeden önce, .NET Framework sürüm 2.0'ı yükleyin.  
-   Aşağıdaki komutu çalıştırarak, ISS'deki Varsayılan Web Sitesi'nde ASP.NET sürümünü yeniden sürüm 1.1.4322 olarak ayarlayın:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Active Directory, Message Queuing ve IIS hakkında daha fazla bilgi için Windows Server 2003 Yardım ve Destek Merkezi'ne başvurun.
  
| ![](/security-updates/images/Cc720201.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| RMS sunucusunu, Varsayılan Web Sitesinde veya IIS'de daha önce tanımladığınız herhangi bir sitede sağlayabilirsiniz. Güvenlik nedeniyle, bu sunucuyu herhangi bir ek site veya hizmet çalıştırmak için kullanmamalısınız. Aksi halde, aynı hesap altında (özellikle Local System hesabı) RMS olarak çalışan birden çok uygulama ve hizmet oluşabilir. Bu durum, özel anahtarları yetkisiz işlemlerle karşı karşıya bırakabilir. RMS sunucusunu, Microsoft Office SharePoint Server 2007 ile aynı Web sitesinde sağlamamanız gerekir. RMS'yi Kerberos kimlik doğrulamasıyla kullanamazsınız. RMS sunucusunu bir Web sitesinde sağlamak, Kerberos kimlik doğrulamasını o sunucu için devre dışı bırakır. RMS, ASP.NET v1.1.4322 kullanacak biçimde yapılandırılmazsa, günlük veritabanına hiçbir bilgi kaydedilmez ve bu da veri kaybına neden olur. |
  
Ayrýca Bkz:  
-----------
  
####  
  
[Veritabanı Sunucusu Altyapısını Planlama](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
