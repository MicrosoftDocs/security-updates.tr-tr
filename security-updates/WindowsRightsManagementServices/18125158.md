---
TOCTitle: Sunucuları Varolan Yüklemeye Ekleme
Title: Sunucuları Varolan Yüklemeye Ekleme
ms:assetid: '7f3598ff-cd19-4daa-aa65-877f7f95a8ec'
ms:contentKeyID: 18125158
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747648(v=WS.10)'
---

Sunucuları Varolan Yüklemeye Ekleme
===================================

Artan talebi karşılamak veya hizmetten çekilmesi gereken sunucuları değiştirmek için RMS yüklemenize gerektikçe sunucu ekleyebilirsiniz. Her RMS yüklemesinin en az bir kök sertifika sunucusu içermesi gerekir ve söz konusu yükleme, isteğe bağlı olarak kümedeki başka kök sertifika sunucularını içerebilir. Her RMS yüklemesi tek başına çalışan veya kümelenmiş lisans sunucularını da içerebilir.

Aşağıdaki yöntemlerin herhangi birini kullanarak RMS yüklemesine sunucu ekleyebilirsiniz:

-   Kök sertifika kümesine bir veya daha fazla RMS sunucusu ekleme.
-   Yeni bir tek başına çalışan lisans sunucusu ekleme.
-   Lisans kümesine bir veya daha fazla RMS sunucusu ekleme.

**Kök Sertifika Sunucuları Ekleme**

Çoğu amaca yönelik olarak, kök sertifika kümesine bir veya daha fazla RMS sunucusu eklemek dağıtımınızın kullanılabilirliğini ve artıklığını artırmanın en iyi yoludur. Bir kök sertifika kümesi, bir veya daha fazla kök sertifika sunucusundan oluşur. Yalnızca lisans ve yayımlama hizmetleri sağlayan lisans sunucularının aksine, kök sertifika sunucuları tüm RMS hizmetlerini sağlar.

Yükleme ve hazırlık sırasında, kümeye sunucu ekle seçeneğini seçebilirsiniz. Bunu yaptığınızda, yeni RMS sunucusu otomatik olarak küme üyesi biçiminde yapılandırılır. Kök sertifika kümesine eklemek üzere RMS sunucusu yükleme ve sağlama hakkında adım adım yönergeler için, bu konuda daha sonra yer alan "[RMS Service Pack 1 Yüklemek için](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)" ve "[Kümeye Sunucu Eklemek için](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)" bölümlerine bakın.

Bu hazırlık adımına ek olarak, ilk kez bir küme oluşturuyorsanız, gerektiğinde küme oluşturma ve yük dengelemeyle birlikte yazılımı veya donanımı da kurmanız gerekir. Zaten bir küme uyguladıysanız, yük dengeleme yazılımı veya donanımınızı yeni küme üyesiyle birlikte çalışacak şekilde yapılandırmanız gerekir.

**Lisans Sunucuları Ekleme**

Tüm RMS hizmetlerini sağlayan kök sertifika sunucusunun aksine, lisans sunucusu yalnızca lisans ve yayımlama hizmetleri sağlar.

Lisans sunucuları isteğe bağlıdır ve genellikle aşağıdakiler gibi belirli lisans gereksinimlerini karşılamak için dağıtılır:

-   Bir bölümün benzersiz hak yönetimi gereksinimlerini destekleme. Örneğin, kuruluşunuzdaki bir grubun diğerlerine göre hak yönetimi açısından farklı güvenlik gereksinimleri olabilir ve gruplarına yönelik lisans uygulaması üzerinde tam denetime sahip olmak isteyebilir. Bir ormanda yalnızca bir kök sertifika sunucusuna izin verildiği için, ayrı bir kök sertifika sunucusunun kurulması uygun olmayabilir. Bu durumda, bu grubun gereksinimlerine ayrılmış bir lisans sunucusu veya lisans kümesi kurabilirsiniz. Ardından, bu lisans sunucusu veya kümesi için hak ilkelerini ayrı ayrı ayarlayabilirsiniz.
-   Sağlam ayrımı ve belirli iş ortaklarına yönelik kaynakların izlenmesini gerektiren bir extranet'in parçası olarak, dış iş ortakları için hak yönetimini destekleme. Daha fazla bilgi için bu konuda daha sonra yer alan "[Extranet URL'sini Yapılandırma](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)" bölümüne bakın.
-   Kök sertifika sunucusundaki lisans görevlerinin yükünü azaltma. Bu yalnızca tek kök sertifika sunucusuna (kök sertifika kümesi yerine) sahip kuruluşlarda performans faydaları sağlayabilir.

Çoğu amaç için, dağıtımınızda bulunan tüm sunucularda artıklık ve yük dengelemesini kurabileceğiniz için RMS sunucularını kök sertifika kümesine eklemeniz önerilir. Lisans sunucularının lisans ve yayımlama isteklerinin işleme yükünü azaltmak için kullanılabilmesine rağmen, lisans sunucuları kök sertifika kümesiyle yükü dengelenmiş hale getirilemez. Lisans sunucularını ayrı olarak dağıtma gereksinimi olmadıkça, tüm RMS sunucularını kök sertifika kümesinin üyesi yaparak yükü dengelemek daha iyidir.

RMS lisans sunucusu yükleme ve sağlama hakkında adım adım yönergeler için, bu konuda daha sonra yer alan "[RMS Service Pack 1 Yüklemek için](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d)" ve "[Lisans Sunucusu Sağlamak için](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e)" bölümlerine bakın.
