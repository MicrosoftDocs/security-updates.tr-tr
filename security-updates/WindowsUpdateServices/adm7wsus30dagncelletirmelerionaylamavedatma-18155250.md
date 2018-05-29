---
TOCTitle: 'Adım 7: WSUS 3.0''da Güncelleştirmeleri Onaylama ve Dağıtma'
Title: 'Adım 7: WSUS 3.0''da Güncelleştirmeleri Onaylama ve Dağıtma'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18155250
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708475(v=WS.10)'
---

Adım 7: WSUS 3.0'da Güncelleştirmeleri Onaylama ve Dağıtma
==========================================================

Bu adımda, sınama grubu içindeki herhangi bir sınama istemcisi bilgisayarı için bir güncelleştirmeyi onaylarsınız. Gruptaki bilgisayarlar izleyen 24 saat içinde WSUS sunucusuyla iletişim kurar. Bu sürenin sonunda, bu güncelleştirmelerin bilgisayarlara dağıtılıp dağıtılmadığını belirlemek için WSUS raporlama özelliğini kullanabilirsiniz. Sınama olumlu sonuçlanırsa, aynı güncelleştirmeleri kuruluşunuzdaki diğer bilgisayarlar için onaylayabilirsiniz.

**Adım 7 aşağıdaki yordamları içerir**

-   Güncelleştirmeleri onaylama ve dağıtma.
-   Güncelleştirmenin durumunu denetleme.

**Güncelleştirmeleri onaylamak ve dağıtmak için**
1.  WSUS Yönetimi konsolunda, **Güncelleştirmeler**'i tıklatın. Bu yapıldığında, varsayılan görünümlerde (**Tüm Güncelleştirmeler**, **Kritik Güncelleştirmeler**, **Güvenlik Güncelleştirmeleri** ve **WSUS Güncelleştirmeleri**) güncelleştirmelerin bir özeti görüntülenir. Bu yordam için **Tüm Güncelleştirmeler**'i kullanın.

2.  Güncelleştirmeler listesinde, yüklenmek üzere onaylamak istediğiniz güncelleştirmeleri seçin. Seçilen bir güncelleştirmeyle ilgili bilgiler Güncelleştirmeler bölmesinin en alt bölmesinde görülebilir. Birbirini izleyen birden fazla güncelleştirmeyi seçmek için, **ÜSTKRKT** tuşunu basılı tutarak güncelleştirmeleri tıklatın; birbirini izlemeyen birden fazla güncelleştirmeyi seçmek için **CTRL** tuşunu basılı tutarak güncelleştirmeleri tıklatın.

3.  Seçimi sağ tıklatın ve **Onayla**'yı tıklatın. **Güncelleştirmeleri Onayla** iletişim kutusu görüntülenir.

4.  Gruplardan birini seçin (örneğin, **Test**) ve solundaki oku tıklatın. **Yükleme için Onaylandı**, **Kaldırma için Onaylandı**, **Onaylanmadı**, **Son Tarih**, **Üst ile Aynı** ve **Alt Öğelere Uygula** seçenekleri bulunan bir bağlam menüsü göreceksiniz. **Yükleme için Onaylandı**'yı ve sonra **Tamam**'ı tıklatın.

5.  Güncelleştirmelerin onaylanmasıyla ilgili farklı görevlerin ilerleyişini gösteren yeni bir pencere (**Onaylama İlerlemesi**) göreceksiniz. Onaylama tamamlandığında, bu pencereyi kapatmak için **Kapat**'ı tıklatın.

| ![](/security-updates/images/Cc708475.note(WS.10).gif)Not                                                     |
|--------------------------------------------------------------------------------------------------------------------------|
| Son tarihleri ayarlama ve güncelleştirmeleri kaldırma gibi, güncelleştirmeleri onaylamayla ilgili birçok seçenek vardır. |

24 saat sonra, güncelleştirmelerin bilgisayarlara dağıtılıp dağıtılmadığını belirlemek için WSUS raporlama özelliğini kullanabilirsiniz.

**Bir güncelleştirmenin durumunu denetlemek için**
1.  WSUS Yönetimi konsolunda, sol bölmedeki **Raporlar**'ı tıklatın.

2.  **Raporlar** sayfasında, birkaç tane standartlaştırılmış rapor görürsünüz. **Özet Güncelleştirme Durumu** raporunu tıklatın. **Güncelleştirmeler Raporu** penceresini görürsünüz.

3.  Güncelleştirme listesine filtre uygulamak istiyorsanız, kullanmak istediğiniz ölçütleri (örneğin, **Bu sınıflandırmalardaki güncelleştirmeleri ekle**) seçin ve pencerenin araç çubuğundaki **Raporu Çalıştır**'ı tıklatın.

4.  **Güncelleştirmeler Raporu** bölmesini görürsünüz. Tek tek güncelleştirmelerin durumunu denetlemek için bölmenin sol bölümünde güncelleştirmeleri seçebilirsiniz. Rapor bölmesinin son bölümü güncelleştirmenin durum özetini gösterir.

5.  Araç çubuğunda uygun simgeyi tıklatarak bu raporu kaydedebilir veya yazdırabilirsiniz.

Güncelleştirmeler sınama grubuna başarıyla dağıtıldıysa, kuruluşunuzdaki diğer bilgisayarlar için aynı güncelleştirmeleri onaylayabilirsiniz.
