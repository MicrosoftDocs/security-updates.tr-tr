---
TOCTitle: 'RMS Service Pack 1 (SP1) ile Dağıtımı Güncelleştirme'
Title: 'RMS Service Pack 1 (SP1) ile Dağıtımı Güncelleştirme'
ms:assetid: 'a562c4b0-15df-46db-9d61-24db74871cfa'
ms:contentKeyID: 18125207
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747714(v=WS.10)'
---

RMS Service Pack 1 (SP1) ile Dağıtımı Güncelleştirme
====================================================

Bu bölüm Microsoft® Windows® Rights Management Services (RMS) Service Pack 1'yi (SP1) varolan bir RMS dağıtımı olan bir kuruluşu yüklemeniz yardımcı olacak bilgiler verir. Yalnızca önceden RMS dağıtmış kuruluşların RMS SP1 ile güncelleştirmeleri gerekir. İlk kez RMS dağıtan kuruluşlar RMS SP1'i, bu belge koleksiyonundaki RMS Dağıtımı Planlama ve RMS sistemi dağıtma bölümündeki yönergeleri izleyerek dağıtabilir.

RMS SP1'i varolan RMS yüklemenizi kaldırmadan yükleyebilirsiniz. RMS SP1 kurulum programı RMS'nin yüklü olduğunu algılar ve gerektiği gibi ek özellikleri ve ayarları ekler.

**Bu konuda**

