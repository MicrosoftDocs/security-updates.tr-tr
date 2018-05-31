---
TOCTitle: Kullanım Lisansı Alma
Title: Kullanım Lisansı Alma
ms:assetid: '0b6cde34-418a-4dee-9d27-b65b93b535ac'
ms:contentKeyID: 18125001
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720194(v=WS.10)'
---

Kullanım Lisansı Alma
=====================

Bir kullanıcının RMS korumalı içeriği kullanabilmesi için RMS lisans hizmetinden kullanım lisansı alması gerekir. Aşağıdaki şekil kullanım lisansı isteme ve alma işlemini göstermektedir.

![](/security-updates/images/Cc720194.37b8d28c-9749-4e81-bc6a-22692fefb8b6(WS.10).gif)

Kullanım lisansı alma işlemi aşağıdaki adımları içerir:

1.  Kullanıcı normal dağıtım kanalı aracılığıyla korunan bir dosya alır ve sonra RMS etkin bir uygulama kullanarak bu dosyayı açar. Kullanıcının geçerli bilgisayarda veya aygıtta hak hesabı sertifikası yoksa, bir tane alması gerekir.
2.  RMS etkin uygulama, korumalı içerik için yayımlama lisansını veren sunucuya bir kullanım lisansı isteği gönderir. İstekte kullanıcının hak hesabı sertifikası (kullanıcının ortak anahtarını içerir) ve yayımlama lisansı (içeriğin simetrik anahtarını içerir) bulunur.
    Bir istemci lisans sertifikasının verdiği yayımlama lisansı, sertifikayı veren sunucunun URL'sini içerir. Bu örnekte, kullanım lisansı isteği, yayımlama lisansını veren bilgisayara değil, istemci lisans sertifikasını veren sunucuya gönderilir.
3.  Lisans sunucusu kullanıcının yetkili olduğunu doğrular, kullanıcının adının yayımlama lisansında bulunduğunu onaylar ve bir kullanım lisansı oluşturur. Sunucu kullanıcının hesap sertifikasını doğrular ve kullanıcıya, doğrudan veya izin sahibi bir grubun üyesi olarak hangi izinlerin verildiğini belirler.
    Sunucu sunucunun özel anahtarını kullanarak simetrik içerik anahtarının şifresini çözer, alıcının ortak anahtarını kullanarak bunu yeniden şifreler ve kullanım lisansına ekler. Bu adım içerik anahtarının ve korumalı içeriğin şifresinin yalnızca söz konusu kullanıcı tarafından çözülmesini sağlar.
    Sunucu, kullanım lisansına uygulama veya Windows sürümü dışlaması gibi tüm ilgili bilgileri ekler. Bu koşullar, kullanım lisansı RMS korumalı içeriğe bağlı olduğunda istemci tarafından zorlanır.
4.  Doğrulama tamamlanınca, lisans sunucusu kullanıcının istemci bilgisayarına kullanım lisansını döndürür.
