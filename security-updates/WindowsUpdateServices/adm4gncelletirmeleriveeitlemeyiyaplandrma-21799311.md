---
TOCTitle: 'Adım 4: Güncelleştirmeleri ve Eşitlemeyi Yapılandırma'
Title: 'Adım 4: Güncelleştirmeleri ve Eşitlemeyi Yapılandırma'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21799311
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939924(v=WS.10)'
---

Adım 4: Güncelleştirmeleri ve Eşitlemeyi Yapılandırma
=====================================================

Bu bölümde, Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) kullanarak karşıdan yüklemek istediğiniz bir güncelleştirmeler kümesinin nasıl yapılandırılacağı anlatılmaktadır.

Adım 4 Yordamlar
----------------

WSUS Yapılandırma Sihirbazı'nı veya WSUS Yönetim Konsolu'nu kullanarak bu yordamları uygulayabilirsiniz.

1.  Akış yukarı sunucunuz ve proxy sunucunuz hakkındaki bilgileri kaydetme ve karşıdan yükleme.
2.  Güncelleştirmelerin dilini seçme.
3.  Güncelleştirmelerini almak istediğiniz ürünleri seçme.
4.  Güncelleştirmelerin sınıflandırmalarını seçme.
5.  Bu sunucu için eşitleme zamanlamasını belirtme.

Ağ bağlantısını yapılandırdıktan sonra, WSUS sunucusunu eşitleyerek güncelleştirmeleri karşıdan yükleyebilirsiniz. WSUS sunucusu Microsoft Update sitesiyle iletişim kurduğunda eşitleme başlar. WSUS iletişim kurduktan sonra, son eşitlemeden sonra kullanıma sunulan yeni güncelleştirmeler olup olmadığını belirler. WSUS sunucusunu ilk defa eşitlediğinizde, tüm güncelleştirmeler kullanılabilir ve yükleme onayınız için hazır olur. İlk eşitleme uzun sürebilir.

Bu bölümdeki yordamlarda, varsayılan ayarlarla eşitleme açıklanmaktadır. WSUS 3.0 SP2 ayrıca eşitleme sırasında bant genişliğini en aza indirgemenizi sağlayan seçenekler de içerir.

Windows Server Update Services Yapılandırma Sihirbazı'nı Kullanıyorsanız
------------------------------------------------------------------------

Adım 3 yordamlarında, akış yukarı sunucu ve proxy sunucu yapılandırmasını tamamlamıştınız. Sonraki yordamlar dizisi, bu yapılandırma sihirbazının **Akış Yukarı Sunucuya Bağlan** sayfasında başlar.

**Akış yukarı sunucu ve proxy bilgilerini kaydetmek ve karşıdan yüklemek için**
1.  Yapılandırma sihirbazının Akış Yukarı Sunucuya Bağlan sayfasında, **Bağlanmaya Başla** düğmesini tıklatın. Bu işlem sonucunda ayarlarınız kaydedilip karşıya yüklenir ve kullanılabilir güncelleştirmelerle ilgili bilgi toplanır.

2.  Bağlantı kurulurken, **Bağlanmayı Durdur** düğmesi görüntülenir. Bağlantıda sorun varsa, **Bağlanmayı Durdur**'u tıklatın, sorunları düzeltin ve bağlantıyı yeniden başlatın.

3.  Karşıdan yükleme başarıyla tamamlandıktan sonra **İleri**'yi tıklatın.

**Güncelleştirme dillerini seçmek için**
1.  Dilleri Seç sayfası, tüm dillerdeki güncelleştirmeleri veya dillerin bir alt kümesindeki güncelleştirmeleri almanızı sağlar. Bir dil alt kümesinin seçilmesi disk alanından kazandıracaktır, ancak söz konusu WSUS sunucusunun tüm istemcilerinin gerek duyacağı dillerin tümünün seçilmesi de önemlidir.

    Yalnızca belirli dillerdeki güncelleştirmeleri almayı seçerseniz, **Yalnızca bu dillerdeki güncelleştirmeleri yükle**'yi seçin ve sonra güncelleştirmelerini istediğiniz dilleri seçin.

2.  **İleri**'yi tıklatın.

**Güncelleştirme ürünlerini seçmek için**
1.  Ürünleri Seç sayfası, güncelleştirmelerini almak istediğiniz ürünleri seçmenizi sağlar. Windows gibi ürün kategorilerini veya Windows Server 2008 gibi belirli ürünleri seçin. Bir ürün kategorisinin seçilmesi, o kategorideki tüm ürünlerin seçilmesine neden olur.

2.  **İleri**'yi tıklatın.

**Güncelleştirme sınıflandırmalarını seçmek için**
1.  Sınıflandırmaları Seç sayfası, almak istediğiniz güncelleştirme sınıflandırmalarını seçmenizi sağlar. Tüm sınıflandırmaları veya bir alt kümesini seçin.

2.  **İleri**'yi tıklatın

**Eşitleme zamanlamasını yapılandırmak için**
1.  Eşitleme Zamanlamasını Ayarla sayfasında, eşitlemeyi el ile veya otomatik olarak gerçekleştirmeyi seçersiniz.

    **El ile eşitle**'yi seçerseniz, WSUS Yönetim Konsolu'ndan eşitleme işlemini başlatmanız gerekir.

    **Otomatik olarak eşitle**'yi seçerseniz, WSUS sunucusu belirtilen aralıklarla eşitleme yapar. **İlk eşitleme** saatini ayarlayın ve bu sunucunun gerçekleştirmesini istediğiniz **Günlük eşitleme** sayısını belirtin. Örneğin, saat 3:00'da başlayarak günde dört eşitleme yapılmasını belirtirseniz, eşitlemeler 3:00, 9:00, 15:00 ve 21:00 saatlerinde yapılır.

