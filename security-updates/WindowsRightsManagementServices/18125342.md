---
TOCTitle: Hak İlkesi Şablonlarıyla Çalışma
Title: Hak İlkesi Şablonlarıyla Çalışma
ms:assetid: 'ff4f1143-f6b9-4dd8-aa4c-c2cbbf6fdf06'
ms:contentKeyID: 18125342
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747804(v=WS.10)'
---

Hak İlkesi Şablonlarıyla Çalışma
================================

Hak ilkesi şablonunu oluşturduktan sonra, yazarlara dağıtımını denetleyerek kuruluşta uygulanmasını yönetebilirsiniz.

RMS, hak ilkesi şablonlarını yapılandırma veritabanında depolar. Ayrıca, bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarının Konumunu Belirtmek için](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)" bölümünde açıklandığı gibi, tüm hak ilkesi şablonlarının bir kopyasını, belirttiğiniz paylaşılan klasörde saklar. Şablonlarınızın, kuruluşun güvenlik kurallarına uygun bir ağdan erişilebilir konumunda depolandığından emin olun. RMS'nin kullandığı Program Files veya IISRoot klasörleri gibi ana klasörlerde şablonlar için paylaşılan klasörler oluşturmamalısınız.

Korumalı içerik yayımlarken, yazar yerel bilgisayarda bulunan şablonların arasından uygulanacak hak ilkesi şablonunu seçer. Hak ilkesi şablonlarını kullanılır hale getirmek için, yöneticinin bu şablonları bir paylaşılan klasörden kullanıcı bilgisayarlarına dağıtması gerekir.

Kullanıcı, korumalı içeriği kullanmaya çalıştığı zaman, RMS etkin uygulama içeriği yayımlamak için kullanılan hak ilkesi şablonunun en son sürümünü yapılandırma veritabanından alır. Bunun ardından, RMS etkinleştirilmiş uygulama, ayarlarını içeriğe uygular. RMS sunucusunda bir hak ilkesi şablonunu değiştirdiğinizde, RMS hem yapılandırma veritabanındaki hem de paylaşılan klasördeki şablonu günceller (RMS sunucu hak ilkesi şablonlarını depolamak için bir dosya konumu belirtecek şekilde yapılandırılmadıysa). Kullanıcıların bilgisayarlarında en son sürüme sahip olmaları için, değiştirildikten sonra hak ilkesi şablonunu istemci sistemlere yeniden dağıtın.

Bir hak ilkesi şablonunu silerseniz, şablon, yapılandırma veritabanından ve şablonların kopyalarının depolanacağı yer olarak belirtilen paylaşılan klasör konumundan da silinir. Bununla birlikte, kullanıcı bilgisayarlarından kaldırılmaz. Şablonu bu konumdan kendiniz kaldırmalısınız. Silinen hak ilkesi şablonlarını tüm kullanıcı bilgisayarlarından kaldırmanız gerekir. Kaldırmazsanız ve silinen hak ilkesi şablonu içerik yayımında kullanılırsa, RMS, yapılandırma veritabanında belirtilen şablonu bulamayacağından içerik için kullanım lisansı veremez.

Hak ilkesi şablonlarıyla çalışırken şu görevleri yerine getirin:

-   **Bir paylaşılan klasör belirtin**. İlk hak ilkesi şablonunuzu oluşturmadan önce, tüm hak ilkesi şablonlarının depolanacağı paylaşılan klasörü belirtmeniz gerekir. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarının Konumunu Belirtmek için](https://technet.microsoft.com/e1bee46d-33db-424f-ba45-1dcedcb883ab)" bölümüne bakın.
-   **Hak ilkesi şablonlarını oluşturun ve düzenleyin**. Kuruluşunuzda hakları yönetmek için gerektiği kadar hak ilkesi şablonu oluşturabilirsiniz. Hak ilkesi şablonu oluştururken kullanıcıları ve uygulanacak hakları tanımlarsınız. Ayrıca içeriğe uygulanacak hak ilkesi şablonunu da tanımlarsınız. Hak ilkesi şablonlarını güncelleştirmeniz gerektiği zaman daha sonra düzenleyebilirsiniz. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.
-   **Hak ilkesi şablonlarını dağıtma**. Yazarın içeriğe belirli bir hak ilkesi şablonunu uygulayabilmesi için, yazarın bilgisayarında hak ilkesi şablonunun bir kopyasının bulunması gerekir. Şablon dağıtımını yöneterek, hangi yazarların hangi hak ilkesi şablonlarını uygulayacağını denetleyebilirsiniz. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Dağıtma](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)" bölümüne bakın.
-   **Hak ilkesi şablonlarının hizmetten çekilmesi**. Bir hak ilkesi şablonunu, gerek kalmadığı zaman silebilirsiniz. Bunu yaparken, kullanıcıların hizmetten çekilen şablon kullanılarak yayımlanan içeriği kullanmaya çalıştıkları zaman sorun yaşamamaları için kullanıcı bilgisayarlarından da kaldırmanız gerekir. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Hizmetten Çekme](https://technet.microsoft.com/32bf98c7-edda-4507-a4b8-4c11bddd6e60)" bölümüne bakın.
