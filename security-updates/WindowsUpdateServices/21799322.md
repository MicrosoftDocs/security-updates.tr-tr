---
TOCTitle: 'Adım 1: WSUS 3.0 SP2 Yükleme Gereksinimlerini Onaylama'
Title: 'Adım 1: WSUS 3.0 SP2 Yükleme Gereksinimlerini Onaylama'
ms:assetid: 'ec01bd75-5def-4899-8cee-ddab827bbd83'
ms:contentKeyID: 21799322
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939916(v=WS.10)'
---

Adım 1: WSUS 3.0 SP2 Yükleme Gereksinimlerini Onaylama
======================================================

Windows Server Upgrade Services 3.0 Service Pack 2'yi (WSUS 3.0 SP2) yüklemeden veya bu sürüme yükseltme yapmadan önce, hem sunucunun hem de istemci bilgisayarların WSUS 3.0 SP2 sistem gereksinimlerini karşıladığını ve yüklemeyi tamamlamak için gerekli izinlere sahip olduğunuzu onaylarsınız.

WSUS 3.0 SP2 Yüklemesi için Sunucu Donanımı ve Yazılım Gereksinimleri
---------------------------------------------------------------------

1.  Sunucunun, donanım, işletim sistemi ve diğer gerekli yazılımlara yönelik sistem gereksinimlerini karşıladığını onaylayın. Sistem gereksinimleri, [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) adresindeki WSUS 3.0 SP2 Sürüm Notları'nda listelenmektedir. WSUS 3.0 SP2 Server yüklemek için Sunucu Yöneticisi'ni kullanıyorsanız, “WSUS 3.0 SP2 Yüklemeye Hazırlanma” bölümündeki adımları izleyerek yazılım gereksinimlerini karşıladığınızı onaylayabilirsiniz.
2.  Yükleme tamamlandığında sunucuyu yeniden başlatmanızı gerektiren roller veya yazılım güncelleştirmeleri yüklüyorsanız, WSUS 3.0 SP2'yi yüklemeden önce sunucuyu yeniden başlatın.

İstemci Yazılım Gereksinimleri
------------------------------

Otomatik Güncelleştirmeler, WSUS 3.0'ın istemcisidir. Otomatik Güncelleştirmeler'in ağa bağlı olmak dışında donanım gereksinimi yoktur.

1.  Otomatik Güncelleştirmeler'i yüklediğiniz bilgisayarınızın, İstemci bilgisayarlara yönelik WSUS 3.0 SP2 sistem gereksinimlerini karşıladığını onaylayın. Sistem gereksinimleri, [http://go.microsoft.com/fwlink/?LinkId=139840](http://go.microsoft.com/fwlink/?linkid=139840) adresindeki WSUS 3.0 SP2 Sürüm Notları'nda listelenmektedir.
2.  Bilgisayarın yeniden başlatılmasını gerektiren yazılımlar yüklüyorsanız, WSUS 3.0 SP2'yi yüklemeden önce bilgisayarı yeniden başlatın.

İzinler
-------

Belirtilen kullanıcılar ve dizinler için aşağıdaki izinler gereklidir:

1.  WSUS Yönetimi ek bileşeninin doğru şekilde görüntülenmesi için, NT Authority\\Network Service hesabının aşağıdaki klasörler için Tam Denetim izni olmalıdır:
    -   %windir%\\Microsoft .NET\\Framework\\v2.0.50727\\Temporary ASP.NET Files
    -   %windir%\\Temp
2.  WSUS 3.0 SP2 yüklemek için kullanmayı planladığınız hesabın, Yerel Administrators grubunun bir üyesi olduğunu onaylayın.

WSUS 3.0 SP2 Yüklemeye Hazırlanma
---------------------------------

Windows 7 veya Windows Server 2008 SP2 çalıştırıyorsanız, Sunucu Yöneticisi'nden WSUS 3.0 SP2 yükleyebilirsiniz. Başka bir desteklenen işletim sistemini kullanıyorsanız veya yalnızca WSUS Yönetim Konsolu'nu yüklüyorsanız, WUSSetup.exe dosyasını kullanarak WSUS 3.0 SP2'yi yüklemek için bu kılavuzun sonraki bölümüne gidin.

**Sunucu Yöneticisi'ni kullanarak WSUS 3.0 SP2 Server yüklemeye hazırlanmak için**
1.  Üzerine WSUS 3.0 SP2'yi yüklemeyi planladığınız sunucuda, yerel Administrators grubunun üyesi olan bir hesabı kullanarak oturum açın.

2.  **Başlat**'ı tıklatın, **Yönetimsel Araçlar**'ın üzerine gelin ve **Sunucu Yöneticisi**'ni tıklatın.

3.  Sunucu Yöneticisi penceresinin sağ bölmesinde, Rol Özeti bölümünde **Rol Ekle**'yi tıklatın.

4.  Başlamadan Önce sayfası görüntülenirse, **İleri**'yi tıklatın.

5.  Sunucu Rollerini Seç sayfasında, **Uygulama Sunucusu** ve **Web Sunucusu (IIS)** seçeneklerinin belirlendiğini onaylayın. Bu seçenekler belirlenmişse, gerekli rol hizmetlerinin seçildiğini onaylamak için bu adımın kalanını uygulayın. Aksi takdirde, şu şekilde Uygulama Sunucusu'nu ve Web Sunucusu'nu (IIS) yükleyin.

    1.  Sunucu Rollerini Seç sayfasında, **Uygulama Sunucusu** ve **Web Sunucusu (IIS)** seçeneklerini belirleyin. **İleri**'yi tıklatın.
    2.  Uygulama Rol Hizmetleri'ni yüklüyorsanız, Uygulama Sunucusu sayfasında **İleri**'yi tıklatın. Uygulama Sunucusu Rol Hizmetleri sayfasında, varsayılan ayarları kabul edin ve **İleri**'yi tıklatın.
    3.  Web Sunucusu IIS yüklüyorsanız, Web Sunucusu (IIS) sayfasında **İleri**'yi tıklatın. Web Sunucusu (IIS) Rol Hizmetleri sayfasında, varsayılan ayarlara ek olarak **ASP.NET**, **Windows Kimlik Doğrulaması**, **Dinamik İçerik Sıkıştırma** ve **IIS 6 Yönetim Uyumluluğu** seçeneklerini belirleyin. Rol Ekleme Sihirbazı penceresi görüntülenirse, **Gereken Rol Hizmetlerini Ekle**'yi tıklatın. **İleri**'yi tıklatın.
    4.  Yükleme Seçimlerini Onaylama sayfasında **Yükle**'yi tıklatın.
    5.  Yükleme Sonuçları sayfasında, bu adımda yüklediğiniz rol hizmetleri için “Yükleme başarılı” iletisinin görüntülendiğini onaylayın ve sonra **Kapat**'ı tıklatın.

Sonraki adım
------------

[Adım 2: WSUS Sunucusu'nu veya Yönetim Konsolu'nu Yükleme](https://technet.microsoft.com/6db6fcb0-c55d-43b9-9b07-4040c6267759).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
