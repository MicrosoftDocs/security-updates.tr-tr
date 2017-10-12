---
TOCTitle: Günlük Veritabanının Bakımı
Title: Günlük Veritabanının Bakımı
ms:assetid: 'de55058b-0d1a-4997-8a45-e14678ddd13f'
ms:contentKeyID: 18125293
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747691(v=WS.10)'
---

Günlük Veritabanının Bakımı
===========================

Günlük girişleri, kullanıcı kaydettirme ve kullanım lisansı atama gibi çeşitli RMS işlemleri için verilen lisans kopyalarını da içerir. En kötü durum senaryosunda (her günlük girişinin, başarılı bir kullanıcı kaydı veya kullanım lisansı almak için başarılı bir girişim olduğu durum), her günlük girişi günlük veritabanı boyutunu yaklaşık olarak 200 KB artırır.

Örneğin, RMS korumalı bir e-posta iletisinin, 50.000 kullanıcısı olan bir şirkette tüm çalışanlara gönderildiğini ve her çalışanın da bu iletiyi açtığını varsayın. Her çalışan bu e-posta iletisini bir gün içinde açarsa, günlük veritabanı 10 GB büyür. Dinleme hizmeti, gerçek XrML verilerini günlüğe kaydetmeyecek şekilde yapılandırılabilir ve bu da günlüğe kaydedilen bilgi miktarını azaltır.