-   [RMS SP1 Güncelleştirmesine Hazırlanma](#bkmk_1)
-   [RMS SP1 Güncelleştirmesini Gerçekleştirme](#bkmk_2)
-   [Kümeleri Güncelleştirme](#bkmk_3)
-   [RMS İstemcileri Güncelleştirme](#bkmk_4)
-   [RMS Sürüm 1.0 ile Birlikte Çalışabilirlik](#bkmk_5)
-   [RMS SP1'i Kaldırma](#bkmk_6)

<span id="BKMK_1"></span>
RMS SP1 Güncelleştirmesine Hazırlanma
-------------------------------------

RMS SP1 güncelleştirmesi kesinti olmadan RMS işlemlerine devam etmenize izin vermek için tasarlanmıştır. Ancak RMS sunucularınızı yükseltmeden önce şunları yapmanız önerilir:

-   Yapılandırma veritabanını ve RMS özel anahtarını yedekleyin. Daha fazla bilgi için, bu belge koleksiyonunda "RMS Dağıtımını Planlama" içindeki RMS Sistem Yedekleri'ne bakın.
-   RMS özel anahtar parolanızın oluğundan emin olun.
-   Önceden günlüğe kaydedilmiş istatistikleri saklamak istiyorsanız, günlük veritabanını yedekleyin.
-   İstemcilerinizde ve sunucularınızda en son kritik ve güvenlik güncelleştirmelerin bulunduğundan emin olun. Tüm kritik ve güvenlik güncelleştirmelerine sahip olduğunuzu doğrulamak için, **Başlat**'ı, **Windows Update**'i tıklatın ve ardından ekranınızda görünen yönergeleri izleyin.

<span id="BKMK_2"></span>
RMS SP1 Güncelleştirmesini Gerçekleştirme
-----------------------------------------

RMS SP1 Kurulum Sihirbazı RMS yüklemenizi algıladığında, geçerli RMS yüklemenize bakar ve yalnızca yeni dosyaları ekler veya RMS SP1'de değişmesi gereken dosyaları değiştirir. RMS'yi başarıyla çalıştırmaktaysanız, RMS çalıştırmaya devam etmek için RMS SP1 yükledikten sonra değişiklik veya ek yapılandırma yapmanız gerekmez.

<span id="BKMK_3"></span>
Kümeleri Güncelleştirme
-----------------------

Bir küme yapılandırmasına RMS yüklediyseniz, yüklemenizdeki güncelleştirmenin etkisini en aza indirmek için kümelerinizin güncelleştirilmesini planlamalısınız. RMS SP1'i kuruluşunuza en iyi nasıl uygulanacağını belirlerken aşağıdaki önerileri dikkate alın:

-   En iyi uygulama olarak, RMS SP1'i aynı anda kümenin bir kısmına yükleyin, böylece kümenin yükseltilmesi daha öngörülebilir ve yükseltme sırasında hizmette bir düşüşe neden olma olasılığını azaltır.
-   Birden fazla RMS kümesi varsa, önce kök sertifikası kümelerini ve ardından alt kayıtlı lisans kümelerini yükseltmelisiniz.
-   Ormanlar arasında grup genişletme kullanıyorsanız, RMS sunucularının ormanlar arasında grup üyeliğini genişletme yeteneğini etkilemeden ormanlardaki kümeleri bağımsız olarak yükseltebilirsiniz.
-   RMS SP1 ve RMS sürüm 1.0 sunucusu bir arada olabilir ve birlikte çalışabilir.
-   RMS SP1 kurulum paketi, RMS SP2'nin bir sunucu üzerinde yeni sürümünü yüklemek için de kullanılabilir; RMS sürüm 1'in yüklenmesini gerektirmez.

<span id="BKMK_4"></span>
RMS İstemcileri Güncelleştirme
------------------------------

Yeni RMS istemcisi, RMS SP1 içinde bulunur. RMS SP1 istemcisi kurulum paketi, bir bilgisayara yeni RMS SP1 sürümünü yüklemek için de kullanılabilir; RMS sürüm 1.0 istemcisinin yüklü olmasını gerektirmez. RMS SP1 istemcisi RMS sürüm 1.0 gerektiren RMS etkin uygulamalarla birlikte kullanılabilmesini sağlamak için geriye doğru uyumluluk içermektedir.

Bu yeni RMS istemcisi aşağıdaki özellikleri sağlar:

-   İstemcinin kasa yüklemek için artık Microsoft'a Internet üzerinden bağlanması gerekmez.
-   RMS istemcisini bir SMS veya grup ilkesi kullanarak yüklerseniz, yükleme için yönetici ayrıcalıkları gerekmez.
-   RMS SP1 istemcisi, hizmetin RMS korumalı içeriği tüketmesi ve yeniden dağıtmasına izin vermek için, Windows SharePoint® Services ve Exchange Server 2003 gibi, RMS etkin Windows Web hizmetleri veya sunucu tarafı uygulamalar için yeni bir sunucu kasası içerir (sunucu güvenlik işlemcisi olarak da bilinir). Bu kasa güvenilen sunucu uygulamaları içinde kullanıldığında yüksek performanslı ve ölçülebilir olacak şekilde tasarlanmıştır
-   RMS istemcisi FIPS 140-2 sertifikalı şifreleme algoritmaları kullanır. Bu sayede istemcinin FIPS uyumlu bir kuruluşta dağıtılması sağlanır.

<span id="BKMK_5"></span>
RMS Sürüm 1.0 ile Birlikte Çalışabilirlik
-----------------------------------------

RMS SP1 bir çok yenilik ve performans gelişimi sağladığı için, testinizi tamamladıktan sonra yüklemelisiniz. RMS SP1 çalıştıran RMS sunucuları ve istemcileri, RMS SP1 çalıştırmayan RMS sunucuları ve istemcileriyle tam olarak birlikte çalışabiliyor olmasına rağmen, karma ortamdaki çalışma şekilleriyle ilgili aşağıdaki farklılıkların olduğunu unutmayın:

-   Yalnızca RMS SP1 çalıştıran sunucular çevrimdışı kayıt yapabilirler.
-   Yalnızca RMS SP1 çalıştıran istemcilere kendini etkinleştirebilir.
-   Aşağıdaki tablo karma ortamların desteklenen işlevselliğini gösterir:

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
<th style="border:1px solid black;" >RMS Sunucu sürümü</th>
<th style="border:1px solid black;" >v1 istemcileriyle desteklenen özellikler</th>
<th style="border:1px solid black;" >SP1 istemcileriyle desteklenen özellikler</th>
<th style="border:1px solid black;" >Karma (v1 ve SP1) istemci ortamlarında desteklenen özellikler</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Önceki tüm özellikler
Sunucunun çevrimdışı kaydı yok. Sunucu Internet üzerinden kayıt yapmalıdır.
Kendini etkinleştiren istemciler yok.</td>
<td style="border:1px solid black;">Önceki tüm özellikler
Sunucunun çevrimdışı kaydı yok.
Kendini etkinleştiren istemciler.</td>
<td style="border:1px solid black;">Önceki tüm özellikler
SP1 istemciler için, istemciler kendini etkinleştirebilir.
Sürüm 1 istemcileri için, istemciler Internet üzerinden etkinleştirilmelidir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP1</td>
<td style="border:1px solid black;">Önceki tüm özellikler
Sunucunun çevrimdışı kaydı.
Kendini etkinleştiren istemciler yok.</td>
<td style="border:1px solid black;">Tüm SP1 özellikleri.
Sunucunun çevrimdışı kaydı.
Kendini etkinleştiren istemciler.
Sunucu kasası.</td>
<td style="border:1px solid black;">Önceki tüm özellikler artı SP1 özellikleri.
Sunucunun çevrimdışı kaydı.
SP1 istemciler için, istemciler kendini etkinleştirebilir.
Sürüm 1 istemcileri için, istemciler Internet üzerinden etkinleştirilmelidir.</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_6"></span>
RMS SP1'i Kaldırma
------------------

RMS SP1 yükledikten sonra RMS sunucunuzu önceki yapılandırmasına döndürmek isterseniz, RMS SP1'yi kaldırmak için **Denetim Masası**'nda **Program Ekle veya Kaldır**'ı tıklatın.

**Not**   RMS SP1 yüklemeden önce bir yapılandırma veritabanı yedeği aldıysanız, RMS SP1 tarafından yapılan tüm değişiklikleri tamamen kaldırmak için bu yedeği geri yükleyebilirsiniz. Yapılandırma veritabanını yedeklemediyseniz, geri yüklenen RMS yüklemesiyle birlikte RMS SP1 yüklemesinden kalan yapılandırma veritabanını kullanabilirsiniz. Geri yüklenen RMS yüklemesi, RMS SP1 yüklemesinin yapılandırma veritabanına eklemiş olduğu fazla alanları kullanmayacağı için yoksayar.
