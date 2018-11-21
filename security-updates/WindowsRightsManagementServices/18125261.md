---
TOCTitle: RMS için Veritabanı Sunucusu Desteği
Title: RMS için Veritabanı Sunucusu Desteği
ms:assetid: 'c9844783-e6c4-49b4-8e7f-0f0377143b44'
ms:contentKeyID: 18125261
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747664(v=WS.10)'
---

RMS için Veritabanı Sunucusu Desteği
====================================

RMS yapılandırması, günlük ve dizin hizmetleri veritabanlarını çalıştırmak için RMS, SQL Server veya Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A gibi bir veritabanı sunucusu kullanır. MSDE 2000'i yalnızca tek sunuculu dağıtımda kullanabilirsiniz. Yerine çalışma koruması için, bir veritabanı sunucusu kümesi kullanabilirsiniz.

Günlük gereksinimlerini desteklemek için yapılandırma ve günlük veritabanlarını ayrı veritabanı sunucusu örneklerinde çalıştırabilir veya kök sertifika sunucusu veya kümesi ile lisans kümeleri için ayrı bir veritabanı sunucusu örneği veya kümesi dağıtabilirsiniz. Bu seçenekler hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sistemini Dağıtma" konusuna bakın.

Varsayılan olarak, RMS Service grubunun bu veritabanları için saklı yordamlarda Yürütme izinleri vardır. Sağlama sırasında oturum açılırken kullanılan kullanıcı hesabı, bu veritabanları üzerinde Veritabanı Sahibi izinlerine sahiptir.

| ![](/security-updates/images/Cc747664.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft SQL Server Desktop Engine, kuruluş çapındaki veritabanını tam olarak çalıştırmak ve desteklemek için gereken araçları içermediğinden, RMS veritabanlarını desteklemek amacıyla yalnızca sınama ortamlarında kullanılması önerilir. Buna ek olarak, MSDE uzak ağları desteklemediğinden, bunu RMS ile aynı sunucuya yüklemeniz gerekir ve RMS kümesine başka RMS sunucuları yükleyemezsiniz. Microsoft SQL Server Desktop Engine kullanım koşullarında, Microsoft SQL Server Desktop Engine veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınız belirtilir. Bu kısıtlama nedeniyle, RMS yapılandırma veritabanını yedekleyemez ve geri yükleyemez, günlük bilgilerini görüntüleyemez veya yapılandırma veritabanında depolanan verileri doğrudan değiştiremezsiniz. |
