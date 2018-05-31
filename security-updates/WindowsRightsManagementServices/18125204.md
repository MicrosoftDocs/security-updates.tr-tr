---
TOCTitle: Message Queuing Hizmetini İzleme
Title: Message Queuing Hizmetini İzleme
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18125204
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747716(v=WS.10)'
---

Message Queuing Hizmetini İzleme
================================

RMS günlüğü, olayları günlük veritabanına göndermek için Message Queuing'i (MSMQ olarak da bilinir) kullanır. Her RMS ön uç sunucusu, iletileri Message Queuing hizmetine gönderir ve her ön uç sunucusunda bulunan günlük dinleyici hizmeti, günlük iletilerini Message Queuing sırasından alarak bunları günlük veritabanına yazar. Günlük veritabanı veya veritabanı sunucunuz kullanılamaz hale gelirse veya günlük dinleyici hizmeti durdurulursa, Message Queuing iletileri sırada depolar. Günlük veritabanını veya veritabanı sunucusunu kapatmayı planlıyorsanız, ilk önce her ön uç sunucusunda günlük dinleyici hizmetini kapatmanız ve daha sonra veritabanını veya veritabanı sunucusunu yeniden başlattıktan sonra her ön uç sunucusunda günlük dinleyici hizmetini yeniden başlatmanız önerilir.

Veritabanının hata vermesine rağmen günlük dinleyici hizmeti çalışmaya devam ederse, günlük dinleyici hizmeti günlük iletilerini veritabanına yazamaz. Günlük dinleyicisi hizmeti, iletileri veritabanı kullanılabilir duruma gelinceye kadar (yeni günlük iletileri bu noktada veritabanına yazılır) "teslim edilemeyen" Message Queuing sırasına taşır. Teslim edilemeyen sırasındaki iletiler otomatik olarak günlük veritabanına yazılmaz. Teslim edilemeyen sırasındaki iletileri görüntülemek veya silmek için aşağıdaki adımları izleyin:

1.  Microsoft Yönetim Konsolu (MMC) Bilgisayar Yönetimi ek bileşenini açın. Bunu yapmak için **Başlat**'ı tıklatın, **Tüm Programlar**'ın ardından **Yönetimsel Araçlar**'ın üzerine gelin ve **Bilgisayar Yönetimi**'ni tıklatın.
2.  Konsol ağacındaki Hizmetler ve Uygulamalar'ın altında, Message Queuing'i ve ardından Özel Sıralar'ı tıklatın.
3.  İki sıra görüntülenir. Her ikisinin de "**drms\_logging**" ile başlayan ve kümenin adıyla devam eden birer adı vardır. Sıralardan birini adı "**drms\_logging\_***\_&lt;kümenizin adı&gt;*\_**deadletter**" şeklindedir. Bu, teslim edilemeyen sırasıdır. Sıranın adını ve ardından Sıra iletileri sırasını tıklatın.
4.  Özelliklerini görüntülemek için iletileri çift tıklatın.
5.  Sırayı silmek için **Sıra iletileri** sırasını sağ tıklatın, **Tüm Görevler**'i seçin ve ardından **Temizle**'yi tıklatın.

Varsayılan yapılandırmada, Message Queuing sıraya sokulmuş tüm iletileri sunucudaki boş depolama alanı sınırına kadar depolar. Message Queuing kullanılabilir sabit disk alanının tümünü kullanırsa, RMS sunucusu istemci isteklerini yerine getiremez. Bunu önlemek için Message Queuing sıralamada kullanabileceği disk alanı miktarını sınırlandırmak üzere aşağıdaki adımları izleyin:

1.  Microsoft Yönetim Konsolu (MMC) Bilgisayar Yönetimi ek bileşenini açın. Bunu yapmak için Başlat'ı tıklatın, Tüm Programlar'ın, ardından Yönetimsel Araçlar'ın üzerine gelin ve Bilgisayar Yönetimi'ni tıklatın.
2.  Konsol ağacındaki Hizmetler ve Uygulamalar'ın altında, Message Queuing'i ve ardından Özel Sıralar'ı tıklatın.
3.  İki sıra görüntülenir. Her ikisinin adı da "drms\_logging" ile başlar. Her bir sırada aşağıdaki adımları izleyin:
    -   Özellikler'i tıklatın.
    -   İleti depolama sınırı (KB) onay kutusunu seçin ve ardından sırada saklanabilecek tüm sıra iletilerinin kilobayt cinsinden toplam boyutunu yazın.

Sıra dolarsa, RMS'den gelen iletiler ulaştıkları anda atılır ve Olay Kimliği 48 ile ilişkili aşağıdaki olay iletisi Sistem Olay günlüğüne gönderilir.

"Özellik Kümesi Message Queuing'e gönderilemedi."

Bu, günlük veritabanındaki bir soruna işaret ettiği için sistem izleme araçlarını bu olay gerçekleştiğinde sizi uyaracak şekilde yapılandırmanız önerilir.
