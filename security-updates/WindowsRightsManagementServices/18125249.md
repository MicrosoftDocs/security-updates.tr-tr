---
TOCTitle: Kullanıcı Hesaplarını Silme
Title: Kullanıcı Hesaplarını Silme
ms:assetid: 'bf73b141-d4d1-4807-a773-3aaff58b0db6'
ms:contentKeyID: 18125249
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747653(v=WS.10)'
---

Kullanıcı Hesaplarını Silme
===========================

Active Directory'den bir kullanıcı hesabını sildiğinizde, kök yapılandırma kümesinin yapılandırma veritabanındaki kullanıcı anahtar tablosunda bulunan kullanıcı hak hesabı sertifikası girdisi otomatik olarak silinmez. Bu nedenle, yeni kullanıcılar eklenip eskileri silinmedikçe kullanıcı anahtar tablosu fazlasıyla büyüyebilir.

Yapılandırma veritabanını korumak için, Active Directory'den her kullanıcı hesabı kaldırılışında söz konusu kullanıcının anahtarını kimlik tanımlayıcısına (SID) göre silen bir saklı yordam çalıştırabilirsiniz. Alternatif olarak, Active Directory'de artık SID'si olmayan kullanıcıların anahtarlarını yapılandırma veritabanından silen bir komut dosyasını düzenli aralıklarla çalıştırabilirsiniz. Bunun SQL Server ve Active Directory'ye büyük bir yük getireceğini unutmayın.
