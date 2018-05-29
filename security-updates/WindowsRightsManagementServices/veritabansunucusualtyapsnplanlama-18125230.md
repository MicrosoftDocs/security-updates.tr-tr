---
TOCTitle: Veritabanı Sunucusu Altyapısını Planlama
Title: Veritabanı Sunucusu Altyapısını Planlama
ms:assetid: 'b12354bd-3143-4d1f-b5aa-450c4550653c'
ms:contentKeyID: 18125230
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747731(v=WS.10)'
---

Veritabanı Sunucusu Altyapısını Planlama
========================================

RMS, işlemlerini desteklemek amacıyla veritabanları ve depolanan yordamlar kullandığından, kuruluşunuzda RMS kullanabilmeniz için veritabanı altyapısı gereklidir. Veritabanı sunucunuz RMS ile aynı sunucuda veya farklı bir sunucuda olabilir. Altyapınızda RMS'yi destekleyecek bir veritabanı sunucusu yoksa, RMS'yi sınamak için veritabanı sunucusu olarak Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) A sürümünü kullanabilirsiniz.

Microsoft SQL Server Desktop Engine, kuruluş çapındaki veritabanını tam olarak çalıştırmak ve desteklemek için gereken araçları içermediğinden, RMS veritabanlarını desteklemek amacıyla yalnızca sınama ortamlarında kullanılması önerilir. Buna ek olarak, MSDE uzak ağları desteklemediğinden, bunu RMS ile aynı sunucuya yüklemeniz gerekir ve RMS kümesine başka RMS sunucuları yükleyemezsiniz. Microsoft SQL Server Desktop Engine kullanım koşullarında, Microsoft SQL Server Desktop Engine veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınız belirtilir. Bu kısıtlama nedeniyle, RMS yapılandırma veritabanını yedekleyemez ve geri yükleyemez, günlük bilgilerini görüntüleyemez veya yapılandırma veritabanında depolanan verileri doğrudan değiştiremezsiniz.

Veritabanlarınızı RMS yüklemenizden farklı bir sunucuya yerleştirmeyi planlıyorsanız, veritabanı desteği sağlamak için SQL Server gibi tam bir veritabanı sunucusu ürünü kullanmanız gerekir. RMS hizmeti hesabına, RMS'yi desteklemek için kullandığınız veritabanı sunucusunda, veritabanlarını okumak, yazmak ve yeni veritabanları oluşturmak üzere uygun izinleri sağladığınızdan emin olun.

RMS, SQL Server 2000 ve MSDE çalıştıran veritabanları için tasarlanmış ve sınanmış olmasına ve Microsoft'un RMS'nin SQL Server 2000 veya MSDE dışında veritabanı sağlayıcıları ile birlikte kullanımını desteklememesine rağmen; RMS, Microsoft .NET Framework tarafından sağlanan ADO.NET arabirimleri kullanan veritabanı sunucularında çalıştırılabilir. Bundan dolayı, diğer veritabanı satıcıları RMS için uygun veritabanı sağlayıcıları geliştirmiş olabilir. İlişkili veritabanının aşağıdaki ölçütlerle uyumlu olması koşuluyla, RMS ile birlikte istediğiniz herhangi bir veritabanını kullanabilirsiniz:

-   Veritabanı Transact-SQL uyumlu olmalıdır, çünkü RMS başlatma komut dosyaları ve depolanmış RMS yordamları Transact-SQL kullanır.
-   Veritabanı sunucusu Microsoft SQL Server'a özgü uzantıları desteklemelidir.

Veritabanı sağlayıcısı aşağıdakileri yapabilmelidir:

-   .NET Framework'ünün System.Data.SqlClient alanının yöntem çağrılarına yanıt verebilmelidir.
-   System.Data.SqlClient ad alanı ile ilişkili işlevsellik sağlamalıdır.
-   SQL kimlik doğrulama yerine Windows Tümleşik Kimlik Doğrulama kullanmalıdır.

RMS'yi farklı bir yapılandırmada kullanıyorsanız, ilgili veritabanı satıcısına veya özelleştirilmiş dağıtımını kullandığınız veritabanı sağlayıcısından yararlandığınız çözüm üreticisine başvurun.

| ![](/security-updates/images/Cc747731.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                                                      |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tüm RMS veritabanları, varsayılan olarak Tam kurtarma özelliği etkin biçimde oluşturulur, ancak işlem günlüğü yedekleme işi oluşturulmaz. Bu, sunucunuzun sabit diskinin dolmasına ve veritabanı sunucusu hatası oluşmasına neden olabilir. Tam kurtarma DRMS\_yapılandırma veritabanı için önerilir, diğer DRMS veritabanları kuruluşunuza uygun başka bir kurtarma modeli kullanmak üzere yapılandırılabilir. |

Bu bölüm şunları kapsar:

-   [Veritabanı Büyümesini Tahmin Etme](https://technet.microsoft.com/87652cc2-b886-4797-8d40-356669768089)
-   [Dizin Hizmetleri Veritabanının Bakımı](https://technet.microsoft.com/911a62f2-c1d6-4091-99b0-b53211be27a7)
-   [Günlük Veritabanının Bakımı](https://technet.microsoft.com/de55058b-0d1a-4997-8a45-e14678ddd13f)
