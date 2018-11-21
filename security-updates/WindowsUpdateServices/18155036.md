---
TOCTitle: 'Adım 1: WSUS Yükleme Gereksinimlerini Gözden Geçirme'
Title: 'Adım 1: WSUS Yükleme Gereksinimlerini Gözden Geçirme'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18155036
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720547(v=WS.10)'
---

Adım 1: WSUS Yükleme Gereksinimlerini Gözden Geçirme
====================================================

Bu kılavuz, Microsoft Windows Server 2003 işletim sistemlerine (Web Edition ve tüm 64 bit sürümler dışında) Microsoft Windows Server Update Services (WSUS) yükleme yönergesi sağlar. Microsoft Windows 2000 Server çalıştıran bir sunucunuz varsa ve daha fazla bilgiye gereksinim duyuyorsanız, “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir).

Aşağıda varsayılan seçenekleri kullanan yüklemelere yönelik temel yükleme gereksinimleri vardır. Diğer yüklemelere yönelik yazılım ve donanım gereksinimlerini “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesinde bulabilirsiniz (Belge İngilizce'dir).

500 istemciye kadar hizmet veren bir sunucu için donanım gereksinimleri aşağıdadır:

-   1 gigahertz (GHz) işlemci
-   1 gigabayt (GB) RAM

Yazılım Gereksinimleri
----------------------

WSUS'yi varsayılan seçeneklerle yüklemek için, aşağıdaki uygulamaların bilgisayarınıza yüklü olması gerekir. WSUS yazılım gereksinimleri hakkında daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir). Bu güncelleştirmelerden herhangi biri yükleme tamamlandıktan sonra bilgisayarın yeniden başlatılmasını gerektiriyorsa, WSUS'yi yüklemeden önce sunucunuzu yeniden başlatmalısınız.

-   Microsoft Internet Information Services (IIS) 6.0. IIS'yi yükleme konusundaki yönergeler için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine (Belge İngilizce'dir) veya Windows Server 2003'teki Yardım ve Destek Merkezi'ne bakın.
-   Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1. Bu yazılımı elde etmek için http://go.microsoft.com/fwlink/?LinkId=47358 adresindeki [Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=47358)'ne bakın.
    Bir diğer yol ise, http://www.windowsupdate.com adresine gidip Kritik Güncelleştirmeler ve Hizmet Paketleri'ni aradıktan sonra Windows Server 2003 için Microsoft .NET Framework 1.1 Service Pack 1'i yüklemektir.
-   Arka Plan Akıllı Aktarım Hizmeti (BITS) 2.0. Windows Server 2003 için BITS 2.0 şu anda Yükleme Merkezi sitesinde yoktur. Bu yazılımı elde etmek için http://go.microsoft.com/fwlink/?LinkId=47357 adresindeki, Windows Server Update Services Open Evaluation'a yönelik [Microsoft Web sitesine](http://go.microsoft.com/fwlink/?linkid=47357) bakın.

| ![](/security-updates/images/Cc720547.note(WS.10).gif)Not                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| WSUS'yi yüklemek için veritabanı yazılımı gerekir, ancak Windows Server 2003 üzerinde gerçekleştirilen varsayılan WSUS yüklemesi, Windows SQL Server™ 2000 Desktop Engine (WMSDE) veritabanı yazılımını da içerdiğinden burada listelenmemiştir. |

Disk Gereksinimleri ve Öneriler
-------------------------------

WSUS'yi yüklemek için sunucunun dosya sistemi aşağıdaki gereksinimleri karşılamalıdır:

-   Hem sistem bölümü hem de WSUS'yi yüklediğiniz bölüm, NTFS dosya sistemiyle biçimlendirilmelidir.
-   Sistem bölümü için en az 1 GB boş alan gereklidir.
-   WSUS'nin içeriği depoladığı birimde en az 6 GB boş alan bulunması gerekir; 30 GB önerilir.
-   WSUS Kurulumu'nun Windows SQL Server 2000 Desktop Engine (WMSDE) uygulamasını yüklediği birimde en az 2 GB boş alan bulunması gerekir.

Otomatik Güncelleştirmeler Gereksinimleri
-----------------------------------------

Otomatik Güncelleştirmeler WSUS'nin istemci bileşenidir. Otomatik Güncelleştirmeler'in ağa bağlı olmak dışında donanım gereksinimi yoktur. Aşağıdaki işletim sistemlerinden herhangi birini çalıştıran bir bilgisayarda Otomatik Güncelleştirmeler'i WSUS ile kullanabilirsiniz:

-   Microsoft Windows 2000 Professional Service Pack 3 (SP3) veya Service Pack 4 (SP4), Windows 2000 Server SP3 veya SP4 ya da Windows 2000 Advanced Server SP3 veya SP4.
-   Microsoft Windows XP Professional, Service Pack 1 veya Service Pack 2 yüklü veya yüklü değil.
-   Microsoft Windows Server 2003 Standard Edition; Windows Server 2003 Enterprise Edition; Windows Server 2003 Datacenter Edition veya Windows Server 2003 Web Edition.
