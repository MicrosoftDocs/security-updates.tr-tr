---
TOCTitle: Güvenilen Kullanıcı Etki Alanı Ekleme ve Kaldırma
Title: Güvenilen Kullanıcı Etki Alanı Ekleme ve Kaldırma
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18125157
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747571(v=WS.10)'
---

Güvenilen Kullanıcı Etki Alanı Ekleme ve Kaldırma
=================================================

RMS, varsayılan olarak hak hesabı sertifikaları farklı bir RMS yüklemesi tarafından verilen kullanıcı isteklerini yerine getirmez. Ancak, kullanıcı etki alanlarını RMS'nin bu tür istekleri işlemesine olanak sağlayan güvenilen kullanıcı etki alanları listesine ekleyebilirsiniz.

Güvenilen her etki alanı için belirli kullanıcıları ve kullanıcı gruplarını da ekleyip çıkarabilirsiniz. Ek olarak, güvenilen bir kullanıcı etki alanını kaldırabilirsiniz, ancak güvenilen kullanıcı etki alanlarından bu Active Directory ormanına ait kök sertifika kümesini kaldıramazsınız. Kök sertifika sunucusu dahil, bir dağıtımdaki her RMS sunucusu kendi ormanındaki kök sertifika kümesine güvenir.

Güvenilen kullanıcı etki alanlarını aşağıdaki şekilde yönetebilirsiniz:

-   Genel olarak dış kullanıcıları desteklemek için, Microsoft® .NET Passport hizmetini güvenilen etki alanları listesine ekleyebilirsiniz. Bu, kuruluşunuzdaki RMS sunucusunun Microsoft .NET Passport hizmeti tarafından verilen hak hesabı sertifikasını içeren lisans isteklerini işlemesine olanak sağlar.
-   Başka bir kuruluşun RMS yüklemesindeki dış kullanıcılara güvenmek için, kuruluşu, güvenilen kullanıcı etki alanları listesine ekleyebilirsiniz. Bu, bir RMS sunucusunun farklı bir kuruluştaki bir RMS sunucusu tarafından verilen bir hak hesabı sertifikasını içeren bir lisans isteğini işlemesini sağlar.
-   Aynı şekilde, kuruluşunuzda bulunan ancak farklı bir Active Directory ormanında yer alan kullanıcıların lisans isteklerini yerine getirmek için bu ormandaki RMS yüklemesini güvenilen kullanıcı etki alanları listesine ekleyebilirsiniz. Bu, güncel ormanda bulunan bir RMS sunucusunun farklı bir ormandaki bir RMS sunucusu tarafından verilen bir hak hesabı sertifikasını içeren bir lisans isteğini işlemesini sağlar.
-   Her güvenilen kullanıcı etki alanı için, güvenilen e-posta etki alanlarını belirtebilirsiniz. Güvenilen Passport alt etki alanları için, güvenilir olmayan e-posta kullanıcılarını veya etki alanlarını belirtebilirsiniz.

Güvenilen kullanıcı etki alanları listesine RMS yüklemesi eklemek için eklemek istediğiniz RMS yüklemesinin sunucu lisans sertifikasını almanız gerekir. Yöneticinin ilk önce güvenilecek sunucudan veya kümeden sunucu lisans sertifikasını vermesi ve sertifika dosyasını size göndermesi gerekir. Ardından, dosya konumunu belirterek dosyayı alabilirsiniz. Dosyayı kaydetmek için oturum açan kullanıcının paylaşılan klasöründe izinlere sahip olması gerekir. Güvenilen bir kullanıcı etki alanı kurduğunuzda özel anahtar bilgileri aktarılmaz.

Güvenilen kullanıcı etki alanlarının nasıl oluşturulacağı hakkında adım adım yönergeler için bu konuda daha sonra yer alan "[Güvenilen Kullanıcı Etki Alanı Eklemek için](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93)" bölümüne bakın.
