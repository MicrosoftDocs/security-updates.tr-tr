---
TOCTitle: Sanal Dizin İzinlerini Ayarlama
Title: Sanal Dizin İzinlerini Ayarlama
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18125075
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747549(v=WS.10)'
---

Sanal Dizin İzinlerini Ayarlama
===============================

Yetki alma özelliği etkinleştirildikten sonra hizmet olarak kullanılabilir. Ancak, yetki alma hizmeti, ilişkilendirilen erişim izinleri olan bir IIS sanal dizinidir. Hizmeti kullanacak olan kullanıcılar için, izinleri sanal dizinde ve decommission.asmx adındaki gerçek dosyada ayarlamanız gerekir.

Sanal dizin için Tümleşik Windows Kimlik Doğrulaması varsayılan olarak etkinleştirilmiştir, ancak gerçek dosyaya yalnızca sistem ve yönetici hesapları erişebilir. Decommission.asmx dosyası için DACL izinlerini belirlerken, gerçek RMS korumasını kaldırmak için yalnızca belirli bir kullanıcı grubuna erişim yetkisi verebilir veya hizmete herkesin erişmesini sağlayabilirsiniz.

Kullanıcıların yetki alma hizmetini kullanmaya başlayabilmesi için, kullanıcı uygulamasının, kullanım lisansı isteklerini bu yeni yetki alma ardışık düzenine gönderebilecek şekilde değiştirilmesi gerekir. Microsoft Office System 2003'te bu işlem, kullanıcının bilgisayarına bir kayıt defteri girdisi eklenerek yapılır. Office 2003 kullanıyorsanız, bu adımı gerçekleştirmek için aşağıdaki yordamı kullanabilirsiniz:

1.  Kayıt Defteri Düzenleyicisi'ni açın.
2.  `HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM`'ye gidin ve `Decommissioning` adında yeni bir anahtar ekleyin.
3.  Decommissioning anahtarı altına, aşağıdaki yeni **Dize Değeri** girdisini, *lisans-sunucunuz* yerine RMS sunucunuzun adını yazarak ekleyin:
    `http://`*lisans-sunucunuz*`/_wmcs/licensing`
4.  Sonra girdiyi sağ tıklatın ve yetki alma hizmetini gösteren değer verisini belirtmek için **Değiştir**'i seçin:
    `http://`*lisans-sunucunuz*`/_wmcs/decommission`

| ![](images/Cc747549.note(WS.10).gif)Not                                   |
|--------------------------------------------------------------------------------------------------------|
| Kuruluşta yetki alma modunda birden çok RMS sunucusu varsa, bu anahtar için birden çok girdi olabilir. |
