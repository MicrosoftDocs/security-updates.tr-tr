---
TOCTitle: Alt Kayıt Hizmetini Bulma
Title: Alt Kayıt Hizmetini Bulma
ms:assetid: 'b159953a-af38-4a9e-8c87-1aff5fb4e366'
ms:contentKeyID: 18125241
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747641(v=WS.10)'
---

Alt Kayıt Hizmetini Bulma
=========================

Tek başına olan bir lisans sunucusunun veya bir kümedeki ilk lisans sunucusunun, RMS kök sertifika sunucusuna alt kayıt isteği göndermesi ve sunucu lisans sertifikası alması gerekir. Bunu yapmak için, lisans sunucusu kök sertifika alt kayıt hizmetinin URL'sini aşağıdaki şekilde edinir.

Lisans sunucusunun sağlanması sırasında RMS Kurulumu Active Directory'yi sorgular ve sonra kök sertifika kümesinin hizmet bağlantı noktasını algılar. RMS, kök sertifika kümesini bulmak için bu hizmet bağlantı noktasında depolanan URL'yi kullanır ve sonra kök sertifika sunucusunun alt kayıt hizmetinden sunucu lisans sertifikası isteğinde bulunur.

Alt kayıt hizmet isteğinde bulunmak için lisans sunucusu ilk olarak Active Directory'den alt kayıt hizmetinin bulunduğu kök sertifika sunucusunun Certification sanal dizinine ait URL'yi alır. Daha sonra, bu yolu alt kayıt hizmetine ekler.

Örneğin, kök sertifika sunucusu üzerindeki Certification sanal dizinine ait URL, Active Directory'de aşağıdaki biçimde depolanır:

http://*sunucu\_adı*/\_wmcs/Certification

Lisans sunucusu alt kayıt hizmet isteğinde bulunduğunda, hizmet dosyası adını aşağıdaki şekilde URL'nin sonuna ekler:

http://sunucu\_adı/\_wmcs/Certification/SubEnrollService.asmx

| ![](/security-updates/images/Cc747641.note(WS.10).gif)Not                           |
|------------------------------------------------------------------------------------------------|
| RMS sunucunuzda SSL'yi etkinleştirdiyseniz, bu URL'ler https:// bağlantı protokolünü kullanır. |
