---
TOCTitle: Kullanım Lisansları ve Dış Kullanıcılar
Title: Kullanım Lisansları ve Dış Kullanıcılar
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18124988
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720176(v=WS.10)'
---

Kullanım Lisansları ve Dış Kullanıcılar
=======================================

RMS yazarların korumalı içeriği Internet üzerinden yetkili dış kullanıcılarla paylaşmasına olanak tanır. İçeriğe eklenen hakların bir RMS sunucusu tarafından lisanslanması gerektiğinden, RMS içerik yayımlama için iç ve dış kullanıcılara eşit koruma sunar. Bu, kuruluşların, iş sözleşmeleri gibi gizli belgeleri Internet üzerinden paylaşmalarını ve bu belgeler üzerinde birlikte çalışmalarını sağlar.

Dış kullanıcı RMS'ye genellikle Internet üzerinden erişir. (Dış kullanıcı iç ağa VPN bağlantısı gibi bir yolla doğrudan erişim sağlayabiliyorsa, işlevsel açıdan bir iç kullanıcıyla eşit durumdadır.) Kullanıcı ister yayımlayan kuruluşta olsun isterse bunun dışında olsun, kullanım lisansı alma işlemi bu konuda daha önce "[Kullanım Lisansı Alma](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)" bölümünde açıklandığı gibi, temelde aynıdır. Kullanıcının bir kullanım lisansı istemek için yazarın ağında bulunması veya ağ üzerinde bir kullanıcı hesabına sahip olması gerekmez.

Gerekli tüm öğeler şunlardır:

-   Kullanıcının geçerli bir hak hesabı sertifikası vardır.
-   Kullanıcının yayımlama lisansını veren ve intranet'te veya extranet'te olabilen RMS lisans sunucusuna erişimi vardır.
-   Kullanıcının hesap sertifikasını veren RMS yüklemesi, kullanım lisansını veren RMS yüklemesinin güvenilen kullanıcı etki alanları listesindedir.

Aşağıdaki dış kullanıcı türleri kullanım lisansı edinebilir:

-   Hesapları, RMS yüklemesine sahip farklı bir Active Directory ormanında yer alan kullanıcılar. Diğer ormandaki RMS yüklemesinin, bu yükleme için güvenilen kullanıcı etki alanı olarak tanımlanması gerekir.
-   Bu yüklemenin güvenilen kullanıcı etki alanları listesine eklenen RMS yüklemesini de çalıştıran başka bir kuruluştaki kullanıcılar.
-   Microsoft RMS Sertifika Hizmeti bu yükleme için güvenilen kullanıcı etki alanları listesinde olduğunda, .NET Passport tabanlı hak hesabı sertifikalarına sahip kullanıcılar.

Güvenilen kullanıcı etki alanları listesine ayrı bir kuruluşu veya kuruluşunuzdaki başka bir RMS yüklemesini ekleyebilirsiniz. Etki alanı ekledikten sonra bu etki alanındaki güvenilir e-posta etki alanlarını tanımlayabilir ve bu etki alanındaki güvenlik tanıtıcılara (SID) güvenilip güvenilmeyeceğini seçebilirsiniz.

Başka bir kuruluş veya kuruluşunuzdaki bir RMS yüklemesi, kendi RMS sunucularının kullanıcılarınızdan gelen kullanım lisansı isteklerini işleyebilmesi için RMS yüklemenizi kendi güvenilen kullanıcı etki alanları listelerine ekleyebilir.

FRMS ve diğer kuruluşlar arasında güvenilen kullanıcı etki alanlarının nasıl oluşturulacağı konusunda daha fazla bilgi için, bu bölümde daha sonra yer alan "[Güvenilen Kullanıcı Etki Alanları](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24)" konusuna ve bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Güvenilen Yayımlama Etki Alanları Ekleme ve Kaldırma" konusuna bakın.
