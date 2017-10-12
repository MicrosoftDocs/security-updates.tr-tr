---
TOCTitle: Hak İlkesi Şablonlarını Yedekleme ve Geri Yükleme
Title: Hak İlkesi Şablonlarını Yedekleme ve Geri Yükleme
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18125227
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747625(v=WS.10)'
---

Hak İlkesi Şablonlarını Yedekleme ve Geri Yükleme
=================================================

Önemli hak ilkesi şablonlarını korumak için, yapılandırma veritabanındaki şablon verilerini düzenli olarak bir ortama yedekleyin ve bu ortamı güvenli bir yere koyun. Bir sistem hatası oluşursa, hak ilkesi şablonlarını yedek kopyanızdan geri yükleyebilirsiniz.

Aşağıdakilerden birini yapın:

-   Hak ilkesi şablonu verilerinin bulunduğu yapılandırma veritabanını tamamen yedekleyin. SQL Server veritabanı yedekleme hakkında daha fazla bilgi için SQL Server belgelerine bakın.
    -veya-
-   Yalnızca yapılandırma veritabanındaki hak ilkesi şablonu verilerini yedekleyin. Bunu, GUID ve TemplateData bilgilerini DRMS\_RightsTemplate adındaki tablodan yeni bir metin dosyasına aktararak yapabilirsiniz. SQL Server veritabanından veri verme hakkında daha fazla bilgi için SQL Server belgelerine bakın.

Yapılandırma veritabanındaki hak ilkesi şablonu verilerini geri yüklemeniz gerekiyorsa, yapılandırma veritabanının yedek kopyasındaki DRMS\_RightsTemplate adındaki tablodan GUID ve TemplateData bilgilerini ayıklayabilir veya basitçe verileri metin dosyasından alabilirsiniz. Bu görevleri yerine getirme hakkında daha fazla bilgi için SQL Server belgelerine bakın.

| ![](images/Cc747625.note(WS.10).gif)Not                            |
|-------------------------------------------------------------------------------------------------|
| Hak ilkesi şablonlarını yedeklemek üzere bir plan yapmak için SQL Server yöneticinize başvurun. |
