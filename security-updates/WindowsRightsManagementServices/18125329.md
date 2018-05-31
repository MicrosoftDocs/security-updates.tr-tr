---
TOCTitle: Hak İlkesi Şablonları
Title: Hak İlkesi Şablonları
ms:assetid: 'eee931c8-7c98-48e9-9e2c-d0b7bd4f2b96'
ms:contentKeyID: 18125329
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747732(v=WS.10)'
---

Hak İlkesi Şablonları
=====================

Hak ilkesi şablonları RMS korumalı içeriğe uygulanabilen standart bir kullanıcılar, haklar ve koşullar kümesini açıklamaktadır. Kullanıcı bir hak ilkesi şablonunu içeriğin bir bölümüne uyguladığında, şablonun açıkladığı haklar yayımlama lisansının parçası olur.

RMS Yönetimi Web sitesinde, hak ilkesi şablonları oluşturmanın yanı sıra varolan şablonları silebilir veya değiştirebilirsiniz. Hak ilkesi şablonları belirli alıcılar veya Active Directory grupları, içeriğin kullanım lisansının ne kadar süreyle geçerli olacağı, içeriğin yayımlandıktan sonra ne kadar süreyle kullanılabileceği ve hatta belirli bir RMS etkin uygulama için geçerli olan özel değerler gibi çeşitli koşullar içerebilir. Şablon bir iptal listesi gerektirebilir. Şablon liste dosyasının URL'sini ve listenin geçerli olduğu gün sayısını belirtir. Alıcı şablonu temel alan bir kullanım lisansı istediğinde, sistem, kullanıcının RMS korumalı içeriği kullanabilmesi için önce iptal listesini denetler. Daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS İptal İşlemi](https://technet.microsoft.com/72689f90-f3c5-4b61-94ea-d825f3199b3b)" bölümüne bakın.

Hak ilkesi şablonlarında bulunan haklara verilebilecek örnekler aşağıdaki gibidir:

-   İçeriği herkes görebilir, ancak yalnızca yazar değiştirebilir.
-   Kuruluştaki herkes içeriği görebilir, bu durum içeriğin yayımlanmasından sonraki bir ay için geçerlidir.
-   Kuruluştaki herkes içeriği görebilir, ancak dışarıdaki ortaklar veya müşteriler göremez.
-   İçeriği yalnızca belirtilen alıcılar görebilir.
-   İçeriği yalnızca belirli bir alıcı görüntüleyebilir veya değiştirebilir.

Şablonlar aşağıdaki gibi çeşitli koşulları içerebilir:

-   Belirli alıcılar veya içeriğe yönelik haklara sahip Active Directory grupları.
-   Kullanım lisansının içerik için geçerli kalacağı süre.
-   İçeriğin yayımlandıktan sonra kullanılabileceği süre.
-   Kullanım lisansının iptal listesi gerektirip gerektirmediği ve listenin hangi sıklıkta yenilenmesi gerektiği.
-   Belirli bir RMS etkin uygulama için geçerli olan özel değerler.

Hak ilkesi şablonları hem yapılandırma veritabanında hem de paylaşılan bir klasörde depolanır. RMS yöneticisi, yazarların kullanabilmesi için hak ilkesi şablonlarını paylaşılan klasörden istemci bilgisayarlara dağıtmaktan sorumludur. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Hak İlkesi Şablonlarını Dağıtma" konusuna bakın.

RMS etkin bir uygulamada, yazarlar genellikle uygulanacak hak ilkesi şablonunu seçebilir; bu şablonda üyelerinin içeriği kullanabileceği bir grup belirtilir. Alıcı kullanım lisansı istediği zaman, sunucu, veritabanındaki hak ilkesi şablonunu uygular; bu, kullanım lisansı koşullarının her zaman şablonun en güncel sürümünü yansıtmasını sağlar.
