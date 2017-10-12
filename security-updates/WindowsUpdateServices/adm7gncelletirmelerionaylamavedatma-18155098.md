---
TOCTitle: 'Adım 7: Güncelleştirmeleri Onaylama ve Dağıtma'
Title: 'Adım 7: Güncelleştirmeleri Onaylama ve Dağıtma'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18155098
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720504(v=WS.10)'
---

Adım 7: Güncelleştirmeleri Onaylama ve Dağıtma
==============================================

Bu adımda Test grubu içindeki test istemcisi bilgisayarları için güncelleştirmeyi onaylarsınız. Gruptaki bilgisayarlar izleyen 24 saat içinde WSUS sunucusuna kaydedilir. Bu sürenin sonunda, bu güncelleştirmelerin bilgisayarlara dağıtılıp dağıtılmadığını belirlemek için WSUS raporlama özelliğini kullanabilirsiniz. Sınama olumlu sonuçlanırsa, aynı güncelleştirmeyi kuruluşunuzdaki diğer bilgisayarlar için onaylayabilirsiniz.

Adım 7 aşağıdaki yordamları içerir:

-   Güncelleştirmeleri onaylama ve dağıtma.
-   Güncelleştirmelerin Durumu raporunu denetleme.

**Güncelleştirmeleri onaylamak ve dağıtmak için**
1.  WSUS konsolu araç çubuğunda, **Güncelleştirmeler**’i tıklatın. Varsayılan olarak, güncelleştirmeler listesine, yalnızca istemci bilgisayarlarda algılanmak üzere onaylanmış Kritik Güncelleştirmeler ve Güvenlik Güncelleştirmeleri'ni göstermek için filtre uygulanır. Bu yordam için varsayılan filtreyi kullanın.

2.  Güncelleştirmeler listesinde, yüklenmek üzere onaylamak istediğiniz güncelleştirmeleri seçin. Seçili güncelleştirmeyle ilgili bilgiler **Ayrıntılar** sekmesinde bulunur. Birbirini izleyen birden fazla güncelleştirmeyi seçmek için, seçim sırasında ÜSTKRKT tuşunu basılı tutun; art arda gelmeyen birden fazla güncelleştirmeyi seçmek için seçim sırasında CTRL tuşunu basılı tutun.

3.  **Güncelleştirme Görevleri**'nin altında **Onayı değiştir**'i tıklatın. **Güncelleştirmeleri Onayla** iletişim kutusu görüntülenir.

4.  **Seçili güncelleştirmelere yönelik grup onayı ayarları** listesinde Test grubunun **Onay** sütununda **Yükle**'yi ve ardından **Tamam**'ı tıklatın.

| ![](images/Cc720504.note(WS.10).gif)Not                                                                                                                                                                                   |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ayar son tarihleri ve güncelleştirmeleri kaldırma gibi güncelleştirmeleri onaylamayla ilgili çeşitli seçenekler vardır. Bunlar, “Microsoft Windows Server Update Services İşletim Kılavuzu” teknik incelemesinde ele alınmıştır (Belge İngilizce'dir). |

24 saat sonra, bu güncelleştirmelerin bilgisayarlara dağıtılıp dağıtılmadığını belirlemek için WSUS raporlama özelliğini kullanabilirsiniz.

**Güncelleştirmelerin Durumu raporunu denetlemek için**
1.  WSUS konsolu araç çubuğunda, **Raporlar**’ı tıklatın.

2.  **Raporlar** sayfasında **Güncelleştirmelerin Durumu**'nu tıklatın.

3.  Güncelleştirmeler listesine filtre uygulamak istiyorsanız, **Görüntüle**'nin altında kullanmak istediğiniz ölçütü seçin ve **Uygula**'yı tıklatın.

4.  Güncelleştirmenin durumunu önce bilgisayar grubuna, sonra da bilgisayara göre görmek istiyorsanız, güncelleştirmenin görünümünü gerektiği gibi genişletin.

5.  Güncelleştirmelerin Durumu raporunu yazdırmak istiyorsanız, **Görevler**'in altında **Raporu yazdır**'ı tıklatın.

Güncelleştirmeler Test grubuna başarıyla dağıtıldıysa, kuruluşunuzdaki diğer bilgisayarlar için aynı güncelleştirmeleri onaylayabilirsiniz.
