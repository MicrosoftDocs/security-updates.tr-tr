---
TOCTitle: 'Adım 4: Güncelleştirmeleri Yapılandırma ve Eşitlemeyi Ayarlama'
Title: 'Adım 4: Güncelleştirmeleri Yapılandırma ve Eşitlemeyi Ayarlama'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18155175
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708447(v=WS.10)'
---

Adım 4: Güncelleştirmeleri Yapılandırma ve Eşitlemeyi Ayarlama
==============================================================

Güncelleştirmeleri karşıdan yüklemeden önce, hangi güncelleştirmeleri karşıdan yüklemek istediğinizi belirtmeniz gerekir. Bu bölümde, karşıdan yüklemek istediğiniz güncelleştirme kümesini nasıl ayarlayacağınız anlatılmaktadır.

Bu adımdaki yordamlar aşağıdakilerin nasıl yapılacağını anlatır:

-   Akış yukarı sunucunuz ve proxy sunucunuz hakkındaki bilgileri kaydetme ve karşıdan yükleme.
-   İstediğiniz güncelleştirmelerin dilini seçme.
-   Güncelleştirmelerini almak istediğiniz ürünleri seçme.
-   İstediğiniz güncelleştirme sınıflandırmalarını seçme.
-   Bu sunucu için eşitleme zamanlamasını belirtme.

Sonraki beş yordam, yapılandırma sihirbazını kullanarak güncelleştirmelerinizi nasıl yapılandıracağınızı anlatır. Daha sonraki yordamlar, bu yapılandırmanın WSUS Yönetimi konsolundan belirli seçenekler seçilerek nasıl gerçekleştirileceğini anlatır.

**Akış yukarı sunucu ve proxy bilgilerini kaydetme ve karşıdan yükleme**
1.  Akış yukarı sunucu ve proxy sunucu yapılandırmasını yapılandırma sihirbazında tamamlamış olmanız ve **Akış Yukarı Sunucuya Bağlan** sayfasını görmeniz gerekir.

2.  **Bağlanmaya Başla** düğmesini tıklatın; bu düğme ayarlarınızı kaydedip karşıya yükler ve kullanılabilir güncelleştirmelerle ilgili bilgileri alır.

3.  Bağlantı kurulurken, **Bağlanmayı Durdur** düğmesi görüntülenir. Bağlantıda sorun varsa, **Bağlanmayı Durdur**'u tıklatın, sorunları düzeltin ve bağlantıyı yeniden başlatın.

4.  Karşıdan yükleme başarıyla tamamlandıktan sonra, **Dilleri Seç** sayfasına gitmek için **İleri**'yi tıklatın veya soldaki bölmeden farklı bir sayfa seçin.

**Güncelleştirme dillerini seçme**
1.  **Dilleri Seç** sayfası, tüm dillerdeki güncelleştirmeleri veya dillerin bir alt kümesindeki güncelleştirmeleri almanızı sağlar. Bir dil alt kümesinin seçilmesi disk alanından kazandıracaktır, ancak söz konusu WSUS sunucusunun tüm istemcilerinin gerek duyacağı dillerin tümünün seçilmesi de önemlidir.

2.  Yalnızca bir kaç dildeki güncelleştirmeleri almayı seçerseniz, **Yalnızca bu dillerdeki güncelleştirmeleri yükle**'yi seçin ve sonra güncelleştirmelerini istediğiniz dilleri seçin. **Ürünleri Seç** sayfasına gitmek için **İleri**'yi tıklatın veya soldaki bölmeden farklı bir sayfa seçin.

**Güncelleştirme ürünlerini seçme**
1.  **Ürünleri Seç** sayfası, güncelleştirmelerini almak istediğiniz ürünleri seçmenizi sağlar.

2.  Windows gibi ürün kategorilerini veya Windows Server 2003 gibi özel ürünleri denetleyebilirsiniz. Ürün kategorisi seçme altındaki tüm ürünlerin seçilmesine neden olur. **Sınıflandırmaları Seç** sayfasına ilerlemek için **İleri**'yi tıklatın veya soldaki bölmeden farklı bir sayfa seçin.

**Güncelleştirme sınıflandırmalarını seçme**
1.  **Sınıflandırmaları Seç** sayfası, almak istediğiniz güncelleştirme sınıflandırmalarını seçmenizi sağlar. Tüm sınıflandırmaları veya bir alt kümesini seçebilirsiniz.

2.  **Eşitleme Zamanlamasını Yapılandır** sayfasına ilerlemek için **İleri**'yi tıklatın veya soldaki bölmeden farklı bir sayfa seçin.

**Eşitleme zamanlamasını yapılandırma**
1.  **Eşitleme Zamanlamasını Yapılandır** sayfasını görürsünüz; bu sayfa eşitlemelerin el ile mi yoksa otomatik olarak mı gerçekleştirileceğini seçmenizi sağlar.

2.  Bu sunucuda el ile eşitlemeyi seçerseniz, WSUS yönetim konsolundan eşitleme işlemini başlatmanız gerekir.

3.  Otomatik olarak eşitlemeyi seçerseniz, WSUS sunucusu belirtilen aralıklarla eşitleme yapar. İlk eşitleme saatini ayarlayın ve bu sunucunun gerçekleştirmesini istediğiniz günlük eşitleme sayısını belirtin. Örneğin, saat 3:00'da başlayarak günde dört eşitleme yapılmasını belirtirseniz, eşitlemeler 3:00, 9:00, 15:00 ve 21:00 saatlerinde yapılır.

