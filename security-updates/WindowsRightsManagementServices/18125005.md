---
TOCTitle: Dış RMS Kullanıcıları için Planlama
Title: Dış RMS Kullanıcıları için Planlama
ms:assetid: '107e1338-4dcf-4ed5-a49d-e875cc883db1'
ms:contentKeyID: 18125005
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720190(v=WS.10)'
---

Dış RMS Kullanıcıları için Planlama
===================================

Bu bölümde, kuruluşunuzun ve dış kullanıcıların RMS korumalı içeriği Internet üzerinden paylaşmasına olanak vermek için uygulayabileceğiniz topolojiler açıklanmaktadır.

Aşağıdaki seçeneklerden birini kullanarak RMS kümelerini iç ve dış kullanım için dağıtabilirsiniz:

-   Internet üzerinden erişilebilecek bir URL için kök sertifika kümesi URL'si ayarlayın. Bu URL'nin intranet'te aynı kümedeki RMS sunucularına çözümlendiğinden emin olun. Bunu yaptığınızda, son kullanıcı bilgisayarlarının lisans almak için kullandığı yayımlama lisans URL'si hem intranet'te hem de Internet'te çalışır.
-   Özellikle Internet yayımcılığı için ayrı bir RMS kümesi kurun. Internet'ten lisans alınması gereken tüm içerik bu kümede yayımlanmalıdır. İçeriğin hem içeriden hem de dışarıdan kullanılması gerekiyorsa, her iki konumda da yayımlanmalıdır. Ayrıca, kullanıcılar Internet sunucusu ile iletişim kurabilmelidir.

Dış Kullanıcılara İzin Verme
----------------------------

Dış kullanıcılar için iç hesaplar oluşturur ve kullanıcıların sanal özel ağ (VPN) üzerinden şirket ağınıza erişmesine izin verirseniz, bu kullanıcıları RMS yüklemenize ekleyebilirsiniz. Hesabın, dış posta kutusunu gösteren bir iç posta kutusu veya e-posta adresi olabilir.

İç posta kutusu kullanıyorsanız, iç yazarların, RMS korumalı içerik yayımladıklarında bu iç posta kutusuyla ilişkilendirilen e-posta adresini (dış kullanıcının kuruluşunuzun dışında sahip olduğu e-posta adreslerini değil) belirtmeleri gerekir. Dış posta kutusu kullanıyorsanız, iç yazarlar, RMS korumalı içerik yayımladıklarında hesabın dış e-posta adresini belirtmeye özen göstermelidir.

Dış kullanıcıların ağ üzerinden erişimini desteklerken ağ güvenliği de sağlamak için, ortak hesapları için ayrı bir Active Directory ormanı oluşturabilirsiniz. Bu topolojiyle, RMS sisteminin Internet'e açılan bölümü için ayrı bir kök sertifika kümesi oluşturabilirsiniz. Bu, dış kullanıcıların, RMS korumalı içeriğe ilk eriştiklerinde, bu Internet'e açılan kök sertifika kümesinden RMS makine sertifikalarını ve hak hesabı sertifikalarını almalarını sağlar.

Dış kullanıcılar için ortak hesapları içeren ayrı bir orman uygulamaya karar verirseniz, bu ormana RMS yüklenmelidir. Daha sonra, iki RMS sunucusu arasında güven oluşturmak için RMS'nin güvenilen yayımlama etki alanı özelliğini kullanabilirsiniz. Ayrıca, dış DNS kayıtlarının, dış ortaklar için oluşturulan ormandaki RMS yüklemesine ilişkin dış küme URL'sini tanımlamasını sağlamanız da gerekir. Bu güven ilişkisini oluşturmak, dış RMS sunucusunun iç RMS sistemi tarafından yayınlanan tüm içerik için kullanım lisansı vermesine (ve bunun tersine) olanak sağlar.

Dış ormanda RMS sunucusu kurmak yerine, gelen trafiği filtrelemek için ISA sunucusu gibi bir sunucu kullanabilir ve proxy RMS lisans isteklerini iç RMS sunucusuna çevirebilirsiniz.

Dış Sertifikalar Kullanma
-------------------------

Internet'e açılan lisans sunucusu olarak ayrı bir RMS sunucusu kurar, içeriği bu lisans sunucusundan yayımlar ve sonra bu sunucuda güven ilişkileri belirlerseniz, dış kullanıcıların RMS korumalı içeriğe erişmesine izin verebilirsiniz.

RMS dağıtımının Internet'e açılan bölümü, Internet kullanımına ayrılmış ayrı bir lisans sunucusudur. Bu, iç lisans yüklemesi ile aynı kümenin parçasıdır ve iç lisans yüklemesi ile aynı veritabanını ve aynı URL'yi kullanır; gelen Internet trafiğini kabul edebilen tek sunucudur.

Dış kullanıcılar bu RMS lisans sunucusundan kullanım lisansı istediklerinde, bu lisans sunucusunun güvenmesi gereken başka bir RMS sertifika hizmetinden Hak Hesabı Sertifikası kullanıyor olacaklardır.

#### Passport Tabanlı Hak Hesabı Sertifikalarına Güvenme

Kuruluşunuz, Microsoft .NET Passport kimlik bilgilerine dayanan hak hesabı sertifikalarına güvenmeyi seçebilir. Bu hesap sertifikaları, kullanıcıların, hak hesabı sertifikalarını Internet'te barındırılan Microsoft Sertifika Hizmeti'ni kullanarak doğrudan almalarını gerektirir.

Bu modelde, dış kullanıcılar RMS makine sertifikalarını ve hak hesabı sertifikalarını Microsoft'tan alır. İçerik yayımlandığında, dış kullanıcının Microsoft .NET Passport hesabı, yayımlama lisansında bir alıcı olarak adlandırılmalıdır.

Microsoft® .NET Passport hesabı, kullanıcı Microsoft'tan hak hesabı sertifikasını yüklediğinde kullanılmış olan .NET Passport hesabıyla eşleşmelidir. Yazar, RMS etkin uygulamaya alıcıları eklerken bu hesabı belirtmelidir. Hesaplar eşleşmezse içerik kullanılamaz.

#### Diğer Dış Sertifikalara Güvenme

Dış kullanıcının şirketinin de RMS dağıtımı varsa, bu şirketle bir güven ilişkisi kurmayı seçebilirsiniz. Bunu yapmak için, şirketten, RMS sunucu lisans sertifikasını vermesini ve size göndermesini isteyin. Sonra sertifikayı, Internet'e açılan lisans sunucunuzun RMS yönetim konsolunu kullanarak alabilirsiniz.
