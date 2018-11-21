---
TOCTitle: RMS Tarafından Kullanılan Veritabanlarının Güvenliğini Sağlama
Title: RMS Tarafından Kullanılan Veritabanlarının Güvenliğini Sağlama
ms:assetid: '65802f9a-81bc-4398-968a-00c9b1dca2fa'
ms:contentKeyID: 18125123
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720285(v=WS.10)'
---

RMS Tarafından Kullanılan Veritabanlarının Güvenliğini Sağlama
==============================================================

RMS, aşağıda belirtildiği şekilde değişen güvenlik gereksinimlerine sahip üç veritabanı oluşturur ve kullanır:

-   **Dizin hizmetleri**. Bu veritabanı, Active Directory grup üyeliği sorgularının sonuçlarını önbelleğe alır. Yalnızca Active Directory bilgilerini içerdiği için, RMS sağlama işlemi sırasında otomatik olarak yapılandırılanın dışında ek güvenlik gereksinimi yoktur.
-   **Günlük**. Bu veritabanında bulunan bilgiler, açıklanması durumunda kullanıcı gizliliğini etkileyebileceği için dizin hizmetleri veritabanındaki bilgilere kıyasla daha gizlidir. Microsoft, kişisel olarak tanımlanabilir bilgilerin günlüğe kaydedilmemesi ve bu veritabanında günlüğe kaydedilen tüm bilgilerin uygun güvenlik önlemleriyle korunmasını güvenceye almak için önemli ölçüde çaba göstermektedir. Bu veritabanı SQL Server çalıştıran bir bilgisayara taşınmadıkça ek güvenlik değişikliklerine gereksinim duyulmaz. Veritabanı başka bir sunucuya taşınırsa, aynı koruma mekanizmalarının yeni ortamda da uygulandığından emin olmanız gerekir.
-   **Yapılandırma**. Bu veritabanı, sunucu özel anahtarlarının dışında, RMS dağıtımınızdaki en önemli ve en değerli kaynaktır. Dikkatli bir şekilde korunması gereken gizli ve önemli bilgileri içerir. Bu veritabanı yapılandırma bilgilerine ek olarak tüm sertifika ve anahtarları, şifreli sunucu özel anahtarını (önerilen donanım şifrelemesini kullanmadığınız sürece) ve özel anahtar parola karmasını içerir.

RMS yapılandırma veritabanını oluşturduğunda, erişimi sınırlandıran ve veritabanınızın güvenliğini sağlayan izinleri belirler.

Veritabanı Güvenliğini Artırma
------------------------------

Ağınız ve sunucu ortamınızda bulunan veritabanlarının toplam güvenliğini artırmak için aşağıdaki ek adımları uygulayabilirsiniz:

-   Veritabanı sunucusunu Server 2003 yüklü bir bilgisayarda çalıştırın. Bu işletim sistemi, varsayılan olarak Windows 2000 Server'dan daha güvenlidir. Her ne kadar Windows 2000 Server tabanlı bir bilgisayarı kilitleyebilseniz de, bu, zaman alıcı bir işlem olabilir ve kötü amaçlı kullanıcıların veritabanınıza erişmelerini sağlayacak boşluklar bırakan hatalar yapabilirsiniz.
-   Veritabanı sunucusuna fiziksel erişimi sınırlandırın.
-   Veritabanı dosyalarında bulunan veritabanı izinlerinin ve DACL'lere erişimin yetkili personelle sınırlandırıldığından emin olun. RMS tarafından yapılandırılan varsayılan izinler ve DACL'ler güvenlidir. Varsayılan ayarların herhangi birini değiştirirken dikkatli olun.
-   Microsoft Internet Information Services (IIS), Message Queuing veya Terminal Hizmetleri gibi gerekmeyen hizmetleri veritabanı sunucusunda çalıştırmayın.
-   RMS veritabanları dışındaki veritabanlarını veritabanı sunucusunda çalıştırmayın.

Şifreli kanallar sağlamak üzere SSL veya Internet Protokolü Güvenliği'ni (IPsec) yapılandırarak SQL Server veritabanlarının güvenliğini sağlayın. Veritabanı iletişimlerinin şifrelenmesi kötü niyetli kullanıcıların kayıtlı verileri yakalamasını veya değiştirmesini engellemeye yardımcı olur.

SQL Server için SSL yapılandırma hakkında daha fazla bilgi için MSDN Web sitesine ([http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=17060)) bakın.

SQL Server 2000 için IPsec yapılandırma hakkında daha fazla bilgi için MSDN Web sitesine ([http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=17061)) bakın.

Microsoft Windows Server 2003 ailesi işletim sistemlerinin güvenliğini sağlama hakkında daha fazla bilgi için, Microsoft Yükleme Merkezi'nden "Windows Server 2003 Güvenlik Kılavuzu" adlı belgeyi edinin ([http://go.microsoft.com/fwlink/?LinkId=36719](http://go.microsoft.com/fwlink/?linkid=36719)).
