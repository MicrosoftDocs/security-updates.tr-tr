---
TOCTitle: Dizin Hizmetleri Veritabanının Bakımı
Title: Dizin Hizmetleri Veritabanının Bakımı
ms:assetid: '911a62f2-c1d6-4091-99b0-b53211be27a7'
ms:contentKeyID: 18125183
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747680(v=WS.10)'
---

Dizin Hizmetleri Veritabanının Bakımı
=====================================

RMS, veritabanı sunucunuz tarafından barındırılan ve kullanıcılar, tanımlayıcılar (örneğin, e-posta adresleri), güvenlik kimlikleri (SID), grup üyeliği ve diğer tanımlayıcılar hakkındaki bilgileri içeren bir dizin hizmetleri veritabanı içerir. Bu bilgiler, RMS lisans hizmeti tarafından Active Directory genel kataloğuna yapılan LDAP sorgularıyla elde edilir ve sonra kullanıcılar kullanım lisansı istediğinde yanıt süresini hızlandırmak için bu veritabanında yerel olarak önbelleğe alınır.

Bu veritabanında depolanan veriler sık olarak eklenip silindiğinden, veritabanı parçalanmaya yatkındır. Tüm DRMS\_DirectoryServices veritabanı tablolarının dizinlerinde, düzenli olarak (günlük veya haftalık) veritabanı yeniden düzenlemesi gerçekleştirmeniz gerekir. Bu işlem, dizinleri yeniden oluşturduğundan veriler parçalanmaz. Parçalanan veriler, düşük performansa ve yönetimsel bir müdahale olmadan devam etmesine izin verilirse sunucu hatasına bile neden olabilir.

Veritabanı sunucusu olarak SQL Server kullanıyorsanız, veritabanı yeniden düzenlemelerini Bakım Sihirbazı'nı kullanarak veya SQL Server Aracısı'nı kullanarak oluşturduğunuz kendi özel komut dosyanızı çalıştırarak yapabilirsiniz.

Veritabanınızda yeniden dizin oluştururken işlem günlüğünüzün kabul edilemeyecek oranda büyüdüğünü fark ederseniz, yeniden dizin oluşturmadan önce Tam kurtarma modundan Toplu Kayıt moduna geçerek bu büyümeyi an aza indirebilirsiniz.
