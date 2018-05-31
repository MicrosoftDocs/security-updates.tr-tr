---
TOCTitle: RMS Kurulumu Sırasında Güvenlik
Title: RMS Kurulumu Sırasında Güvenlik
ms:assetid: '0a3d40b2-f27e-4e63-baff-a9c8433f5f91'
ms:contentKeyID: 18124998
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720192(v=WS.10)'
---

RMS Kurulumu Sırasında Güvenlik
===============================

RMS dosyalarını yüklemek ve yapılandırmak için, RMS Kurulumu oturum açmış olan kullanıcının kimlik bilgilerini kullanır. Bu amaç doğrultusunda, yükleme yordamını gerçekleştiren yöneticinin, yerel Administrators grubunun üyesi olan bir kullanıcı hesabıyla oturum açması gerekir. Bu ayrıca, tek bilgisayar yüklemeleri dışındaki tüm yüklemeler için bir etki alanı kullanıcı hesabı olmalıdır.

Yükleme yordamı sırasında Windows Installer hizmeti (Msiexec.exe) başlatılır. Bu hizmet, kendi üst kullanıcısının simgesini devralır. Ardından, işlem sonrası özel eylemler varsa, Msiexec.exe hizmeti oturum açan kullanıcının kimliğini kullanır. Bu, işlemin bir tarayıcıdan veya komut satırından başlatılmasına bağlı olmaksızın gerçekleşir.

RMS Kurulumu aşağıdaki görevleri gerçekleştirir:

-   Dosyaları C:\\Program Files\\RMS klasörüne kopyalar. Bu klasör normalde Administrators ve Power Users üyelerinin erişimine olanak sağlar. Sürücü ve dosya konumunu Kurulum sırasında yapılandırabilirsiniz.
-   Sağlama Web sitesi olan RMS Yönetim Web sitesini varsayılan olarak 5720 numaralı bağlantı noktasında oluşturur. Bu Web sitesi yüklenen dosyaları gösterir.
-   WMCSProvisioningAppPool adlı uygulama havuzunu oluşturur ve bunu RMS Yönetim Web sitesiyle ilişkilendirir. Bu uygulama havuzu tarafından kullanılan hizmet hesabı, Ağ Hizmetleri hizmet hesabıdır.
-   Performans sayaçlarını yükler.
-   RMS Service Group'a aşağıdaki kayıt defteri anahtarı için Okuma ve Yazma izni verir.
    Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda
    `HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0`
    Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda
    `HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0`
