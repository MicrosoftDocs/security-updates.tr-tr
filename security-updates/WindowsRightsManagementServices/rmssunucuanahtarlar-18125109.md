---
TOCTitle: RMS Sunucu Anahtarları
Title: RMS Sunucu Anahtarları
ms:assetid: '5f4100a1-9aa5-42af-85c8-4bc691022f06'
ms:contentKeyID: 18125109
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720280(v=WS.10)'
---

RMS Sunucu Anahtarları
======================

RMS sunucusunun 1024 bit RSA anahtarlarından oluşan bir anahtar çifti vardır.

Sunucu ortak anahtarı, yalnızca RMS sunucusunun içerik anahtarını alması ve yayımlama lisansı için kullanım lisansları vermesi amacıyla, yayımlama lisansındaki içerik anahtarını şifrelemek için kullanılır. Sunucu lisans sertifikası sunucu ortak anahtarını içerir.

Sunucu ortak anahtarı, sunucu tarafından verilen tüm sertifika ve lisansların imzalanmasında kullanılır.

Sunucu özel anahtarının korunması
---------------------------------

Varsayılan olarak, sağlama sırasında sunucu özel anahtarı oluşturulur ve şifrelenmiş biçimde RMS veritabanında depolanır. Sağlama sırasında diğer bir seçenek de, daha önceden sunucuya yüklenen şifreleme hizmet sağlayıcısını (CSP) belirtmektir.

CSP'yi iki farklı şekilde kullanabilirsiniz:

-   Sunucunuzla birlikte varsayılan olarak yüklenen yazılım CSP uygulamaları arasından seçim yapabilirsiniz.
    -veya-
-   Sunucuya yüklediğiniz Microsoft ürünü olmayan bir yazılım CSP'si kullanabilirsiniz.

| ![](images/Cc720280.note(WS.10).gif)Not                                                       |
|----------------------------------------------------------------------------------------------------------------------------|
| Donanım güvenlik modülü kullanmak isterseniz, donanım güvenlik modüllerini destekleyen bir CSP'yi seçtiğinizden emin olun. |

Sunucu özel anahtarını CSP kullanarak korumayı seçerseniz, RMS sağlayıcının adını ve yapılandırma veritabanındaki anahtar kapsayıcısının adını depolar.
