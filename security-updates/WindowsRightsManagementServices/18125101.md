---
TOCTitle: 'RMS SSS: İç ve Dış Erişim'
Title: 'RMS SSS: İç ve Dış Erişim'
ms:assetid: '59c2c51f-6c20-450c-a334-0e1486292074'
ms:contentKeyID: 18125101
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747577(v=WS.10)'
---

RMS SSS: İç ve Dış Erişim
=========================

İç ve Dış RMS Erişimi Hakkında SSS
----------------------------------

-   [Güvenlik duvarımın, güvenlik duvarı dışındaki RMS istemcilerinin RMS sunucularına erişmesine olanak vermesi için hangi değişiklikleri yapmam gerekir?](#bkmk_37)
-   [Extranet senaryosu nasıl çalışır?](#bkmk_38)
-   [Kullanıcı telif haklı içerik oluşturur ve bu içeriği RMS yüklemesine erişimi olmayan birine verirse, alıcı içeriği kullanabilir mi?](#bkmk_39)
-   [Müşterilerime Outlook 2003 veya Outlook 2007 kullanarak telif haklı e-posta gönderirsem, postayı okumak için ne yapmaları gerekir?](#bkmk_40)
-   [Kuruluşların kendi RMS sunucuları varsa, telif haklı içerik alışverişini nasıl yapabilirler?](#bkmk_41)
-   [Outlook desteği olmayan dışarıdaki bir kuruluşa RMS ile korunan bir e-posta gönderildiğinde, alıcı, Internet Explorer'da Hak Yönetimi Eklentisi kullanılarak okunan e-postayı yanıtlayabilir mi?](#bkmk_42)

<span id="BKMK_37"></span>
#### Güvenlik duvarımın, güvenlik duvarı dışındaki RMS istemcilerinin RMS sunucularına erişmesine olanak vermesi için hangi değişiklikleri yapmam gerekir?

Güvenlik duvarı, dışarıdaki bilgisayarların HTTP (TCP 80 bağlantı noktası) veya HTTPS (TCP 443 bağlantı noktası) üzerinden RMS sunucusuna Basit Nesne Erişim Protokolü (SOAP) isteği yapmasına olanak vermelidir.

<span id="BKMK_38"></span>
#### Extranet senaryosu nasıl çalışır?

Yayımlama lisansında içeriğe bağlı olan iki URL bulunur. Biri, RMS kümesi sağlandığında ayarlanan intranet URL'sidir. Diğeri ise, RMS yöneticisi tarafından ayarlanabilen extranet URL'sidir. Bu extranet URL'si, istemcinin güvenlik duvarı dışından kullanım lisansı almasını sağlar. Yeni telif haklı içerik oluşturmak için extranet URL kullanılamaz. Bu durumda, RMS istemcisinde kayıt defteri geçersiz kılması gerekir.

<span id="BKMK_39"></span>
#### Kullanıcı telif haklı içerik oluşturur ve bu içeriği RMS yüklemesine erişimi olmayan birine verirse, alıcı içeriği kullanabilir mi?

Korumalı içerik ilk açıldığında kullanıcının RMS yüklemesine bağlantısı yoksa, kullanıcı içeriği kullanamaz.

Office 2003 veya daha ileri sürümü eşitlendiğinde, telif haklı e-postaya ilişkin kullanım lisanslarını otomatik olarak aldığından, e-posta ağ bağlantısı olmadan okunabilir. Ancak, Office 2003 veya daha ileri sürüm e-posta için kullanım lisanslarını otomatik olarak önbelleğe alırken, e-postaya ekli Excel 2007, Excel 2003, Word 2007, Word 2003, PowerPoint 2007 ve PowerPoint 2003 belgelerine, bu belgelerin eklendiği e-posta ile aynı haklar atanır. Bunlar, e-posta karşıdan yüklendiğinde otomatik olarak eşitlenmez ve bilgisayar kullanım lisansı almak için ağa bağlandığında tek tek açılmalıdır.

<span id="BKMK_40"></span>
#### Müşterilerime Outlook 2003 veya Outlook 2007 kullanarak korumalı e-posta gönderirsem, postayı okumak için ne yapmaları gerekir?

Alıcının Outlook 2003, Outlook 2007 veya Hak Yönetimi Eklentisiyle birlikte Internet Explorer kullanıyor olması gerekir. Alıcının kuruluşu, kendi RMS yüklemenizle ile RMS yüklemeleriniz arasında güvenli bir ilişki oluşturduysa, alıcı başka bir eylem yapmadan e-postayı okuyabilir. Güven ilişkisi, RMS sunucu lisans sertifikalarının, ilgili ortak anahtarlarıyla birlikte alınıp verilmesiyle oluşturulur.

Alıcının kuruluşunda RMS altyapısı yoksa veya güven ilişkisi oluşturulmamışsa, müşterinizden bir Windows Live ID oluşturmasını isteyebilir ve müşterinizin Windows Live ID kimlik bilgilerine atanan hakları belirterek alıcıya e-posta gönderebilirsiniz. Bu yöntem, kullanım lisansı almak için Internet'ten erişilebilen Microsoft IRM Hizmeti'ni kullanır. IRM hizmeti, kullanıcıların IRM'yi deneme amaçlı olarak kullanmasını sağlamak için ücretsiz sunulur ve yalnızca RMS'yi sınamaya yöneliktir. Bu hizmeti kullanarak içeriği korumayı seçerseniz, lütfen ileride önceden bilgi verilmeden yürürlükten kaldırılabileceğini göz önünde bulundurun.

<span id="BKMK_41"></span>
#### Kuruluşların kendi RMS sunucuları varsa, telif haklı içerik alışverişini nasıl yapabilirler?

RMS, bir RMS yüklemesi tarafından oluşturulan kullanıcı sertifikalarına diğer yükleme tarafından güvenildiği, güvenilen kullanıcı etki alanları kullanır.

<span id="BKMK_42"></span>
#### Outlook desteği olmayan dışarıdaki bir kuruluşa RMS ile korunan bir e-posta gönderildiğinde, alıcı, Internet Explorer'da Hak Yönetimi Eklentisi kullanılarak okunan e-postayı yanıtlayabilir mi?

E-posta alıcısı telif haklı e-postayı diğer e-postalar gibi yanıtlayabilir, ancak alınan e-postanın özgün gövdesi kendi özgün alıcıları için telif haklı olarak kalır. E-postanın paketlenme şekli, istemci uygulaması tarafından belirlenir. Özgün e-posta, yanıta şifreli ek olarak eklenebilir veya Outlook 2003 veya Outlook 2007'de olduğu gibi tümüyle kaldırılabilir.
