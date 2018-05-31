---
TOCTitle: RMS Önkoşulları ve Denetim Listeleri
Title: RMS Önkoşulları ve Denetim Listeleri
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18125175
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747582(v=WS.10)'
---

RMS Önkoşulları ve Denetim Listeleri
====================================

RMS'yi yüklemeye başlamadan önce RMS'yi kullanmaya yönelik teknoloji önkoşullarını gözden geçirin; listelenen teknolojilerin her biri RMS ile tümleşiktir ve RMS'yi başarıyla dağıtmak için bunlar hakkında temel bilgi sahibi olunması önemlidir. RMS'yi dağıtmak ve yönetmek için görev listelerini ve planları oluşturmanıza yardımcı olması amacıyla aşağıdaki denetim listelerini kullanın:

-   [Teknoloji Önkoşulları](#bkmk_9)
-   [RMS Dağıtımı Denetim Listeleri](#bkmk_10)
-   [RMS Yönetimi Denetim Listeleri](#bkmk_14)

<span id="BKMK_9"></span>
Teknoloji Önkoşulları
---------------------

Bu belge grubu Windows RMS'nin nasıl çalıştığını, kuruluşunuz için dağıtımı nasıl planlayıp gerçekleştireceğinizi ve sistemin günlük yönetimini nasıl yapacağınızı anlamanıza yardımcı olan bilgiler sağlar. Aşağıdaki alanlarda bilginiz olduğunu kabul edilir:

-   Windows Server 2003 dağıtımı ve yönetimi
-   Active Directory dağıtımı ve yönetimi
-   Microsoft® Internet Information Services 6.0 (IIS) dağıtımı ve yönetimi
-   Microsoft® SQL Server™ 2000 yönetimi
-   Temel ortak anahtar altyapısı (PKI) kavramları
-   Sunucu ağ bağlantısı ve güvenliği

Bu konular hakkında daha fazla bilgi için, bu belge grubundaki [RMS Sunucusunu Çalıştırma](http://go.microsoft.com/fwlink/?linkid=42495) bölümünde bulunan “Ek Kaynaklar” konusuna bakın.

<span id="BKMK_10"></span>
RMS Dağıtımı Denetim Listeleri
------------------------------

Bu bölümde aşağıdaki dağıtım görevleri için denetim listeleri sağlanmaktadır:

-   [Tek Sunucu Yüklemesini Dağıtma](#bkmk_11)
-   [Kök Sertifikası ve Lisans Kümelerini Dağıtma](#bkmk_12)
-   [RMS'yi Ormanlarda Dağıtma](#bkmk_13)

RMS'yi dağıtma konusunda daha fazla bilgi için, bu belge grubundaki [RMS sistemi dağıtma](http://go.microsoft.com/fwlink/?linkid=42494) konusuna bakın.

<span id="BKMK_11"></span>
Tek Sunucu Yüklemesini Dağıtma
------------------------------

Tek bir RMS sunucusunu dağıtmak için aşağıdaki denetim listesini kullanın.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kavramları ve planlama bilgilerini gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS sistemi dağıtma</a> bölümünde &quot;RMS Dağıtımına Hazırlanma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sistem gereksinimlerini gözden geçirin ve gerekli tüm donanımın ve yazılımın bulunduğunu doğrulayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS Dağıtımını Planlama</a> bölümünde &quot;RMS için Altyapı Gereksinimleri&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS Dağıtımını Planlama</a> bölümünde &quot;Veritabanı Sunucusu Altyapısını Planlama&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Donanım ve yazılım önkoşulları, yönetim hesapları ve SMS veya Grup İlkesi desteği dahil olmak üzere altyapıyı uygun bir şekilde kurun.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Dağıtımına Hazırlanma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS'yi sunucuya yükleyin ve yapılandırın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Dağıtımı sınayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;Sınama Ortamını Kurma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Üretim ortamında RMS'yi uygulayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Uygulamasının Kapsamını Tanımlama&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Kök Sertifikası ve Lisans Kümelerini Dağıtma  
--------------------------------------------
  
Kök sertifikası ve lisans kümelerini dağıtmak için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kavramları ve planlama bilgilerini gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Dağıtımına Hazırlanma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sistem gereksinimlerini gözden geçirin ve gerekli tüm donanımın ve yazılımın bulunduğunu doğrulayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS Dağıtımını Planlama</a> bölümünde &quot;RMS için Altyapı Gereksinimleri&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS Dağıtımını Planlama</a> bölümünde &quot;Veritabanı Sunucusu Altyapısını Planlama&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Yüklenecek topolojiyi ve bileşenleri anlamak için dağıtım planınızı gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=37537">RMS Dağıtımını Planlama</a> bölümünde &quot;RMS Topolojinizi Belirleme&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Donanım ve yazılım önkoşulları, yönetim hesapları ve SMS veya Grup İlkesi desteği dahil olmak üzere altyapıyı uygun bir şekilde kurun.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Dağıtımına Hazırlanma&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Kök sertifika kümesindeki sunuculara RMS'yi yükleyin ve yapılandırın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;Sertifika ve Lisans Desteği için Sunucu Ekleme&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lisans kümelerindeki sunuculara RMS'yi yükleyin ve yapılandırın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;Sertifika ve Lisans Desteği için Sunucu Ekleme&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Yük dengelemeyi ayarlayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;Kümeleri Desteklemek için Temel Altyapıyı Genişletme&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dağıtımı sınayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;Sınama Ortamını Kurma&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim ortamında RMS'yi uygulayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Uygulamasının Kapsamını Tanımlama&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
RMS'yi Ormanlarda Dağıtma  
-------------------------
  
Kök RMS'yi ormanlar arasında dağıtmak için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kavramları ve planlama bilgilerini gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS Dağıtımına Hazırlanma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Güven modelinize bağlı olarak gereken izinleri yapılandırın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS'yi Ormanlarda Dağıtma&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ormanlarınız için uygun Active Directory özniteliklerini ayarlayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> bölümünde &quot;RMS'yi Ormanlarda Dağıtma&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
RMS Yönetimi Denetim Listeleri  
------------------------------
  
Bu bölümde aşağıdaki yönetim görevleri için denetim listeleri sağlanmaktadır:
  
-   [Hak İlkesi Şablonu Uygulama](#bkmk_15)  
-   [Yeni RMS İstemcisi Dağıtma](#bkmk_16)  
-   [Güvenilen Kullanıcı Etki Alanı Ekleme](#bkmk_17)  
-   [Güvenilen Yayımlama Etki Alanı Ekleme](#bkmk_18)
  
RMS'yi yönetme konusunda daha fazla bilgi için, bu belge grubundaki [RMS Sunucusunu Çalıştırma](http://go.microsoft.com/fwlink/?linkid=42495) bölümüne bakın.
  
<span id="BKMK_15"></span>
Hak İlkesi Şablonu Uygulama  
---------------------------
  
Hak ilkesi şablonu uygulamak için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Belirsiz kavramları gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS Teknik Başvuru Kılavuzu</a> içinde &quot;Hak İlkesi Şablonları&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hak ilkesi şablonunun konumunu belirtin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Hak İlkesi Şablonlarının Konumunu Belirtmek İçin&quot;.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Hak ilkesi şablonunu oluşturun.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Hak İlkesi Şablonları Oluşturma ve Değiştirme&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Hak İlkesi Şablonu Eklemek İçin&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hak ilkesi şablonunu dağıtın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Hak İlkesi Şablonlarını Dağıtma&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Yeni RMS İstemcisi Dağıtma  
--------------------------
  
RMS istemcisinin yeni sürümünü dağıtmak için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Belirsiz kavramları gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42494">RMS Sistemini Dağıtma</a> içindeki &quot;İstemci Dağıtımı Planlaması&quot;
<a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Kasa Sürümlerini Dışlama&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Tüm istemcileri en yeni istemci sürümüne yükseltmeye zorlamak için, eski kasa sürümünü dışlayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Kasa Sürümlerini Dışlamak İçin&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Güvenilen Kullanıcı Etki Alanı Ekleme  
-------------------------------------
  
Güvenilen kullanıcı etki alanı eklemek için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Belirsiz kavramları gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS Teknik Başvuru Kılavuzu</a> içindeki &quot;Güvenilen Kullanıcı Etki Alanları&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Güvenilen Kullanıcı Etki Alanları Ekleme ve Kaldırma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Eklemek istediğiniz kullanıcı etki alanının sunucu lisans sertifikasını alın. (Bunu güvenilecek yüklemenin yöneticisi sağlamalıdır.) Sonra kullanıcı etki alanını yüklemenize ekleyin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Güvenilen Kullanıcı Etki Alanı Eklemek için&quot;.</td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Güvenilen Yayımlama Etki Alanı Ekleme  
-------------------------------------
  
Güvenilen yayımlama etki alanı eklemek için aşağıdaki denetim listesini kullanın.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Başvuru</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Belirsiz kavramları gözden geçirin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42496">RMS Teknik Başvuru Kılavuzu</a> içindeki &quot;Güvenilen Yayımlama Etki Alanları&quot;.
<a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Güvenilen Yayımlama Etki Alanları Ekleme ve Kaldırma&quot;.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Eklemek istediğiniz şifreli sunucu lisans sertifikasını ve yayımlama etki alanının özel anahtarını alın ve sonra yayımlama etki alanını yüklemenize ekleyin.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=42495">RMS Sunucusunu Çalıştırma</a> içindeki &quot;Güvenilen Yayımlama Etki Alanı Eklemek için&quot;.</td>
</tr>
</tbody>
</table>
