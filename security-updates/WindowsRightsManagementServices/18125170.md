---
TOCTitle: Ölçeklendirme Gereksinimlerini Değerlendirme
Title: Ölçeklendirme Gereksinimlerini Değerlendirme
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18125170
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747663(v=WS.10)'
---

Ölçeklendirme Gereksinimlerini Değerlendirme
============================================

Tek veya birden çok sunucu dağıtma kararını vermek için, RMS dağıtımını kullanacak kullanıcı sayısını ve bunların koruyacağı dosya sayısını belirleyin.

Bu, ortalama kullanım gereksinimini verir. Ortalama gereksinimin yaklaşık üç katı olan en yüksek kullanım gereksinimi için planlama yapın.

Ayrıca şirketinizin hataya dayanıklılık ve hizmet sunma standartlarını da dikkate alın.

RMS, referans oluşturan ölçümler sağlamak için, çift işlemcisi olan 2,4 GHz Pentium 4 sunucu ve 1 GB RAM kullanılarak sınandı. Bu yapılandırmada, RMS sunucusu yaklaşık olarak saniyede 50 lisans teslim etti.

Bir RMS sisteminin kullanım gereksinimlerini hesaplamak için kapasite planlaması sırasında aşağıdaki rakamları kullanabilirsiniz:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >İşlem</th>
<th style="border:1px solid black;" >Oluşum</th>
<th style="border:1px solid black;" >İstemciden sunucuya bant genişliği kullanımı (KB)</th>
<th style="border:1px solid black;" >Sunucudan istemciye bant genişliği kullanımı (KB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lisans isteği</td>
<td style="border:1px solid black;">Her kullanıcı ve her içerik parçası için yinelenir</td>
<td style="border:1px solid black;">64</td>
<td style="border:1px solid black;">18</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hak hesabı sertifikası</td>
<td style="border:1px solid black;">Yalnızca RMS başlatma trafiği</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">16</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">İstemci kaydı</td>
<td style="border:1px solid black;">Yalnızca RMS başlatma trafiği</td>
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">16</td>
</tr>
</tbody>
</table>
  
Ek olarak, Active Directory sorgu trafiği ağ verimini etkileyebilir. Ancak, RMS sunucularını genel katalog sunucularına çok yakın bir şekilde dağıtıyorsanız, genellikle bu bir etken olmaz. Bunun istisnası, bir sitedeki tüm genel katalog sunucularındaki hata nedeniyle, aynı kapasiteyi desteklemeyen bir bağlantı üzerinden başka bir sitenin bu sitenin yerine çalışmasıdır.
  
Aşağıdaki tabloda, Active Directory sorgu trafiğinin kuruluşunuzun ağına etkisini değerlendirmek için kullanabileceğiniz RMS işlemlerinin bant genişliği kullanımına yönelik temel veriler sağlanır.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >İşlem</th>
<th style="border:1px solid black;" >RMS'den genel kataloğa bant genişliği kullanımı (KB)</th>
<th style="border:1px solid black;" >Genel katalogdan RMS'ye bant genişliği kullanımı (KB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RMS bağlantı kurulumu (ldap_bind)</td>
<td style="border:1px solid black;">1600</td>
<td style="border:1px solid black;">200</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS grup üyeliği değerlendirmesi (ldap_search)</td>
<td style="border:1px solid black;">200</td>
<td style="border:1px solid black;">100</td>
</tr>
</tbody>
</table>
  
Bu başvuru tablolarını kullanırken, sayıları dağıtımınızın içeriğine göre uyguladığınızdan emin olun. Örneğin, kullanıcı 15 grubun üyesiyse, RMS arama isteği için 200 bayt ve genel katalogdan gelen yanıt için 1500 bayt (100 bayt x 15) gerekecektir.
  
İçerik lisansı istek yoğunluğu, RMS'nin gerçekleştirdiği işlemlerin büyük çoğunluğunu gösterdiğinden, kapasite planlama, beklenen içerik lisansı istek yoğunluklarına dayanarak planlanmalıdır. Lisans istekleri veri yoğun işlemler olmadığından ve tümüyle önbelleğe alınan bilgilere dayandığından, disk sürücüsünün giriş/çıkış hızı ve performansı RMS için çok önemli etkenler değildir.
  
Sunucu performansı belirlenirken dikkat edilecek en önemli değişken CPU kullanımıdır, bu yüzden uygun işlemcilerin seçilmesi önemlidir. Sunucunun yükü arttıkça RMS sunucularının bellek gereksinimi de artar ve sunucunun en yüksek performans düzeyini aşar. Bu durumda, Internet Information Services (IIS) gelen istekleri sunucu işleyinceye kadar bellekte sıraya alır. IIS'de yapılandırdığınız sıra sınırlamasına bağlı olarak, sıra belirlenen en yüksek uzunluğa ulaştığında, gelen isteklerin sıraya alınması durdurulur ve istekler reddedilir.
  
Yük modeline ilişkin RMS bellek gereksinimleri (çalışma kümesi), fiziksel bellek boyutu sınırlarına tümüyle uymalıdır. Toplam bellek boyutunu belirleyen en önemli etken grup genişletme önbelleğe alma gereksinimleridir. RMS çalıştıran her sunucuda en az 1 GB RAM olması önerilir.
  
Her RMS sunucusu, belirli bir sürede belirli sayıda istemci isteğini işleyebilir (yaklaşık olarak saniyede 30 ile 50 lisans). Bu yüzden, sunucu ekleme bir kümenin lisans verme kapasitesini doğru orantılı olarak artırır ve ayrıca daha yüksek güvenilirlik sağlar. Sonuç olarak, ölçeklendirme hem tek tek sunuculara, hem de dağıttığınız sunucu sayısına uygun olmalıdır. Aşağıdaki yapılandırma örnekleri, bu tahminleri, RMS dağıtımınıza yönelik ölçeklendirme gereksinimlerini hesaplamak için nasıl kullanabileceğinizi gösterir.
  
-   Düşük Yoğunlukta Kullanım Yapılandırması  
    RMS'nin destekleyeceği kullanım gereksinimleri bazı kuruluşlarda oldukça düşük düzeydedir. Örneğin, yaklaşık 5.000 kullanıcısı olan ve bu kullanıcıların yüzde 10'unun e-posta içeriğini korumak için düzenli olarak RMS kullandığı bir kuruluşta, ortalama bir kullanıcının saatte 3 e-posta iletisi koruması beklenebilir. Bu gereksinimlere dayanarak, RMS sunucularının saatte 1.500 lisans teslim etmesi gerekir; bu da saniyede 0,42 lisans demektir. Bu ortalama kullanım gereksinimini verir; bu rakam 3 ile çarpıldığında ise en yüksek kullanım olarak saniyede 1,25 lisans elde edilir.  
    Bu hesaplama esas alındığında, kullanım oldukça düşüktür. Bu nedenle, tek bir RMS sunucusu bu kuruluş için yeterli olacaktır.  
-   Ortalama Yoğunlukta Kullanım Yapılandırması  
    Birçok kuruluş, gereksinimleri ortalama olan çok sayıda kullanıcı grubuna sahiptir. Örneğin, yaklaşık 40.000 kullanıcısı olan ve bu kullanıcıların yüzde 50'sinin e-posta içeriğini korumak için düzenli olarak RMS kullandığı bir kuruluşta, ortalama bir kullanıcının saatte 7 e-posta iletisi ve saatte 1 belge veya başka bir dosya koruması beklenebilir. Bu gereksinimlere dayanarak, RMS sunucularının saatte 160.000 lisans teslim etmesi gerekir; bu da saniyede 44,4 lisans demektir. Bu ortalama kullanım gereksinimini verir; bu rakam 3 ile çarpıldığında ise en yüksek kullanım olarak saniyede 133,3 lisans elde edilir.  
    Bu hesaplama esas alındığında, kullanım biraz daha yüksek olacaktır ve 3 RMS sunucusu geçerli kullanıcı gereksinimlerini karşılamaya yeterliyken, 6 RMS sunucusu geçerli kullanıcı gereksinimlerini karşılayacağı gibi büyümeye de açık olmayı sağlayacaktır.  
-   Yüksek Yoğunlukta Kullanım Yapılandırması  
    Daha büyük kuruluşların genellikle, yoğun kullanım gereksinimleri olan oldukça fazla kullanıcı grubu vardır. Örneğin, yaklaşık 150.000 kullanıcısı olan ve bu kullanıcıların yüzde 70'inin e-posta içeriğini korumak için düzenli olarak RMS kullandığı bir kuruluşta, ortalama bir kullanıcının saatte 15 e-posta iletisi ve saatte 3 belge veya başka bir dosya koruması beklenebilir. Bu gereksinimlere dayanarak, RMS sunucularının saatte 1.890.000 lisans teslim etmesi gerekir; bu da saniyede 525 lisans demektir. Bu ortalama kullanım gereksinimini verir; bu rakam 3 ile çarpıldığında ise en yüksek kullanım olarak saniyede 1575 lisans elde edilir.  
    Bu hesaplama esas alındığında, kullanım çok yüksek olacaktır ve 32 RMS sunucusu geçerli kullanıcı gereksinimlerini karşılamaya yeterliyken, 51 RMS sunucusu geçerli kullanıcı gereksinimlerini karşılayacağı gibi büyümeye de açık olmayı sağlayacaktır.
  
Hesaplamalarınız saniyede 30 ila 50 lisans teslim edildiğini gösteriyorsa, bir RMS sunucusuna daha gereksiniminiz var demektir.
