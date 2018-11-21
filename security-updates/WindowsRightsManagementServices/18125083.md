---
TOCTitle: RMS Etkin Uygulamalar
Title: RMS Etkin Uygulamalar
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18125083
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720231(v=WS.10)'
---

RMS Etkin Uygulamalar
=====================

RMS etkin içerik oluşturmak veya bunu kullanmak için, bu konuda açıklandığı gibi, kullanıcıların bir RMS etkin uygulamaya sahip olması gerekir. Ayrıca, RMS istemcisinin de yüklü olması ve bunların kullandıkları bilgisayarların etkinleştirilmiş olması gerekir. Daha fazla bilgi için, bu konunun daha sonraki bölümlerinde yer alan "[RMS İstemcisi](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2)" ve "[RMS Makine Etkinleştirmesi](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125)" konularına bakın.

RMS etkin uygulamalar içerik yazarlarının, içeriğin kullanım biçimini denetlemek amacıyla, oluşturdukları dosyalara kullanım haklarını yayımlama lisansları biçiminde eklemesine olanak tanır. Ayrıca, RMS etkin uygulamalar şifrelenmiş dosya bilgilerini işler ve kullanıcıların yayımlama lisansında tanımlanan izinlere göre içeriği kullanmasına olanak tanır.

Geliştiriciler Rights Management Services Client SDK'yı kullanarak RMS korumalı içerik lisanslayan, yayımlayan ve kullanan RMS etkin uygulamalar oluşturabilir. RMS etkin uygulamalar, Microsoft® Windows® 98 İkinci Sürüm veya daha yenisini çalıştıran bilgisayarlar için geliştirilebilir.

Geliştiriciler Rights Management Services Client SDK'yı kullanarak RMS etkin sunucu uygulamaları da geliştirebilir. Bu uygulamalar içeriği yayımlayabilir, ancak kullanamaz.

E-posta ve Web sayfalarındaki RMS korumalı içeriği kullanmak için başka bir RMS etkin uygulaması olmayan kullanıcılar, Microsoft® Internet Explorer için Hak Yönetimi Eklentisi'ni edinip kulanabilirler. Örneğin, Outlook Web Access (OWA) müşterileri RMS korumalı e-posta iletilerini kullanmak için Internet Explorer için Hak Yönetimi Eklentisi'ni kullanabilir.

Internet Explorer için Hak Yönetimi Eklentisi'ni [Microsoft Web sitesiden](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450) yükleyebilirsiniz.

| ![](/security-updates/images/Cc720231.note(WS.10).gif)Not                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Internet Explorer için Hak Yönetimi Eklentisi'ni Windows XP Service Pack 2 ile kullanıyorsanız, geliştirilmiş güvenlik yapılandırması bazı uygulama uyumluluk sorunlarına neden olabilir. |

Kuruluşunuzdaki her bir etki alanının extranet bağlantı URL'si Internet Explorer'daki Yerel Intranet sitelerine eklenmediyse, Internet Explorer için Hak Yönetimi Eklentisi'ni kullanan kullanıcılar sürekli olarak sitelere bağlanmak isteyip istemediklerini soran bir iletiyle karşılaşır. Bu iletilere verilen hatalı bir yanıt RMS istemcisinin kullanıcı hesabı için yeni bir hak hesabı sertifikası almasına neden olabilir.

Bu siteleri kuruluş genelinde doğru şekilde ayarlamak için, gerekli URL'leri kayıt defterine Yerel Intranet bölgesinin bir parçası olarak yazmak için bir komut dosyası kullanın. Yerel Intranet bölgesi varsayılan olarak iletileri ortadan kaldırmayı sağlayan yüksek bir güvenlik düzeyi sağlar.
