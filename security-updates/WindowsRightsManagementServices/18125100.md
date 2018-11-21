---
TOCTitle: Yetki Alma İşlemini Anlama
Title: Yetki Alma İşlemini Anlama
ms:assetid: '57bd9949-9433-437b-93ed-ffb2dff9992e'
ms:contentKeyID: 18125100
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720276(v=WS.10)'
---

Yetki Alma İşlemini Anlama
==========================

RMS, Internet Information Services'i (IIS) kullanarak, sunduğu çeşitli hizmetleri kullanıma açar. Örneğin, sertifika hizmeti kullanıcıları ve bilgisayarlarını kaydederken, lisans hizmeti içerik yayımlar ve RMS korumalı bilgilere erişim sağlar. Yetki alma işlemini başlatabilmek için RMS sunucusunda, yetki alma hizmeti olarak adlandırılan ek bir hizmetin etkinleştirilmesi gerekir. Yetki alma hizmeti etkinleştirildiğinde, sunucu tarafından sağlanan diğer tüm hizmetler devre dışı bırakılır.

RMS sunucusu yetki alma işlemi için etkinleştirildikten sonra, uygulamalar yetki alma hizmetinden RMS korumalı içeriğin şifresini kalıcı olarak çözen bir içerik anahtarı edinebilir.

RMS sunucusu yetkisi alınmış modda çalışırken, özgün RMS korumalı içeriğe erişim hakkı olan veya olmayan herhangi bir kullanıcı içerik anahtarı edinebilir ve içeriğe yönelik tüm hakları alabilir.

İçeriğin şifresi çözüldükten sonra, kullanıcının, içeriği RMS koruması olmadan kaydetmesi gerekir. Yetki alma hizmetini kullanabilmek için, kullanıcının RMS altyapısına kaydolmuş olması gerekir. Etkin RMS istemcisi olmayan bir kullanıcı, RMS korumalı içeriğe erişim hakkı kazanmak için yetki alma hizmetini kullanamaz.