Günlük veritabanındaki eski bilgileri ikinci bir veritabanında arşivlemek için komut dosyaları oluşturmayı düşünün. Günlük komut dosyası örneklerini, [Microsoft Web sitesinden](http://go.microsoft.com/fwlink/?linkid=26724) (http://go.microsoft.com/fwlink/?LinkId=26724) ücretsiz olarak yüklenebilen RMS Araç Seti'nde bulabilirsiniz.

Günlük Veritabanı Büyümesini Etkileyen Değişkenler
--------------------------------------------------

Günlük veritabanının boyutunu öngörmek ortamınıza bağlıdır. Günlükteki bazı “başlangıç” girişleri öngörülebilir:

-   RMS sunucusu kaydı
-   Kullanıcı kaydı (her kullanıcı tarafından kullanılan her bilgisayara yönelik benzersiz istek)
-   Çevrimdışı yayımlama sertifikaları için otomatik kullanıcı istekleri

Günlük veritabanındaki, korumalı içerik için kullanım lisansı verilmesiyle ilişkili ilk başlangıç girişlerinden sonraki toplu girişler. Bu veritabanının büyümesini etkileyen koşullar vardır:

-   Kullanıcının korumalı içeriğe her erişiminin yeni lisans gerektirmesi. Bu, korumalı belgeler için varsayılan yöntem değil, isteğe bağlı bir ayardır. Bu gereksinimi uygulamayı seçerseniz, veritabanlarınız daha hızlı büyür.
-   Bir kişiye bir günde gönderilen, tahmini korumalı e-posta iletisi sayısı.
-   Bu korumalı e-posta iletilerini okuyacak tahmini benzersiz kullanıcı sayısı.
-   Bir günde bir kişi tarafından oluşturulacak tahmini korumalı Microsoft Office 2003 (Word, PowerPoint ve Excel) belgesi sayısı.
-   Korumalı belgelerin tahmini alıcıları.

Günlük veritabanın başlangıçtaki boyutu, RMS sunucusu sertifika isteğini de içerecek şekilde, yaklaşık olarak 1,7 MB'dir. Her yeni kullanıcı kaydında, yeni kullanıcı, bir hak hesabı sertifikası (RAC) ve istemci lisans sertifikası (CLC) alır. Bu iki eylem günlüğe kaydedilir ve veritabanının boyutunu 0,06 MB artırırlar. Kullanıcının korumalı içerik için her başarılı lisans alışında, veritabanı 0,19 MB büyür.

Bu tahminin nasıl çalıştığını anlamak için, 5.000 kullanıcısı olan bir şirketin genel kullanım için RMS dağıttığını düşünün. Her kullanıcının bir bilgisayarı vardır ve kuruluş iki RMS sunucusu kullanır. Dağıtımdan sonra, her kullanıcı her gün, beş kullanıcıya gönderilen ortalama bir tane RMS korumalı e-posta iletisi oluşturur. Ayrıca her kullanıcı, üç kullanıcı tarafından erişilen bir tane RMS korumalı belge oluşturur. Aşağıdaki tabloda, bu etkinliğin günlük veritabanı boyutunu nasıl artırdığı hesaplanmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Eylem</th>
<th style="border:1px solid black;" >Günlük Büyümesi</th>
<th style="border:1px solid black;" >Toplam Günlük Boyutu</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS sunucusu başarılı bir şekilde sağlanır</td>
<td style="border:1px solid black;">1,7 MB</td>
<td style="border:1px solid black;">1,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">5000 çalışan kaydı (5000*0,06)</td>
<td style="border:1px solid black;">300 MB</td>
<td style="border:1px solid black;">301,7 MB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Erişilen korumalı e-posta iletisi sayısı (25000*0,19)</td>
<td style="border:1px solid black;">4,750 MB</td>
<td style="border:1px solid black;">5.051,7 MB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Erişilen korumalı belge sayısı (15000*0,19)</td>
<td style="border:1px solid black;">2.850 MB</td>
<td style="border:1px solid black;">7.901,7 MB</td>
</tr>
</tbody>
</table>
  
Böylece kayıt işleminden sonra günlük veritabanının statik boyutu yaklaşık 300 MB'dir. Bu örnekteki günlük büyüme 7,6 GB'dir; bu ise varsayılan Message Queuing yüklemesinin 8 GB sınırına yakındır. Günlük veritabanı bir günden daha uzun süre kullanılamadığında, günlük girişleri kaybolmaya başlar.
  
Günlük Veritabanı Boyutunu Denetleme  
------------------------------------
  
Dağıtım planınız günlük veritabanı yönetimi için bir yöntem içermelidir. Aşağıda en çok kullanılan yaklaşımlar belirtilmiştir.
  
-   **Ayıklama ve arşivleme**  
    Bu yöntem, seçilen bilgilerin, günlük girişleri günlükte belli bir süre kaldıktan sonra günlük veritabanından alınarak ikinci bir veritabanında arşivlenmesi için SQL Server komut dosyaları kullanımını içerir. Bu yöntem, veritabanlarındaki ilgisiz bilgileri filtreleyerek, bu bilgilerin boşuna yer kaplamasını da engeller.  
-   **Günlüğe kaydedilen bilgileri sınırlama**  
    Günlük veritabanı üç ana tablodan oluşur. Bunlardan biri, günlük filtresi etkinleştirildiğinde günlüğe kaydedilmesi gereken asıl tablo alanını belirleyen **DRMS\_Log\_Filter** tablosudur.  
    Açık/kapalı tablo girdileri, RMS sunucusundaki Günlük Dinleme Hizmeti tarafından gerçekten günlüğe kaydedilen asıl tablo alanlarını belirtir. Bu alanlardan ikisi (XrML ile ilişkili olarak), her lisans isteği satırının yaklaşık %99'unu kapladıklarından, günlüğe kaydetme işlemini devre dışı bırakmak için önceden 0 değerine ayarlanmışlardır.  
    **DRMS\_Config\_ServerName\_Port** veritabanının altında bulunan **DRMS\_ClusterPolicies** adındaki başka bir tablo, **LoggingFiltering**'in (Günlük Filtresi) **PolicyName** (İlke Adı) öğesini içerir. **LoggingFiltering** varsayılan olarak etkin değildir. **LoggingFiltering** değerini 1 olarak değiştirirseniz ve Günlük Dinleme Hizmeti'ni yeniden başlatırsanız, daha önce verilen örnekteki günlük veritabanı büyümesi 7,6 GB'den yaklaşık 160 MB'ye düşer.  
-   **Günlük veritabanını taşıma**  
    Büyüyen günlük veritabanını yönetmek için bir başka seçenek de, bu veritabanını daha fazla disk alanına sahip bir sunucuya taşımaktır. Günlük veritabanı yapılandırma veritabanından farklı bir veritabanı sunucusunda bulunabilir. Günlük veritabanını farklı bir sunucuya taşımak için aşağıdaki adımları uygulayın:  
    1.  Tüm RMS sunucularındaki günlük dinleme hizmetini durdurun.  
    2.  Veritabanını farklı bir sunucuya kopyalayın (veya yeni bir veritabanı oluşturun).  
    3.  RMS **DRMS\_Config\_ServerName\_Port** veritabanını, **DRMS\_ClusterPolicies** tablosunu seçerek ve **LoggingDatabaseName** (Veritabanı sunucusu adı) ve **LoggingDatabaseServer** (Veritabanı adı) değerlerini değiştirerek düzenleyin.  
    4.  Komut satırından IISRESET.exe dosyasını çalıştırarak IIS'yi başlatın.
