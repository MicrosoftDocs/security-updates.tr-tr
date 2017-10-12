---
TOCTitle: 'Adım 7: WSUS Güncelleştirmelerini Onaylama ve Dağıtma'
Title: 'Adım 7: WSUS Güncelleştirmelerini Onaylama ve Dağıtma'
ms:assetid: 'c4e58e17-d5e3-4194-8f26-b459e0c03b86'
ms:contentKeyID: 21799275
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939909(v=WS.10)'
---

Adım 7: WSUS Güncelleştirmelerini Onaylama ve Dağıtma
=====================================================

Bu adımda, Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) için sınama grubunda herhangi bir bilgisayara yönelik güncelleştirmeyi onaylarsınız. Gruptaki bilgisayarlar, güncelleştirmeyi almak için izleyen 24 saat içinde WSUS sunucusuyla bağlantı kurar. Bu güncelleştirmelerin bilgisayarları sınamak üzere dağıtılıp dağıtılmadığını belirlemek için WSUS raporlama özelliğini kullanabilirsiniz. Sınamalar başarıyla tamamlandığında, kuruluşunuzda ilgili bilgisayar grupları için güncelleştirmeleri onaylayabilirsiniz.

Adım 7 Yordamlar
----------------

-   Güncelleştirmeleri onaylama ve dağıtma.
-   Güncelleştirmenin durumunu denetleme.

**Güncelleştirmeleri onaylamak ve dağıtmak için**
1.  WSUS Yönetim Konsolu'nda, **Güncelleştirmeler**'i tıklatın. **Tüm Güncelleştirmeler**, **Kritik Güncelleştirmeler**, **Güvenlik Güncelleştirmeleri** ve **WSUS Güncelleştirmeleri** için bir güncelleştirme durum özeti görüntülenir.

2.  **Tüm Güncelleştirmeler** bölümünde **Bilgisayarlara gereken güncelleştirmeler**'i tıklatın.

3.  Güncelleştirmeler listesinde, sınama bilgisayar grubunuza yüklenmek üzere onaylamak istediğiniz güncelleştirmeleri seçin. Seçilen bir güncelleştirmeyle ilgili bilgiler, Güncelleştirmeler bölmesinin en alt bölmesinde görülebilir. Birbirini izleyen birden fazla güncelleştirmeyi seçmek için, **ÜSTKRKT** tuşunu basılı tutarak güncelleştirmeleri tıklatın; birbirini izlemeyen birden fazla güncelleştirmeyi seçmek için **CTRL** tuşunu basılı tutarak güncelleştirmeleri tıklatın.

4.  Seçimi sağ tıklatın ve **Onayla**'yı tıklatın.

5.  **Güncelleştirmeleri Onayla** iletişim kutusunda sınama grubunuzu seçin ve AŞAĞI oku tıklatın.

6.  **Yükleme için Onaylandı**'yı ve sonra **Tamam**'ı tıklatın.

7.  Güncelleştirme onayını etkileyen görevlerin ilerlemesini gösteren Onaylama İlerlemesi penceresi görüntülenir. Onaylama tamamlandığında **Kapat**'ı tıklatın.

24 saat sonra, güncelleştirmelerin sınama grubu bilgisayarlarına dağıtılıp dağıtılmadığını belirlemek için WSUS Raporları özelliğini kullanabilirsiniz.

**Bir güncelleştirmenin durumunu denetlemek için**
1.  WSUS Yönetim Konsolu'nun gezinti bölmesinde **Raporlar**'ı tıklatın.

2.  **Raporlar** sayfasında **Özet Güncelleştirme Durumu** raporunu tıklatın. **Güncelleştirmeler Raporu** penceresi görüntülenir.

3.  Güncelleştirme listesine filtre uygulamak istiyorsanız, kullanmak istediğiniz ölçütleri (örneğin, **Bu sınıflandırmalardaki güncelleştirmeleri ekle**) seçin ve pencerenin araç çubuğundaki **Raporu Çalıştır**'ı tıklatın.

4.  **Güncelleştirmeler Raporu** bölmesini görürsünüz. Tek tek güncelleştirmelerin durumunu denetlemek için bölmenin sol bölümünde güncelleştirmeleri seçebilirsiniz. Rapor bölmesinin son bölümü güncelleştirmenin durum özetini gösterir.

5.  Araç çubuğunda ilgili simgeyi tıklatarak bu raporu kaydedebilir veya yazdırabilirsiniz.

6.  Güncelleştirmeleri sınadıktan sonra, kuruluşunuzdaki ilgili bilgisayar gruplarına yüklenmek üzere güncelleştirmeleri onaylayabilirsiniz.

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)

WSUS 3.0 SP2'yi kullanma hakkında daha fazla bilgi için, bkz:

WSUS Dağıtım Kılavuzu, [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832).

WSUS İşlemler Kılavuzu, [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838).
