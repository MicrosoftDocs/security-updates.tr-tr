---
TOCTitle: Veritabanı Büyümesini Tahmin Etme
Title: Veritabanı Büyümesini Tahmin Etme
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18125164
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747585(v=WS.10)'
---

Veritabanı Büyümesini Tahmin Etme
=================================

RMS veritabanlarınız için gereken depolama alanı miktarını hesaplarken, RMS yapılandırma veritabanı için en az 10 megabayt (MB) kapasite planlayın ve sonra her 500 sunucu için 1 MB ekleyin. Günlük veritabanı yapılandırma veritabanından farklı bir veritabanı sunucusunda bulunabilir.

RMS günlük kaydı özelliğini kullanıyorsanız, günlük veritabanının, büyük miktarda günlüğe kayıt işleminin oluştuğu kullanıcı sertifikası başlangıç aşamasında her kullanıcı için yaklaşık olarak 1 MB büyümeyi desteklemesi gerekir. Örneğin, dağıtımınız 1.000 kullanıcıyı destekleyecekse, günlük veritabanı, bu kullanıcılar etkinleştirildiğinde ve RMS sertifika sunucusu tarafından lisanslandığında 1 gigabayta (GB) kadar büyüyecektir. Normal işlemlerde, günlük veritabanı her kullanıcı için günde 200 kilobayt (KB) miktarında büyüyebilir (aşamalı dağıtım yapıyorsanız, sisteme eklenen her yeni kullanıcı için ek olarak 1 MB hesaplayın.)
