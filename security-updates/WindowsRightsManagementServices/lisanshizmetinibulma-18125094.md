---
TOCTitle: Lisans Hizmetini Bulma
Title: Lisans Hizmetini Bulma
ms:assetid: '4eabbb76-b359-443a-b737-098c5659e9c6'
ms:contentKeyID: 18125094
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720269(v=WS.10)'
---

Lisans Hizmetini Bulma
======================

RMS lisans hizmeti, kimliği doğrulanan kullanıcıların korumalı içeriği kullanmasına olanak tanıyan kullanım lisansları verir.

Bu hizmet kök sertifika ve lisans sunucuları veya kümeleri üzerinde çalışır. Kullanım lisansı isteğinde bulunmak için istemci ilk önce URL'yi Active Directory'den lisans hizmetinin bulunduğu kök sertifika kümesinin Licensing sanal dizinine alır. Ardından yolu lisans hizmetinin sonuna ekler.

Örneğin, kök sertifika kümesinin Licensing sanal dizininin URL'si aşağıdaki biçimde Active Directory'de depolanır:

http://*sunucu\_adı*/\_wmcs/Licensing

Sunucu kullanım lisansı istediğinde, lisans hizmeti dosya adını aşağıdaki şekilde URL'nin sonuna ekler:

http://*sunucu\_adı*/\_wmcs/Licensing/License.asmx

Hizmet konumu yayımlama lisansını veren RMS sunucusu veya .NET Passport hesabıdır; URL, yayımlama lisansında bulunur.

| ![](images/Cc720269.note(WS.10).gif)Not                           |
|------------------------------------------------------------------------------------------------|
| RMS sunucunuzda SSL'yi etkinleştirdiyseniz, bu URL'ler https:// bağlantı protokolünü kullanır. |
