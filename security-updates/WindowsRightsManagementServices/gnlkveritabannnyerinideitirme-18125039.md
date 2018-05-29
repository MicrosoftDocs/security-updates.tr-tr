---
TOCTitle: Günlük Veritabanının Yerini Değiştirme
Title: Günlük Veritabanının Yerini Değiştirme
ms:assetid: '34ea8045-dc94-422e-9601-29927cfc1534'
ms:contentKeyID: 18125039
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720238(v=WS.10)'
---

Günlük Veritabanının Yerini Değiştirme
======================================

Varsayılan RMS yapılandırması, yapılandırma veritabanı ve günlük veritabanını aynı sunucuya yerleştirir. SQL Server'ın günlük ve yapılandırma veritabanları için yeterli alana sahip olduğundan emin olmak için düzenli olarak denetim yapın.

Günlük veritabanı çok fazla büyürse, istediğiniz an bu veritabanını farklı bir sunucuya taşıyabilirsiniz. Yönetim Web sitesini kullanarak günlük veritabanının konumunu değiştirmeniz mümkün değildir; bunun yerine aşağıdaki adımları izleyerek bu işlemi el ile yapmanız gerekir:

1.  Günlüğü, bu konuda daha sonra yer alan "[Günlüğü Açmak veya Kapatmak için](https://technet.microsoft.com/8e672f95-566f-4070-9a2a-2f70f087148f)" bölümünde açıklandığı şekilde kapatın.
2.  SQL Server Enterprise Manager'ı kullanarak günlük veritabanını kaynak sunucudan hedef sunucuya kopyalayın. Tabloların ve saklı yordamların yeni veritabanında oluşturulduğundan emin olun. Bunu yapmanın bir yolu SQL Server Enterprise Manager Copy Database Wizard'ı kullanmaktır.
3.  Yapılandırma veritabanını yeni sunucu ve veritabanı adlarını yansıtacak şekilde değiştirin. Veritabanını taşıdığınız kümenin yapılandırma veritabanındaki DRMS\_ClusterPolicies tablosunda aşağıdakileri yapın:
    -   LoggingDatabaseServer ilkesinin değerini yeni veritabanı sunucusunun adını yansıtacak şekilde değiştirin.
    -   LoggingDatabaseName ilkesinin değerini yeni veritabanının adını yansıtacak şekilde değiştirin.

    | ![](/security-updates/images/Cc720238.note(WS.10).gif)Not                                                                                                                                                           |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | SQL Server Enterprise Manager, db\_variant alanlarla çalışmadığından, bu görev için kullanılamaz. Bunun yerine, SQL Server'la birlikte verilen Query Analyzer'ı veya başka bir veritabanı düzenleme aracını kullanabilirsiniz. |

4.  Kümede bulunan tüm sunucularda IIS'yi yeniden başlatın.
5.  Günlüğü tekrar etkinleştirin.
