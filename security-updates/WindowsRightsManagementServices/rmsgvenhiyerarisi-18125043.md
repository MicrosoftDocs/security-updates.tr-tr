---
TOCTitle: RMS Güven Hiyerarşisi
Title: RMS Güven Hiyerarşisi
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18125043
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720232(v=WS.10)'
---

RMS Güven Hiyerarşisi
=====================

RMS sistemindeki bileşenler Microsoft Kayıt Hizmeti, kuruluş RMS sunucuları, istemci bilgisayarları ve sistem kullanıcılarını içerir. Her bileşene, bileşenin sistemdeki kimliğini oluşturan bir sertifika verilir. Bir güven hiyerarşisi bu sertifikalar ve dolayısıyla bunları elinde bulunduran varlıklar arasındaki güven ilişkisini tanımlar. Güven hiyerarşisi, güvenilen varlıklar ve bu varlıkların diğer güvenilen varlıklara verdikleri lisanslar arasındaki güven ilişkisini de tanımlar.

Güven hiyerarşisi sertifikaları ve lisansları, RMS'nin belirli bir sertifikadan veya lisanstan güvenilen anahtar çiftine kadar uzanan yolu her zaman izleyebileceği bir zincir halinde bağlar. Güven zinciri geçerli sertifika, bunu veren varlığın sertifikası, bu varlığın sertifikasını veren varlığın sertifikası şeklinde güven köküne kadar giden zinciri içerir.

RMS için güven kökü veya "güven çapası" bir Microsoft anahtar çiftidir. Bu genel güven kökü, bir kuruluşun içindeki ve dışındaki, kullanıcılar ve ortaklar gibi güvenilen varlıkları kapsayan bir güven ekosistemi oluşturmasına olanak sağlar.

Aşağıdaki diyagramda bir kuruluştaki güven hiyerarşisi gösterilmektedir. Güven zinciri ana sertifikaları veren Microsoft hizmetlerine kadar gider.

![](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif)
1.  Her istemci bilgisayara Microsoft kök ortak anahtarını içeren benzersiz bir kasa verilir.
2.  RMS bir lisans isteği aldığında, güven hiyerarşisindeki yolu güvenin köküne kadar izleyerek sorumluları doğrular.
3.  RMS lisansta adı geçen güvenilen varlığın kimliğini doğrular.
4.  RMS güvenilen varlığın sertifikasının güven hiyerarşisindeki bir sunucu tarafından verildiğini doğrular.

Sertifika zincirinin her düzeyinde, RMS sertifikayı veya lisansı doğrular ve sonra güven zinciri üzerinden bilinen güven köküne bağlandığını doğrular. Zincirdeki her lisans veya sertifika RMS tarafından aşağıdaki koşulları doğrulamak için denetlenir:

-   XrML'si geçerlidir.
-   Sertifikayı verenin imzası geçerlidir.
-   Lisansın semantiği hedeflenen kullanım için uygundur.
-   Koşullar (geçerlilik tarihleri gibi) karşılanmıştır.
-   Lisans iptal edilmemiştir.
-   Lisans imza anahtarı ve onaylı, sertifikayı veren anahtarı eşleşmelidir.
