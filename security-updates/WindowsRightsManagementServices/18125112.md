---
TOCTitle: RMS İçerik Anahtarları
Title: RMS İçerik Anahtarları
ms:assetid: '63c814bf-2809-477e-a2db-d90370442075'
ms:contentKeyID: 18125112
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720284(v=WS.10)'
---

RMS İçerik Anahtarları
======================

Yazar RMS korumalı içerik yayımladığında, RMS etkin uygulama simetrik içerik anahtarı oluşturur ve içeriği şifrelemek için bunu kullanır. RMS, içerik anahtarı oluşturmak için Gelişmiş Şifreleme Standardı'nı (AES) kullanır.

İçerik anahtarı yayımlama lisansında bulunur ve lisansı yayımlayan RMS sunucusunun ortak anahtarıyla şifrelenir.

Bu sunucu bir kullanım lisansı isteği aldığında, sunucu özel anahtarıyla içerik anahtarının şifresini çözer ve ardından (isteğin bir parçası olarak aldığı) kullanıcı ortak anahtarıyla içerik anahtarını yeniden şifreler. İçerik anahtarı daha sonra bu kullanım lisansına eklenir.
