---
TOCTitle: İçerikten RMS Korumasını Kaldırma
Title: İçerikten RMS Korumasını Kaldırma
ms:assetid: 'c30361e3-50d2-4474-a87d-d38de502cf9e'
ms:contentKeyID: 18125254
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747658(v=WS.10)'
---

İçerikten RMS Korumasını Kaldırma
=================================

Yetki alma işlemi tamamlandığında önemli bilgilerin korunabilmesi için hangi dosyaların kimin tarafından ve ne zaman kurtarılması gerektiğine önceden karar verin. Gerekli tüm RMS korumalı dosyalardan RMS koruması kaldırıldığında, sunucu altyapıdan kaldırılabilir.

İçerikten RMS korumasını kaldırma işlemi aşağıdaki gibidir:

1.  Kullanıcı varolan tüm kullanım lisanslarını bilgisayardan kaldırmalıdır. Böylece RMS istemcisi içeriği açmak için lisans almak amacıyla sunucuya gider. Kullanım lisansları istemci bilgisayarda %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM klasöründe depolanır ve dosya adlarında EUL öneki bulunur.
2.  Yetki alma sunucusuna erişimi olan kullanıcı, RMS korumalı bir dosyayı açmaya çalışır.
3.  Uygulama yetki alma sunucusuna bağlanır ve içerik anahtarını alır.
4.  İçeriğin şifresi çözülür ve içerik düzenlenebilir, kaydedilebilir, iletilebilir veya yazdırılabilir.
5.  Kullanıcı içeriği RMS koruması olmadan kaydeder. Artık RMS sunucusuna bağlanmak gerekmeden tüm kullanıcılar içeriği açabilir.
