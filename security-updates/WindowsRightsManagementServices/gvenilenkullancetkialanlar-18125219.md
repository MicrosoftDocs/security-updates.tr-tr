---
TOCTitle: Güvenilen Kullanıcı Etki Alanları
Title: Güvenilen Kullanıcı Etki Alanları
ms:assetid: 'a09b883f-f455-4c46-a4fd-d37b689e1d24'
ms:contentKeyID: 18125219
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747618(v=WS.10)'
---

Güvenilen Kullanıcı Etki Alanları
=================================

RMS, varsayılan olarak hak hesabı sertifikaları farklı bir etki alanı tarafından verilen kullanıcılara kullanım lisansı vermez. Kullanıcı etki alanı bir kök sertifika kümesi, isteğe bağlı lisans sunucuları veya kümeleri ile ilişkili veritabanlarından oluşan bir RMS yüklemesidir.

RMS'yi, başka bir kullanıcı etki alanının sunucu lisans sertifikasını alıp bunu güvenilen kullanıcı etki alanları listesine ekleyerek, bu tür istekleri işleyecek şekilde yapılandırabilirsiniz. Bunu yaptığınız zaman, hesap sertifikaları güvenilen kullanıcı etki alanı tarafından verilmiş olan kullanıcılar, yüklemenize kullanım lisansı istekleri gönderebilir. Bu kullanım lisansları iç kullanıcılardan alınan istekler gibi işlem görür.

| ![](images/Cc747618.note(WS.10).gif)Not                                                                    |
|-----------------------------------------------------------------------------------------------------------------------------------------|
| Kök sertifika kümesi, aynı yüklemedeki tüm RMS sunucularının güvenilen kullanıcı etki alanları listesine otomatik olarak yerleştirilir. |

Farklı kullanıcı etki alanlarındaki kullanıcılara korumalı içeriği paylaşma izni verebilirsiniz. Bu, aşağıdaki örneklerde açıklanmaktadır:

-   Kuruluşunuz paylaşmak ve korumak istediğiniz gizli belgeler üzerinde bir başka kuruluşla birlikte yakın ilişki içinde çalışıyor. Diğer kuruluş da RMS çalıştırıyor. İki kuruluş da diğerinin RMS yüklemesini kendi güvenilen kullanıcı etki alanları listesine ekleyebilir, böylece her iki kuruluştaki kullanıcılar korumalı içerik üzerinde birlikte çalışabilir ve bunları Internet veya extranet üzerinden alıp verebilir.
-   Her bir Active Directory ormanında yalnızca bir RMS yüklemesi olabilir. Kuruluşunuz birden fazla Active Directory ormanı dağıtmıştır ve her biri RMS çalıştırmaktadır. Kullanıcılar korumalı içeriği, hangi ormanda olduğuna bağlı olmadan, diğer kullanıcılarla paylaşmak istiyor. Bunu sağlamak için, her ormandaki güvenilen kullanıcı etki alanları listesine diğer ormanların RMS yüklemesini ekleyebilirsiniz.
-   Kuruluşunuzdaki kullanıcılar, korumak istediğiniz gizli belgeler üzerinde diğer kuruluştaki kullanıcılarla birlikte çalışıyor. Diğer kuruluş RMS çalıştırmıyor. Diğer kuruluştaki kullanıcılar .NET Passport hesapları oluşturabilir ve siz de RMS yüklemenizin güvenilen kullanıcı etki alanları listesine .NET Passport'u ekleyebilirsiniz. Her iki şirketteki kullanıcılar korumalı içerik üzerinde çalışabilir ve Internet üzerinden bu içeriğin alıp gönderebilir.

Güvenilen kullanıcı etki alanları ve adım adım yönergeler hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Güvenilen Kullanıcı Etki Alanları Ekleme ve Kaldırma" ve "Güven İlkeleri Oluşturma" konularına bakın.
