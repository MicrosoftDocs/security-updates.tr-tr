---
TOCTitle: Çekirdek Bileşenleri Belirleme
Title: Çekirdek Bileşenleri Belirleme
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18125263
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747751(v=WS.10)'
---

Çekirdek Bileşenleri Belirleme
==============================

Uygun topolojiyi oluşturmak için RMS dağıtımının temel bileşenlerini ve bunların rollerini anlamanız önemlidir. Aşağıdaki listede RMS dağıtımınızın parçası olacak sunucular tanımlanmaktadır:

-   Kök sertifika sunucuları. Kök sertifika sunucusu RMS dağıtımının ilk bileşenidir ve diğer tüm bileşenler buna bağlıdır. Kök sertifika sunucusu, kuruluşunuzdaki RMS istemcilerine hak hesabı sertifikaları sağlayan hesap sertifika hizmetini de içerecek şekilde, tüm RMS hizmetlerini çalıştırır. Her Active Directory ormanında yalnızca bir kök sertifika sunucusu olabilir. Ancak, artıklık ve yük dengelemesi için kullanılabilecek bir kök sertifika kümesi oluşturmak üzere yüklemeye birden çok sunucu ekleyebilirsiniz. Kök sertifika kümesinin parçası olan tüm sunucular, yüklemeye ilk sertifika sunucusunu sağladığınızda tanımlanmış olan yapılandırma veritabanını kullanır.
-   Lisans sunucuları. Lisans sunucusu isteğe bağlıdır ve kök sertifika kümesinin parçası değildir; ancak kök sertifika sunucusunun altında kayıtlıdır. Lisans sunucusu, sertifika ve diğer hizmetler için (hesap sertifikası hizmetleri sağlayamaz) kök sertifika sunucusuna bağlıdır, ancak yayımlama lisansı ve kullanım lisansı sağlamak üzere lisans hizmetlerini çalıştırır. Artıklık ve yük dengelemesi kurmak için, yüklemeye, lisans kümesi oluşturmak üzere birden çok sunucu ekleyebilirsiniz. Lisans kümesinde olan tüm sunucular, bu kümenin ilk sertifika sunucusunu sağladığınızda tanımlanmış olan yapılandırma veritabanını kullanır.
-   Altyapı bileşenlerini çalıştıran sunucular. SQL Server 2000 ve Active Directory gibi bileşenleri de içeren gerekli altyapıyı, dağıtımınızdaki ek sunucular sağlayabilir. Bu bileşenleri nereye kuracağınız ve gereken sunucu sayısı gereksinimlerinize bağlıdır.

Kuruluşunuz için tasarladığınız RMS topolojisi, tüm bu bileşenlerin dağıtımını kapsamalıdır.
