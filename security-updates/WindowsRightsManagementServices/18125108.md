---
TOCTitle: İstemci Kimlik Bilgilerini Doğrulamak için Akıllı Kart Kullanma
Title: İstemci Kimlik Bilgilerini Doğrulamak için Akıllı Kart Kullanma
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18125108
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747579(v=WS.10)'
---

İstemci Kimlik Bilgilerini Doğrulamak için Akıllı Kart Kullanma
===============================================================

Ek güvenlik sağlamak ve kimlik bilgileri üzerine denetime sahip olmak için kuruluşunuzda akıllı kart kullanıyorsanız, şimdi bu akıllı kartları RMS sunucusundan hak hesabı sertifikaları ve kullanım lisanları almak için de kullanabilirsiniz. RMS sunucusunu istemci kimlik bilgileri doğrulaması istemek üzere yapılandırmak için, RMS'yi yapılandırdığınız Web sitesinde Güvenli Yuva Katmanı'nı (SSL) etkinleştirmeniz ve Internet Information Services'da (IIS) kimlik doğrulama yöntemini yapılandırmanız gerekir. Bu görevi yerine getirmek için aşağıdaki adımları izleyebilirsiniz:

1.  **Internet Bilgi Hizmetleri Yöneticisi**'ni açın.
2.  Sunucu öğesini genişletin, Web sitesinin klasörünü sağ tıklatın ve ardından **Özellikler**'i tıklatın.
3.  **Dizin Güvenliği** sekmesini tıklatın ve **Güvenli Bağlantılar** alanındaki **Windows dizin hizmeti eşleştiricisini etkinleştir** onay kutusunu seçin.
4.  Web sitesinin klasörünü genişletin, **\_wmcs** sanal dizinini açın ve kimlik doğrulamasını yapılandırmak istediğiniz (**Lisans** veya **Sertifika**) sanal dizini genişletin.
    -   Bir kullanıcı kullanım lisansı istediği zaman kimlik doğrulaması yapılandırmak isterseniz, license.asmx dosyasını sağ tıklatın ve ardından **Özellikler'**i tıklatın.
    -   Bir kullanıcı kullanım sertifikası istediği zaman kimlik doğrulaması yapılandırmak isterseniz, certification.asmx dosyasını sağ tıklatın ve ardından **Özellikler'**i tıklatın.
5.  **Dosya Güvenliği** sekmesini tıkların ve daha sonra **Güvenli Bağlantılar** alanında **Düzenle**'yi tıklatarak **Güvenli Bağlantılar** iletişim kutusunu açın.
6.  **Güvenli kanal gerektir (SSL)**'i seçin ve aşağıdakilerden birini tıklatın.
    -   Sadece akıllı kart benzeri, istemci tarafında sertifikaları olan istemcilerin hizmete bağlanabilmesini istiyorsanız, **İstemci sertifikaları gerektir**'i tıklatın.
    -   İstemcilerin akıllı kart sertifikası veya kullanıcı adı ve parola seçeneklerinden herhangi birini kullanarak kimlik doğrulama kimlik bilgileri sağlamasını istiyorsanız, **İstemci sertifikalarını kabul et**'i tıklatın.
7.  **İstemci sertifika eşleşmesini etkinleştir**'i seçin ve **Tamam**'ı tıklatın.
8.  Hem sertifika hem de lisans için kullanıcı kimliği doğrulamayı kullanmak istiyorsanız, bu yordamı alternatif sanal dizini ikinci kez seçerek tekrarlayın.

Bu ayarlar yapılandırıldıktan sonra, sunucu tarafından yayımlanan RMS korumalı içeriği açmaya çalışan kullanıcıya, sunucu tarafından hak hesabı sertifikası veya kullanım lisansı verilmeden önce kullanıcıdan kimlik doğrulama kimlik bilgilerini vermesi istenir.
