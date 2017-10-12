---
TOCTitle: Günlük Boyutunu Yönetme
Title: Günlük Boyutunu Yönetme
ms:assetid: '431b32b3-02f0-4666-b52c-183eb65154fd'
ms:contentKeyID: 18125071
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720271(v=WS.10)'
---

Günlük Boyutunu Yönetme
=======================

Günlük hizmeti SQL Server veritabanına büyük miktarda veri gönderir. Veriler için yeterli disk kapasitesi bulunduğundan emin olmak için günlük veritabanınızı düzenli olarak denetlemeniz gerekir. Veri miktarının fazla olduğunun ve raporlama gereksinimlerinizin bazı bilgileri gerektirmediğinin farkına varırsanız, SQL Server filtrelerinin günlük dosyalarını yalnızca gereksinim duyduğunuz günlükleri saklayacak şekilde azaltmasını sağlayabilirsiniz. Günlük bilgilerini süzme hakkındaki yönergeler için bkz: SQL Server Enterprise Manager Yardımı.

Kullanılabilir disk alanı açısından günlük veritabanınızın çok fazla büyüdüğünü fark ederseniz, günlük veritabanını, bu konuda daha sonra yer alan "[Günlük Veritabanının Yerini Değiştirme](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)" bölümünde açıklandığı şekilde farklı bir sunucuya taşıyabilirsiniz.

| ![](images/Cc720271.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Giden günlük ileti sırasının boyutunu düzenli olarak izlemek için ayrıca Sistem Monitörü'nü kullanmalısınız. Sıra boyutu ciddi miktarda büyürse, günlük dinleyici hizmetinin doğru şekilde çalıştığını doğrulayın. Sistem Monitörü'nü kullanma hakkında daha fazla bilgi için bkz: Windows Server 2003 Yardım ve Destek Merkezi. |
