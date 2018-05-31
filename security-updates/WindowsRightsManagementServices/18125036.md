---
TOCTitle: 'RMS Service Pack 2 (SP2) ile Dağıtımınızı Güncelleştirme'
Title: 'RMS Service Pack 2 (SP2) ile Dağıtımınızı Güncelleştirme'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18125036
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720225(v=WS.10)'
---

RMS Service Pack 2 (SP2) ile Dağıtımınızı Güncelleştirme
========================================================

Bu bölüm Microsoft® Windows® Rights Management Services (RMS) Service Pack 2'yi (SP2) varolan bir RMS dağıtımı olan bir kuruluşu yüklemeniz yardımcı olacak bilgiler verir. Yalnızca önceden RMS dağıtmış kuruluşların RMS SP2 ile güncelleştirmeleri gerekir. İlk kez RMS dağıtan kuruluşlar RMS SP2'yi, bu belge koleksiyonundaki RMS Dağıtımı Planlama ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) ve RMS sistemi dağıtma ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) bölümündeki yönergeleri izleyerek dağıtabilir.

RMS SP2'yi varolan RMS SP1 yüklemenizi kaldırmadan yükleyebilirsiniz. RMS SP2 kurulum programı RMS SP1'in yüklü olduğunu algılar ve gerektiği gibi ek özellikleri ve ayarları ekler.

| ![](/security-updates/images/Cc720225.note(WS.10).gif)Not                                                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hizmet paketi içermeyen RMS sunucusundan RMS SP2'ye yükseltme desteklenmez. RMS sunucusunu hizmet paketi olmadan kullanıyorsanız, RMS SP2'ye yükseltmeden önce RMS SP1'e yükseltmeniz gerekir. RMS istemcisi, RMS istemcisinin herhangi bir önceki sürümünden yükseltilebilir. |

**Bu konuda**

