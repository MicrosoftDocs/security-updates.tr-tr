---
TOCTitle: 'RMS''de FIPS Uyumluluğu Sorunları'
Title: 'RMS''de FIPS Uyumluluğu Sorunları'
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18125133
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747551(v=WS.10)'
---

RMS'de FIPS Uyumluluğu Sorunları
================================

Rights Management Services (RMS) 1.0 Service Pack 1 (SP1), FIPS tarafından değerlendirilmiş şifreleme işlevi kullanımı gerektiren kuruluşlarda etkin bir şekilde çalışmak üzere tasarlanmıştır.

Federal Bilgi İşlem Standardı 140-1 (FIPS 140-1) ve bunu izleyen FIPS 140-2, ABD hükümetinin, şifreleme yazılımı uygulamaları için referans oluşturan standartlarıdır. Şifreleme algoritmalarını uygulamaya yönelik en iyi yöntemleri, anahtarın ve veri arabelleklerinin kullanımını ve işletim sistemiyle çalışma şeklini belirtirler.

RMS, gizli verileri korumak amacıyla FIPS uyumlu sistemin bir parçası olarak uygulanabilir.

-   FIPS tarafından değerlendirilmiş şifreleme hizmeti, işlevleri aşağıda belirtildiği biçimde kısıtlar: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. Bu kısıtlama, güvenlik kanalı sağlayıcısını, yalnızca daha güçlü Aktarım Katmanı Güvenliği (TLS) 1.0 protokolü ile anlaşmaya zorlar. Internet Explorer'ın TLS'yi destekleyecek şekilde yapılandırılması gerekebilir, ancak pek çok üçüncü taraf Web sunucusu TLS'yi desteklemez. Bu konuyla ilgili daha fazla bilgi için [Microsoft Web sitesinde](http://go.microsoft.com/fwlink/?linkid=43614) 811834 numaralı Bilgi Bankası makalesine bakın.

Yazılım tabanlı özel anahtar koruması kullanacaksınız, RMS özel anahtarını, Microsoft'un varsayılan iki şifreleme hizmeti sağlayıcısından (CSP) birini kullanarak koruyun. Bu CSP'ler ABD hükümetinin FIPS 140-1 veya FIPS 140-2 (uygun olan) değerlendirme işleminden geçmiştir. Gerekli olmasa da, güvenlik konusunun çok önemli olduğu müşterilere, üst düzey RMS sunucusu özel anahtarlarını korumak için donanım güvenliği modülleri (nCipher veya IBM gibi) kullanmaları önerilir. Donanım güvenliği modülleri (HSM) kullanılırsa, HSM kullanmak üzere uygun CSP'nin seçilmesi gerekir. Bu işlem, sistemin yeniden başlatılmasını gerektirebilir. Bu konuyla ilgili daha fazla bilgi için [Microsoft Web sitesinde](http://go.microsoft.com/fwlink/?linkid=44138) 830690 numaralı Bilgi Bankası makalesine bakın.

RMS sisteminizi uygularken aşağıdaki seçimleri yapmanız gerekir:

-   Windows'ta FIPS uyumlu şifreleme için NSA kurallarını uygulayın.
-   Yerel Güvenlik İlkesi'ni FIPS uyumlu şifreleme kullanacak şekilde etkinleştirin.
-   Yukarıdaki ortamda RMS SP1 istemcileri ve sunucuları dağıtımı yapın.
-   RMS sunucunuzdaki Internet Information Services uygulamasında Aktarım Katmanı Güvenliği (TLS) protokolünü etkinleştirin.
-   İstemcilerinizin Internet Explorer uygulamalarında Aktarım Katmanı Güvenliği (TLS) protokolünü etkinleştirin.
-   SQL istemcileri ve veritabanı sunucusundaki SQL Server arasında Windows TLS/SSL Güvenlik Sağlayıcısı ile kullanılan SQL Düz Veri Akışı (TDS) protokolünü etkinleştirin.
-   SQL'i, TSL/SSL gerektirecek şekilde yapılandırın.
