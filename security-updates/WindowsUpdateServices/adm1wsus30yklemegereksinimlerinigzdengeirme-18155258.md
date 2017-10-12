---
TOCTitle: 'Adım 1: WSUS 3.0 Yükleme Gereksinimlerini Gözden Geçirme'
Title: 'Adım 1: WSUS 3.0 Yükleme Gereksinimlerini Gözden Geçirme'
ms:assetid: '912b37d7-021e-4c95-b317-49dd15b4611c'
ms:contentKeyID: 18155258
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708484(v=WS.10)'
---

Adım 1: WSUS 3.0 Yükleme Gereksinimlerini Gözden Geçirme
========================================================

Bu kılavuzda WSUS 3.0'ın nasıl yükleneceği anlatılmaktadır. WSUS 3.0 ile ilgili sistem gereksinimleri ve desteklenen platformlar için, Windows Server 2003 Service Pack 1 ve Windows Server® 2008 işletim sistemlerinde Sürüm Notları'na ([http://go.microsoft.com/fwlink/?LinkId=71220](http://go.microsoft.com/fwlink/?linkid=71220)) bakın.

Windows Server 2003 Service Pack 1 Üzerine WSUS 3.0 Yüklemeyle İlgili Yazılım Gereksinimleri
--------------------------------------------------------------------------------------------

Windows Server 2003 Service Pack 1 üzerine WSUS 3.0 yüklemek için bilgisayarınızda aşağıdakiler yüklü olmalıdır. Bu güncelleştirmelerden herhangi biri yükleme tamamlandıktan sonra sunucunun yeniden başlatılmasını gerektiriyorsa, WSUS 3.0'ı yüklemeden önce sunucunuzu yeniden başlatmalısınız.

-   Microsoft Internet Information Services (IIS) 6.0.
-   Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0 ve WinHTTP 5.1 Windows Server 2003 için Güncelleştirme. Bu yazılımı karşıdan yüklemek için Yükleme Merkezi'ne gidin ([http://go.microsoft.com/fwlink/?LinkID=47251](http://go.microsoft.com/fwlink/?linkid=47251)).
-   Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x86). Bu yazılımı karşıdan yüklemek için, Yükleme Merkezi'ne ([http://go.microsoft.com/fwlink/?LinkID=68935](http://go.microsoft.com/fwlink/?linkid=68935)) gidin. (64-bit platformlar için de Yükleme Merkezi'ne ([http://go.microsoft.com/fwlink/?LinkID=70637](http://go.microsoft.com/fwlink/?linkid=70637)) gidin.)
-   Microsoft Report Viewer Redistributable 2005. Bu yazılımı edinmek için, Yükleme Merkezi'ne gidin ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Windows Server 2003 için Microsoft Yönetim Konsolu 3.0 (KB907265). Bu yazılımı karşıdan yüklemek için, Yükleme Merkezi'ne ([http://go.microsoft.com/fwlink/?LinkID=70412](http://go.microsoft.com/fwlink/?linkid=70412)) gidin. (64-bit platformlar için de Yükleme Merkezi'ne ([http://go.microsoft.com/fwlink/?LinkID=70638](http://go.microsoft.com/fwlink/?linkid=70638)) gidin.)

Windows Server 2008 Üzerine WSUS 3.0 Yüklemeyle İlgili Yazılım Gereksinimleri
-----------------------------------------------------------------------------

Windows Server 2008 üzerine WSUS 3.0 yüklemek için bilgisayarınızda aşağıdakiler yüklü olmalıdır. Bu güncelleştirmelerden herhangi biri yükleme tamamlandıktan sonra sunucunun yeniden başlatılmasını gerektiriyorsa, WSUS 3.0'ı yüklemeden önce sunucunuzu yeniden başlatmalısınız.

-   Microsoft Internet Information Services (IIS) 7,0. Aşağıdaki bileşenlerin etkinleştirildiğinden emin olun:
    -   Windows Kimlik Doğrulaması
    -   ASP.NET
    -   6.0 Yönetim Uyumluluğu
    -   IIS Metatabanı Uyumluluğu
-   Microsoft Report Viewer Redistributable 2005. Bu yazılımı karşıdan yüklemek için, Yükleme Merkezi'ne gidin ([http://go.microsoft.com/fwlink/?LinkID=70410](http://go.microsoft.com/fwlink/?linkid=70410)).
-   Microsoft SQL Server™ 2005 Service Pack 1. Bu yazılımı karşıdan yüklemek için, Yükleme Merkezi'ne gidin ([http://go.microsoft.com/fwlink/?LinkID=66143](http://go.microsoft.com/fwlink/?linkid=66143)).

.NET Framework 2.0 ve BITS 2.0 güncelleştirmesi işletim sisteminin bir parçası olarak Windows Server 2008 üzerinde bulunmaktadır.

Disk gereksinimleri ve öneriler
-------------------------------

WSUS 3.0'ı yüklemek için sunucunun dosya sistemi aşağıdaki gereksinimleri karşılamalıdır:

-   Hem sistem bölümü hem de WSUS 3.0'ı yüklediğiniz bölüm, NTFS dosya sistemiyle biçimlendirilmiş olmalıdır.
-   Sistem bölümü için en az 1 GB boş alan bulunması önerilir.
-   WSUS'nin içeriğini depoladığı birimde en az 20 GB boş alan bulunması gerekir; 30 GB boş alan bulunması önerilir.
-   WSUS Kurulumu'nun Windows® İç Veritabanı uygulamasını yüklediği birimde en az 2 GB boş alan bulunması önerilir.

Yalnızca konsol yüklemesi gereksinimleri
----------------------------------------

WSUS 3.0 şimdi WSUS sunucusundan ayrı olarak uzak sistemlere WSUS Yönetim konsolunu yüklemenize olanak tanımaktadır. Yalnızca konsol yüklemeleri aşağıdaki işletim sistemlerinde gerçekleştirilebilir:

-   Windows Server® 2008
-   Windows Vista®
-   Windows Server 2003 Service Pack 1
-   Windows XP Service Pack 2

Yalnızca konsol yüklemelerinin yazılım gereksinimleri aşağıda verilmiştir

-   Microsoft Yükleme Merkezi'nde bulunan Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x86) ([http://go.microsoft.com/fwlink/?LinkId=68935](http://go.microsoft.com/fwlink/?linkid=68935)). 64-bit platformlar için, Microsoft .NET Framework Sürüm 2.0 Yeniden Dağıtılabilir Paketi (x64) sayfasına ([http://go.microsoft.com/fwlink/?LinkId=70637](http://go.microsoft.com/fwlink/?linkid=70637)) gidin.
-   Microsoft Yükleme Merkezi'nde bulunan Windows Server 2003 için Microsoft Yönetim Konsolu 3.0 (KB907265) ([http://go.microsoft.com/fwlink/?LinkId=70412](http://go.microsoft.com/fwlink/?linkid=70412)). 64-bit platformlar için, Windows Server 2003 x64 Edition için Microsoft Yönetim Konsolu 3.0 (KB907265) sayfasına ([http://go.microsoft.com/fwlink/?LinkId=70638](http://go.microsoft.com/fwlink/?linkid=70638)) gidin.
-   Microsoft Yükleme Merkezi'nde bulunan Microsoft Report Viewer Redistributable 2005 ([http://go.microsoft.com/fwlink/?LinkId=70410](http://go.microsoft.com/fwlink/?linkid=70410)).

Otomatik Güncelleştirmeler gereksinimleri
-----------------------------------------

Otomatik Güncelleştirmeler, WSUS 3.0'ın istemci bileşenidir. Otomatik Güncelleştirmeler'in ağa bağlı olmak dışında donanım gereksinimi yoktur. Aşağıdaki işletim sistemlerinden herhangi birini çalıştıran bir bilgisayarda Otomatik Güncelleştirmeler'i WSUS 3.0 ile kullanabilirsiniz:

-   Windows Vista.
-   Windows Server® 2008.
-   Microsoft Windows® Server 2003, tüm sürümleri ve hizmet paketleri.
-   Microsoft Windows XP Professional Service Pack 1 veya Service Pack 2.
-   Microsoft Windows 2000 Professional Service Pack 4, Windows 2000 Server Service Pack 4 veya Windows 2000 Advanced Server Service Pack 4.

İzinler
-------

Aşağıdaki disk izinlerinin belirtilen dizinler için belirtilen kullanıcılara verilmiş olması gerekir:

1.  Yerleşik Users grubunun ya da NT Authority\\Network Service hesabının (Windows Server 2003'te), WSUS içerik dizininin bulunduğu sürücünün kök dizininde okuma izni olmalıdır. Bu izin yoksa, BITS karşıdan yüklemeleri başarısız olur.
2.  NT Authority\\Network Service hesabının, WSUS içerik dizininde (genellikle &lt;SistemSürücüsü&gt;:WSUS\\WsusContent) "Tam Denetim" izni olmalıdır. Bu izin WSUS sunucusu kurulumu tarafından dizini oluşturduğunda ayarlanır, ancak bazı güvenlik yazılımları bu izni sıfırlayabilir. Bu izin yoksa, BITS karşıdan yüklemeleri başarısız olur.
3.  WSUS Yönetimi ek bileşeninin doğru şekilde görüntülenmesi için, NT Authority\\Network Service hesabının aşağıdaki dizinlerde "Tam Denetim" izni olmalıdır:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp

İzinleri ayarlama hakkında daha fazla bilgi için, DCPROMO Bazı IIS Klasörlerinde İzinleri Korumuyor makalesine bakın ([http://go.microsoft.com/fwlink/?LinkID=76332](http://go.microsoft.com/fwlink/?linkid=76332)).
