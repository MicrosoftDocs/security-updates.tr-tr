---
TOCTitle: RMS Sunucularının Güvenliğini Sağlama
Title: RMS Sunucularının Güvenliğini Sağlama
ms:assetid: '7e6c4d3a-6cfb-4e96-9dda-ead83f961a6e'
ms:contentKeyID: 18125162
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747574(v=WS.10)'
---

RMS Sunucularının Güvenliğini Sağlama
=====================================

RMS sunucularınızda bulunan kullanıcı hesaplarını ve güvenlik ayarlarını yönetmek için aşağıdaki önerilerden yararlanabilirsiniz:

-   RMS'yi yönetmek için kullandığınız Web sitesinin sanal dizinlerinde, erişimi yerel yöneticilerle sınırlandıran isteğe bağlı erişim denetim listeleri (DACL) vardır. Bir yerel yönetici, üye ekleyip kaldırarak ve yönetim Web sayfalarındaki ek erişim denetim girdilerini (ACE) kullanarak erişimi daha fazla denetlemek üzere ek bir güvenlik grubu oluşturabilir.
-   Daha iyi güvenlik sağlamak için Güvenlik Ayarları Web sayfasının (SecurityPolicy.aspx) DACL ayarlarını değiştirin. Hazırlığa izin vermek için varsayılan ACE, RMS'yi hazırlayan hesaba tam denetleme izni verir. Hazırlıktan sonra ACE'yi kişi veya sınırlı güvenlik grubuna değiştirmeniz gerekir.
-   Her RMS sunucusuna yönelik izin ve haklara ek olarak, tüm dağıtımı güven altına alma konusunda büyük bir öneme sahip olan yapılandırma veritabanının güvenlik gereksinimlerine özel dikkat gösterin. Daha fazla bilgi için bu konuda daha sonra yer alan "[Yapılandırma Veritabanının Güvenliğini Sağlama](https://technet.microsoft.com/e023b96f-81d0-45fb-8cc5-becaf6d47ae1)" bölümüne bakın.

**Microsoft® SQL Server™ güvenliğinin** nasıl sağlanacağı konusunda daha fazla bilgi için [Microsoft Web sitesinde](http://www.microsoft.com/)(http://www.microsoft.com/) bulunan SQL Server Güvenliği Web sayfasına bakın.

Microsoft® Windows Server 2003 işletim sistemi ailesinin bir üyesini çalıştıran bilgisayarların güvenliğinin nasıl sağlanacağı konusunda daha fazla bilgi için [Microsoft Web sitesinde](http://www.microsoft.com/)(http://www.microsoft.com/) bulunan Microsoft Yükleme Merkezi'nden "Windows Server 2003 Güvenlik Kılavuzu"nu edinin.
