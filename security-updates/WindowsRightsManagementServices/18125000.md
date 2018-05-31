---
TOCTitle: RMS Makine Etkinleştirmesi
Title: RMS Makine Etkinleştirmesi
ms:assetid: '09a0d631-9860-477f-9d10-df61b3bfe125'
ms:contentKeyID: 18125000
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720182(v=WS.10)'
---

RMS Makine Etkinleştirmesi
==========================

Makine etkinleştirmesi, istemci bilgisayarda RMS korumalı içerik yayımlamak veya kullanmak için sağlanması gereken bir önkoşuldur. Makine etkinleştirmesi, istemci bilgisayara, benzersiz bir kasa ve eşleşen bir RMS makine sertifikası verme işlemidir. Kasa bilgisayarın özel anahtarını, makine sertifikası ise bilgisayarın ortak anahtarını içerir. Kasa, bilgisayarın özel anahtarını içerdiğinden, şifreleme ve şifre çözme işlemlerine yönelik temel güvenlik sorumlusudur. Bilgisayarın her kullanıcısının, makine etkinleştirme işlemi tarafından oluşturulan benzersiz bir makine sertifikası olacaktır.

Service Pack 1'e yönelik RMS istemcisiyle kullanılan makine etkinleştirme işlemi, sürüm 1'deki makine etkinleştirme işleminden önemli ölçüde farklıdır. Service Pack 1'e yönelik RMS istemcisi "kendini etkinleştirir". RMS istemcisi oturum açan bir kullanıcı tarafından yüklendiğinde veya oturum açan kullanıcı RMS özelliğini ilk kez kullandığında, istemci, Windows'ta bulunan şifreleme API'sini kullanarak çeşitli anahtar kümeleri oluşturan etkinleştirme işlemini başlatır. Bu anahtarlar, kullanıcıyı, bilgisayarı ve RMS istemcisini RMS güven hiyerarşisinde birbirine bağlayan bir makine sertifikası oluşturan bir dizi şifreleme gerçekleştirmek için kullanılır.
