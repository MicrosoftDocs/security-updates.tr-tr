---
TOCTitle: Sınama Ortamını Kurma
Title: Sınama Ortamını Kurma
ms:assetid: 'cdd96b05-49e2-4b6f-bfae-40b5c028ec66'
ms:contentKeyID: 18125272
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747673(v=WS.10)'
---

Sınama Ortamını Kurma
=====================

RMS varolan Active Directory altyapınızla ve Microsoft SQL Server™ 2000 çalıştıranlar gibi veritabanı sunucularınızla tümleştirilir. Bu destekleyici bileşenlerin kritik yapısı nedeniyle, RMS'yi kuruluşunuzda dağıtmadan önce ayrı bir sınama ortamında tam olarak sınamanız gerekir. Bu, sınama ortamında ayrıca Active Directory ve veritabanı sunucusu yüklemeleri kurmanızı gerektirir.

Bir ormanda bulunan ve bir veritabanı sunucusuyla bir istemciden oluşan en temel RMS sunucusu yapılandırmasıyla başlayın. RMS'yi tanıdıkça, kuruluşunuzun üretim ortamında dağıtacağınız topolojiye daha uygun olacak şekilde, gerektiğinde birçok orman ve dış erişim de ekleyerek yapılandırmanızı büyütebilirsiniz. Sınama ortamı kuruluş dağıtım planının tüm artıklık ve çoklu site yapılandırmalarını içermeyebilir, ancak dağıtmanız gereken tüm destekleyici bileşenleri çalıştıran en az bir sunucu içermelidir.

Aşağıdaki listede temel RMS yapılandırmasını sınamak için kullanabileceğiniz sınama ortamına yönelik olası en düşük yapılandırma açıklanmaktadır:

-   Windows 2000 Server Service Pack 3 (SP3) veya daha ileri bir sürümü çalıştıran ve SQL Server 2000 SP3a yüklü bir etki alanı denetleyicisi. SQL Server RMS günlük, yapılandırma ve dizin hizmetleri veritabanlarını barındırır. RMS, Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A ile, veya veritabanı RMS ile aynı sunucuda olacaksa SQL Server ile kullanılabilir. Veritabanı desteği için uzak sunucu kullanacaksanız, SQL Server gereklidir. MSDE 2000'i Microsoft Web sitesinden yükleyebilirsiniz.

| ![](images/Cc747673.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Etki alanı denetleyicisi için en düşük gereksinim Windows 2000 Server Service Pack 3 (SP3) olmakla birlikte, Active Directory grup genişletmesindeki performans geliştirmeleri nedeniyle Windows Server 2003 önerilir. MSDE 2000'in RMS veritabanlarını sadece deneme ortamlarını desteklemek için kullanılması önerilir, çünkü MSDE 2000 ağ arabirimlerini desteklemez. Ayrıca, MSDE 2000 kullanım koşullarında, MSDE 2000'i değiştirmek için SQL Server istemci araçlarını kullanamayacağınız belirtilmektedir. Bu sınırlamayla, günlük bilgilerini görüntüleyemeyecek veya yapılandırma veritabanında depolanmış verileri değiştirmeyeceksiniz. |

-   RMS'nin yüklenmiş ve sağlanmış olduğu, Windows Server 2003 çalıştıran kök sertifika sunucusu. İstiyorsanız, sınama ilerledikçe kök sertifika kümesi oluşturmak için daha fazla sunucu ekleyebilirsiniz.
-   Windows XP Professional, RMS istemcisi ve RMS etkin bir uygulama çalıştıran istemci bilgisayar.
-   Active Directory'de e-posta adresi özniteliği olan kullanıcı hesapları.

Temel RMS altyapısını yükleme ve yapılandırma ile altyapı gereksinimlerinin üretim ortamına nasıl uygulanacağı hakkında bilgi için, bu konuda daha sonra yer alan "[Temel Altyapıyı Kurma](https://technet.microsoft.com/3a0a3a47-e755-4455-bb22-0e05053723e4)" bölümüne bakın.
