---
TOCTitle: Çevrimdışı Yayımlama
Title: Çevrimdışı Yayımlama
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18125333
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747741(v=WS.10)'
---

Çevrimdışı Yayımlama
====================

Çevrimdışı yayımlama, RMS etkin uygulamanın yayımlama lisansını alma yolu nedeniyle çevrimiçi yayımlamadan farklıdır.

Yazar, içeriği çevrimdışı yayımlamadan önce, kök sertifika sunucusuna ağ erişimine sahipken bir istemci lisans sertifikası almalıdır.

Çevrimdışı yayımlama işlemi aşağıdaki adımları içerir:

1.  Yazar RMS etkin bir uygulama kullanarak belgeyi oluşturur ve sonra içeriğe yönelik hak ve koşulları belirtir.
2.  Yazar dosyayı kaydettiğinde, istemci lisans sertifikası, yerel bilgisayar veya aygıtın dosya için bir yayımlama lisansı vermesini ve imzalamasını sağlar.
    Yayımlama lisansı içerik anahtarının iki kopyasını içerir: Biri, istemci lisans sertifikasının ortak anahtarıyla, diğeri istemci lisans sertifikasını veren sunucunun ortak anahtarıyla şifrelenmiştir. Ayrıca sunucunun URL'sini de içerir. İki ortak anahtar ve URL istemci lisans sertifikasından alınır.
3.  Bilgisayar, yazara RMS korumalı içeriği çevrimdışı kullanma hakkı veren özel bir kullanım lisansı olan sahip lisansını oluşturmak için, istemci lisans sertifikasını kullanır. İstemci lisans sertifikası yayımlama lisansındaki simetrik içerik anahtarının şifresini çözmek için kendi özel anahtarını kullanır ve bunu yeniden şifreleyip sahip lisansına gönderir.
4.  Uygulama dosyayı içerik anahtarıyla şifreler ve yayımlama lisansını dosyaya bağlar. Bu dosyanın şifresini çözmeye yönelik lisansları yalnızca yayımlama lisansını veren RMS sunucusu veya güvenilen yayımlama etki alanının üyesi olan sunucu verebilir.
