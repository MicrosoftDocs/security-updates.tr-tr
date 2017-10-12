---
TOCTitle: RMS Sunucularının Yetkisini Alma
Title: RMS Sunucularının Yetkisini Alma
ms:assetid: '11badb02-62c1-455c-96b7-935bbcb496bc'
ms:contentKeyID: 18125011
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720200(v=WS.10)'
---

RMS Sunucularının Yetkisini Alma
================================

RMS'nin yetkisi aldığınızda, önceden yayımladığı RMS korumalı içeriğin şifresini çözen bir anahtar sağlayabilmesi için RMS sunucusunun davranışı değiştirilir. Bu anahtar, içeriğin RMS koruması olmadan kaydedilebilmesini sağlar. Bu, kuruluşunuzda RMS koruması kullanımına son vermeye karar verdiyseniz faydalı olabilir.

Kullanıcıların, içeriklerini RMS koruması olmadan kaydedebilme fırsatı bulması ve ağ ve sistem yöneticilerinizin tüm RMS etkinleştirilmiş istemcilerin hizmeti kullanmalarını engellemesine yetecek kadar uzun süre sunucuyu yetkisi alınmış halde çalıştırmanız gerekir.

Yetki alma özelliğini yönetim Web sitesinin **Güvenlik ayarları** Web sayfasından etkinleştirebilirsiniz. Yetki alma özelliğini etkinleştirdikten sonra, sunucuyu standart bir RMS sunucu yapılandırmasına geri yükleyemezsiniz. Yükleme herhangi bir güvenilen yayımlama etki alanını içerdiyse, bu etki alanlarının da yetkisi alınır.

Yetki alma özelliği etkinleştirildikten sonra, yönetim Web sitesi yalnızca **Yetkisi alınan sunucu bilgileri** sayfasını içerir; başka bir yönetim işlemi desteklenmez. Sunucunuzun yetkisini alma işlemini tamamlamak için aşağıdaki adımları gerçekleştirmeniz gerekir:

1.  Yetki alma sanal kök dizinine **RMS Service Group** Okuma ve Yürütme izinlerini verin.
2.  Decommissioning.asmx dosyasının DACL'sine **Everyone** grubunu ve Okuma izinlerini ekleyin.
3.  Kullanıcılarınıza RMS yüklemesinin yetkisini aldığınızı bildirin ve içeriklerini RMS korumasız olarak kaydetmek üzere sunucuya bağlanmalarını önerin.
4.  Kuruluşunuzdaki tüm RMS etkinleştirilmiş uygulamaları decommissioning.asmx sayfasına bağlanacak biçimde yapılandırın. Bu, RMS etkin uygulamaya bağlı olarak kayıt defteri anahtarı veya Grup İlkesi ayarıyla denetlenebilir.
5.  Kuruluşunuz otomatik olarak yayımlamaya yönelik yüklemeden yararlanan RMS etkin uygulamalar kullanıyorsa, bu uygulamaların yetki alma hizmetini kullanmasını sağlamak amacıyla bu bilgisayarlarda bir kayıt defteri girdisi ayarlamak için Grup İlkesi'ni kullanmanız gerekir.
6.  İçeriğin tümünün korunmasız hale getirildiğinden emin olduktan sonra, sunucu özel anahtarını yedeklemeniz ve ardından RMS'yi sunucudan kaldırmanız gerekir.
