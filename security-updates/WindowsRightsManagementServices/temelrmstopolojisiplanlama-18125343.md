---
TOCTitle: Temel RMS Topolojisi Planlama
Title: Temel RMS Topolojisi Planlama
ms:assetid: 'fec3201e-201f-4faf-910e-fa44132af83d'
ms:contentKeyID: 18125343
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747755(v=WS.10)'
---

Temel RMS Topolojisi Planlama
=============================

Temel RMS topolojisi, kök sertifika kümesi olarak hizmet veren bir veya daha çok fiziksel sunucudan oluşur. Bu küme kuruluşta sertifika, lisans ve yayımlama için kullanılır. Dağıtım çok küçük bir dağıtım değilse, normal olarak tek bir URL arkasında birden çok fiziksel sunucu yapılandırılır. Bu küme, kök sertifika sunucusunu oluşturmak üzere ilk sunucu sağlanıp sonra da tahmin ettiğiniz etkinliği desteklemek için gereken kök sertifika sunucusu sayısına erişinceye kadar kümeye sunucu ekleyerek oluşturulur. Aşağıdaki şekilde bu topoloji gösterilmektedir.

![](images/Cc747755.a3332719-4d25-4694-a89a-7c31fd97ca3b(WS.10).gif)

Bir kümeye sunucu eklediğinizde aynı yapılandırma ve günlük veritabanlarını paylaşırlar (bunlar SQL Server veritabanlarıdır). SQL Server kök sertifika sunucusunda veya ayrı bir sunucuda bulunabilir.

Yük dengeleme, kök sertifika kümesindeki tüm sunucularda ayarlanır. Sertifika ve lisanslara yönelik tüm istekler, kümedeki ilk sunucuyu yapılandırırken belirttiğiniz ortak URL üzerinden kök sertifika kümesine aktarılır.

Az sayıda istemciyi destekleyecekseniz, RMS'yi yerel veritabanıyla tek bir sunucuda kurabilirsiniz. Sunucu kuruluştaki tüm sertifika ve lisans işlerinden sorumludur. Bu yapılandırma tek bir hata noktası oluşturduğundan, yapılandırmanızın yedeklerini düzenli olarak almanız önerilir.