2.  **İleri**'yi tıklatın.

3.  Bitti sayfasında, **Windows Server Update Services Yönetim ek bileşenini başlat** onay kutusunu seçili bırakarak WSUS Yönetim Konsolu'nu başlatabilir ve **İlk eşitlemeyi başlat** onay kutusunu seçili bırakarak ilk eşitlemeyi başlatabilirsiniz.

4.  **Son**'u tıklatın.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th style="border:1px solid black;" ><img src="images/Dd939924.Important(WS.10).gif" />Önemli</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Sunucu eşitleme yaparken yapılandırmada yaptığınız değişiklikleri kaydedemezsiniz. Eşitleme bitinceye kadar bekleyin ve değişikliklerinizi kaydedin.
    </td>
    </tr>
    </tbody>
    </table>
 

WSUS Yönetim Konsolu'nu Kullanıyorsanız
---------------------------------------

Aşağıdaki yordamda, WSUS Yönetim Konsolu kullanılarak yapılandırma adımlarının nasıl uygulanacağı açıklanmaktadır.

**Ürünleri ve güncelleştirme sınıflandırmalarını seçmek için**
1.  **Seçenekler** bölmesinde, **Ürünler ve Sınıflandırmalar**'ı tıklatın. **Ürünler** ve **Sınıflandırmalar** sekmelerinin bulunduğu bir iletişim kutusu görüntülenir.

2.  **Ürünler** sekmesinde, bu sunucunun güncelleştirmelerini almasını istediğiniz ürün kategorisini veya belirli ürünleri seçin ya da **Tüm Ürünler**'i seçin.

3.  **Sınıflandırmalar** sekmesinde, istediğiniz sınıflandırmaları seçin ya da **Tüm Sınıflandırmalar**'ı seçin.

4.  Seçimlerinizi kaydetmek için **Tamam**'ı tıklatın.

**Güncelleştirme dosyalarını ve dillerini seçmek için**
1.  **Seçenekler** bölmesinde, **Güncelleştirme Dosyaları ve Dilleri**'ni tıklatın. **Güncelleştirme Dosyaları** ve **Güncelleştirme Dilleri** sekmelerinin bulunduğu bir iletişim kutusu görüntülenir.

2.  **Güncelleştirme Dosyaları** sekmesinde, **Güncelleştirme dosyalarını bu sunucuda yerel olarak depola** seçeneğini veya tüm istemci bilgisayarların Microsoft Update'ten yükleme yapmasını seçin. Güncelleştirme dosyalarını bu sunucuda depolamaya karar verirseniz, yalnızca onaylanan güncelleştirmelerin mi yoksa hızlı yükleme dosyalarının mı karşıdan yükleneceğine karar verebilirsiniz.

3.  **Güncelleştirme Dilleri** sekmesinde, güncelleştirme dosyalarını yerel olarak depoluyorsanız, **Güncelleştirmeleri tüm dillerde yükle** (varsayılan) veya **Yalnızca belirtilen dillerdeki güncelleştirmeleri yükle** seçeneğini belirleyebilirsiniz. Bu WSUS sunucusunun akış aşağı sunucuları varsa, yalnızca akış yukarı sunucuda belirtilen dillerdeki güncelleştirmeleri alabilir.

4.  **Tamam**'ı tıklatarak bu ayarları kaydedin.

**WSUS sunucusunu eşitlemek için**
1.  **Seçenekler** panelinde, **Eşitleme Zamanlaması**'nı tıklatın.

2.  **Eşitleme Zamanlaması** sekmesinde, eşitlemeyi el ile veya otomatik olarak gerçekleştirmeyi seçersiniz.

    **El ile eşitle**'yi seçerseniz, WSUS Yönetim Konsolu'ndan eşitleme işlemini başlatmanız gerekir.

    **Otomatik olarak eşitle**'yi seçerseniz, WSUS sunucusu belirtilen aralıklarla eşitleme yapar. **İlk eşitleme** saatini ayarlayın ve bu sunucunun gerçekleştirmesini istediğiniz **Günlük eşitleme** sayısını belirtin. Örneğin, saat 3:00'da başlayarak günde dört eşitleme yapılmasını belirtirseniz, eşitlemeler 3:00, 9:00, 15:00 ve 21:00 saatlerinde yapılır.

3.  Seçimlerinizi kaydetmek için **Tamam**'ı tıklatın.

4.  WSUS Yönetim Konsolu'nun gezinti bölmesinde **Eşitlemeler**'i seçin.

5.  Sağ tıklatın veya sağdaki **Eylemler** bölmesine gidin ve sonra **Şimdi Eşitle**'yi tıklatın.

    Konsolun sağ tarafında **Eylemler** bölmesini görmüyorsanız, konsol araç çubuğunda **Görünüm**'ü tıklatın, **Özelleştir**'i tıklatın ve **Eylem bölmesi** onay kutusunun seçili olduğundan emin olun.

6.  Eşitleme tamamlandıktan sonra, güncelleştirmelerin listesini görüntülemek için sol bölmede **Güncelleştirmeler**'i tıklatın.

Sonraki adım
------------

[Adım 5: İstemci Güncelleştirmelerini Yapılandırma](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