Yukarıdaki yapılandırma adımlarının tümünü tamamladıktan sonra, yapılandırma sihirbazında **Bitti** sayfasını seçin. **Windows Server Update Services Yönetim ek bileşenini başlat** onay kutusunu seçili bırakarak WSUS Yönetimi konsolunu başlatabilir ve **İlk eşitlemeyi başlat** onay kutusunu seçili bırakarak ilk eşitlemeyi başlatabilirsiniz.

| ![](images/Cc708447.note(WS.10).gif)Not                                                                                    |
|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sunucu eşitleme yaparken yapılandırmada yaptığınız değişiklikleri kaydedemezsiniz. Değişikliklerinizi kaydetmek için eşitleme bitinceye kadar bekleyin. |

![](images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

Aşağıdaki yordamlarda, yukarıdaki yapılandırma adımlarının WSUS Yönetimi konsolunun **Seçenekler** sayfası kullanılarak nasıl gerçekleştirileceği anlatılmaktadır:

-   Ürünleri ve sınıflandırmaları seçme
-   Güncelleştirme dosyaları ve dilleri

**Ürünleri ve sınıflandırmaları seçme**
1.  WSUS Yönetimi konsolunu başlatın: **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gidin, **Yönetimsel Araçlar**'ın üzerine gidin ve sonra **Microsoft Windows Server Update Services**'ı tıklatın.

2.  Sol bölmedeki WSUS sunucunuzun altında **Seçenekler**'i seçin.

3.  Ortadaki bölmede, **Ürünler ve Sınıflandırmalar**'ı seçin.

4.  İki sekme bulunan bir iletişim kutusu görürsünüz: **Ürünler** ve **Sınıflandırmalar**.

5.  **Ürünler** sekmesinde, bu sunucunun güncelleştirmelerini almasını istediğiniz ürün kategorisini veya belirli ürünü seçin ya da **Tüm Ürünler**'i seçin.

6.  **Sınıflandırmalar** sekmesinde, istediğiniz sınıflandırmaları seçin ya da **Tüm Sınıflandırmalar**'ı seçin.

7.  Seçimlerinizi kaydetmek için **Tamam**'ı tıklatın.

**Güncelleştirme dosyaları ve dilleri**
1.  **Seçenekler** sayfasında, **Güncelleştirme Dosyaları ve Dilleri**'ni seçin.

2.  İki sekme bulunan bir iletişim kutusu görürsünüz: **Güncelleştirme Dosyaları** ve **Güncelleştirme Dilleri**.

3.  **Güncelleştirme Dosyaları** sekmesinde, güncelleştirme dosyalarının yerel olarak mı depolanacağını yoksa tüm istemci bilgisayarların Microsoft Update'ten mi yükleyeceğini seçebilirsiniz. Güncelleştirme dosyalarını bu sunucuda depolamayı seçerseniz, yalnızca onaylanan güncelleştirmelerin mi yoksa hızlı yükleme dosyalarının mı karşıdan yükleneceğini seçebilirsiniz.

4.  **Güncelleştirme Dilleri** sekmesinde, güncelleştirmeleri tüm diller için almayı (varsayılan) veya yalnızca belirli diller için almayı seçebilirsiniz. Bu WSUS sunucusunun akış aşağı sunucuları varsa, yalnızca akış yukarı sunucuda belirtilen dillerdeki güncelleştirmeleri alabilirler.

5.  **Tamam**'ı tıklatarak bu ayarları kaydedin.

Ağ bağlantısını yapılandırdıktan sonra, WSUS sunucusunu eşitleyerek güncelleştirmeleri karşıdan yükleyebilirsiniz.

Eşitleme, WSUS sunucusunun Microsoft Update sitesiyle iletişim kurmasını içerir. İletişim kurulduktan sonra WSUS, son eşitlemeden sonra kullanıma sunulan yeni güncelleştirmeler olup olmadığını belirler. WSUS sunucusunu ilk kez eşitlediğinizden tüm güncelleştirmeler kullanılabilir durumdadır ve yükleme için onayınıza hazırdır. İlk eşitleme oldukça uzun sürebilir.

| ![](images/Cc708447.note(WS.10).gif)Not                                                                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu belgede, varsayılan ayarlarla eşitleme açıklanır; ancak WSUS, eşitleme sırasında bant genişliğini en aza indirmenizi sağlayan seçenekler içerir. |

**WSUS sunucunuzu eşitlemek için**
1.  WSUS Yönetimi konsolunda, **Eşitlemeler**'i seçin.

2.  Sağ tıklatın veya sağdaki **Eylemler** bölmesine gidin ve sonra **Şimdi eşitle**'yi tıklatın.

| ![](images/Cc708447.note(WS.10).gif)Not                                                                                                                                  |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Konsolun sağ tarafında **Eylemler** bölmesini görmüyorsanız, konsol araç çubuğunda **Görünüm**'ü tıklatın, **Özelleştir**'i tıklatın ve **Eylem bölmesi** onay kutusunun seçili olduğundan emin olun. |

Eşitleme tamamlandıktan sonra, güncelleştirmelerin listesini görmek için sol bölmede **Güncelleştirmeler**'i tıklatın.
