---
TOCTitle: Yayımlama Hizmetini Bulma
Title: Yayımlama Hizmetini Bulma
ms:assetid: '5d500841-a202-4865-b5d2-d0775d4e1bbc'
ms:contentKeyID: 18125104
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747580(v=WS.10)'
---

Yayımlama Hizmetini Bulma
=========================

RMS yayımlama hizmeti, içeriği korumak için kullanılan yayımlama lisanslarını verir. Bu hizmet, şirket ağına bağlı olmadıklarında kullanıcıların içerik yayımlamasına olanak sağlayan istemci lisans sertifikalarını da verir.

Yayımlama hizmeti, kök sertifika kümesi veya lisans sunucularından kullanılabilir. Yazar RMS korumalı içerik yayımladığında RMS etkin uygulama bu hizmetten istekte bulunur. Yayımlama hizmeti isteğinde bulunmak için, uygulama ilk olarak Active Directory'den sunucunun, yayımlama hizmetinin bulunduğu Licensing sanal dizininin URL'sini alır. Ardından yolu yayımlama hizmetinin sonuna ekler.

Örneğin, bir sunucunun Licensing sanal dizininin URL'si Active Directory'de aşağıdaki biçimde depolanır:

http://*sunucu\_adı*/\_wmcs/Licensing

Sunucu yayımlama lisansı isteğinde bulunduğunda, yayımlama hizmeti dosya adını aşağıdaki şekilde URL'nin sonuna ekler:

http://*sunucu\_adı*/\_wmcs/Licensing/Publish.asmx

RMS, hak hesabı sertifikasının Windows kullanıcı kimlik doğrulamasını temel aldığını algılarsa, yayımlama hizmetinin konumu Active Directory ormanı tarafından belirlenir. Bu, hem iç kullanıcılar hem de sanal özel ağ (VPN) ile kuruluş ağına bağlanan dış kullanıcılar için geçerlidir.

RMS, hak hesabı sertifikasının Microsoft® .NET Passport'u temel aldığını algılarsa, yayımlama hizmetinin konumu RMS korumalı içerikte belirtilen .NET Passport hesabıdır.

| ![](/security-updates/images/Cc747580.note(WS.10).gif)Not                           |
|------------------------------------------------------------------------------------------------|
| RMS sunucunuzda SSL'yi etkinleştirdiyseniz, bu URL'ler https:// bağlantı protokolünü kullanır. |