-   [RMS SP2 Güncelleştirmesine Hazırlanma](#bkmk_preparingforsp2update)
-   [RMS SP2 Güncelleştirmesini Gerçekleştirme](#bkmk_performingsp2update)
-   [Kümeleri Güncelleştirme](#bkmk_updateclusters)
-   [RMS İstemcileri Güncelleştirme](#bkmk_updateclients)
-   [RMS sürüm 1.0 ile Birlikte Çalışabilirlik](#bkmk_interop)
-   [RMS SP2'yi Kaldırma](#bkmk_removingrms)

<span id="bkmk_PreparingForSP2Update"></span>
RMS SP2 Güncelleştirmesine Hazırlanma
-------------------------------------

RMS SP2 güncelleştirmesi kesinti olmadan RMS çalıştırmaya devam etmenize izin vermek için tasarlanmıştır. Ancak RMS kümenizi yükseltmeden önce şunları yapmanız önerilir:

-   Yapılandırma veritabanını ve RMS özel anahtarını yedekleyin. Daha fazla bilgi için, bu belge koleksiyonunda RMS Sistem Yedekleri'ne ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) bakın.
-   Yazılım tabanlı bir özel anahtar kullanıyorsanız, RMS özel anahtar parolanızın oluğundan emin olun.
-   Önceden günlüğe kaydedilmiş istatistikleri saklamak istiyorsanız, günlük veritabanını yedekleyin.
-   İstemcilerinizde ve sunucularınızda en son kritik ve güvenlik güncelleştirmelerin bulunduğundan emin olun. Tüm kritik ve güvenlik güncelleştirmelerine sahip olduğunuzu doğrulamak için, **Başlat**'ı, **Windows Update**'i tıklatın ve ardından ekranınızda görünen yönergeleri izleyin.

<span id="bkmk_PerformingSP2Update"></span>
RMS SP2 Güncelleştirmesini Gerçekleştirme
-----------------------------------------

Windows Rights Management Services Service Pack 2 Kurulum Sihirbazı RMS yüklemenizi algıladığında, geçerli RMS SP1 yüklemenize bakar ve yalnızca yeni dosyaları ekler veya RMS SP2'de değişmesi gereken dosyaları değiştirir. RMS'yi başarıyla çalıştırmaktaysanız, RMS çalıştırmaya devam etmek için RMS SP2 yükledikten sonra değişiklik veya ek yapılandırma yapmanız gerekmez.

<span id="bkmk_UpdateClusters"></span>
Kümeleri Güncelleştirme
-----------------------

Bir küme yapılandırmasına RMS yüklediyseniz, yüklemenizdeki güncelleştirmenin etkisini en aza indirmek için kümelerinizin güncelleştirilmesini planlamalısınız. RMS SP2'yi kuruluşunuza en iyi nasıl uygulanacağını belirlerken aşağıdaki önerileri dikkate alın:

-   En iyi uygulama olarak, RMS SP2'yi aynı anda kümenin bir kısmına yükleyin, böylece kümenin yükseltilmesi daha öngörülebilir ve yükseltme sırasında hizmette bir düşüşe neden olma olasılığını azaltır.
-   Birden fazla RMS kümesi varsa, önce kök sertifikası kümelerini ve ardından alt kayıtlı lisans kümelerini yükseltmelisiniz.
-   Ormanlar arasında grup genişletme kullanıyorsanız, RMS sunucularının ormanlar arasında grup üyeliğini genişletme yeteneğini etkilemeden ormanlardaki kümeleri bağımsız olarak yükseltebilirsiniz.
-   RMS SP2, RMS SP1 ve RMS sürüm 1.0 sunucusu yalnızca farklı Active Directory ormanlarındaysa bir arada olabilir ve birlikte çalışabilir. Aynı kümede RMS sunucusunun farklı sürümlerinin olması önerilmez.
-   RMS SP2 kurulum paketi, RMS SP2'nin bir sunucu üzerinde yeni dağıtımını yüklemek için de kullanılabilir; RMS SP1'in yüklenmesini gerektirmez.

<span id="bkmk_UpdateClients"></span>
RMS İstemcileri Güncelleştirme
------------------------------

Yeni RMS SP2 istemcisi, Windows Update veya Microsoft Yükleme Merkezi'nde bulunabilir. RMS SP2 istemcisi kurulum paketi, bir bilgisayara yeni RMS SP2 sürümünü yüklemek için de kullanılabilir; RMS sürüm 1.0 istemcisinin yüklü olmasını gerektirmez. RMS SP2 istemcisi RMS sürüm 1.0 gerektiren RMS etkin uygulamalarla birlikte kullanılabilmesini sağlamak için geriye doğru uyumluluk içermektedir.

RMS istemcisini güncelleştirme ve yükleme hakkında daha fazla bilgi için, bkz. RMS İstemcisini Dağıtma ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)).

<span id="bkmk_InterOp"></span>
RMS Sürüm 1.0 ile Birlikte Çalışabilirlik
-----------------------------------------

RMS SP2 bir çok yenilik ve performans gelişimi sağladığı için, sonraki yükseltme döngüsünde yüklemelisiniz. RMS SP2 çalıştıran RMS sunucuları ve istemcileri, RMS SP2 çalıştırmayan RMS sunucuları ve istemcileriyle tam olarak birlikte çalışabiliyor olmasına rağmen, karma ortamdaki çalışma şekilleriyle ilgili aşağıdaki farklılıkların olduğunu unutmayın:

-   Yalnızca RMS SP1 ve sonraki sürümleri çalıştıran sunucular çevrimdışı kayıt yapabilirler.
-   Yalnızca RMS SP1 ve sonraki sürümleri çalıştıran istemcilere kendini etkinleştirebilir.
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
<th style="border:1px solid black;" >Sürüm 1 istemcileriyle desteklenen özellikler</th>
<th style="border:1px solid black;" >SP2 istemcileriyle desteklenen özellikler</th>
<th style="border:1px solid black;" >Karma istemci ortamlarında desteklenen özellikler</th>
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
SP2 istemciler için, istemciler kendini etkinleştirebilir.
Sürüm 1 istemcileri için, istemciler Internet üzerinden etkinleştirilmelidir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Önceki tüm özellikler
Sunucunun çevrimdışı kaydı.
Kendini etkinleştiren istemciler yok.</td>
<td style="border:1px solid black;">Tüm SP1 özellikleri.
Sunucunun çevrimdışı kaydı.
Kendini etkinleştiren istemciler.
Sunucu kasası.
Microsoft SQL Server™ 2005 kutunun dışında desteklenir.</td>
<td style="border:1px solid black;">Önceki tüm özellikler artı SP2 özellikleri.
Sunucunun çevrimdışı kaydı.
SP2 istemciler için, istemciler kendini etkinleştirebilir.
Sürüm 1 istemcileri için, istemciler Internet üzerinden etkinleştirilmelidir.</td>
</tr>
</tbody>
</table>
 

<span id="bkmk_RemovingRMS"></span>
RMS SP2'yi Kaldırma
-------------------

RMS SP2 yükledikten sonra RMS sunucunuzu önceki yapılandırmasına döndürmek isterseniz, RMS SP2'yi kaldırmak için **Denetim Masası**'nda **Program Ekle veya Kaldır**'ı tıklatın.
