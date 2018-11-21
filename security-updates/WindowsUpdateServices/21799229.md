---
TOCTitle: 'Adım 6: Bilgisayar Gruplarını Yapılandırma'
Title: 'Adım 6: Bilgisayar Gruplarını Yapılandırma'
ms:assetid: '70518732-2179-4e41-9609-7f9999867f41'
ms:contentKeyID: 21799229
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939860(v=WS.10)'
---

Adım 6: Bilgisayar Gruplarını Yapılandırma
==========================================

Bilgisayar grupları, Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) dağıtımlarının önemli bir parçasını oluşturur. Bilgisayar grupları, güncelleştirmeleri sınamanızı ve belirli bilgisayarlara yönlendirmenizi sağlar. İki varsayılan bilgisayar grubu vardır: Tüm Bilgisayarlar ve Atanmamış Bilgisayarlar. Varsayılan olarak, her istemci bilgisayar WSUS sunucusuyla ilk kez iletişim kurduğunda, sunucu bu iki gruba da istemci bilgisayarı ekler.

Kuruluşunuzda güncelleştirmeleri yönetmek için ihtiyaç duyduğunuz sayıda özel bilgisayar grubu oluşturabilirsiniz. Bunu en iyi şekilde yapmak için, güncelleştirmeleri kuruluşunuzdaki diğer bilgisayarlara dağıtmadan önce sınamak üzere en az bir bilgisayar grubu oluşturun.

Adım 6 Yordamlar
----------------

1.  Sınama bilgisayar grubu oluşturma.
2.  En az bir bilgisayarı sınama grubuna taşıma.

**Sınama grubu oluşturmak için**
1.  WSUS Yönetim Konsolu'nda, **Bilgisayarlar**'ı genişletin ve **Tüm Bilgisayarlar**'ı seçin.

2.  **Tüm Bilgisayarlar**'ı sağ tıklatıp **Bilgisayar Grubu Ekle**'yi tıklatın.

3.  **Bilgisayar Grubu Ekle** iletişim kutusunda, yeni sınama grubunun **Ad** öğesini belirtin ve **Ekle**'yi tıklatın.

Sonraki yordamda, bir istemci bilgisayarı sınama grubuna atayacaksınız. Sınama bilgisayarı, ağdaki istemci bilgisayarların çoğunluğuyla tutarlı yazılım ve donanıma sahip olup henüz kendisine kritik bir rol atanmamış olan herhangi bir bilgisayardır. Sınamalarınız başarılı olduktan sonra, istediğiniz gruplarda bilgisayarların güncelleştirmelerini onaylayabilirsiniz.

**Sınama grubuna bilgisayar atamak için**
1.  WSUS Yönetim Konsolu'nda, **Bilgisayarlar**'ı tıklatın.

2.  Sınama grubuna atamak istediğiniz bilgisayar grubunu tıklatın.

3.  Bilgisayarlar listesinde, sınama grubuna atamak istediğiniz bilgisayarı veya bilgisayarları seçin.

4.  **Üyeliği Değiştir**'i sağ tıklatın.

5.  **Bilgisayar Grup Üyeliğini Ayarla** iletişim kutusunda, önceden oluşturduğunuz sınama grubunu seçin ve **Tamam**'ı tıklatın.

Sitenizde güncelleştirmeleri yönetmek için gerekli sayıda ek bilgisayar grupları oluşturmak üzere bu iki yordamı yineleyin, yani bir grup oluşturun ve sonra bilgisayarları bu gruba atayın.

Sonraki adım
------------

[Adım 7: WSUS Güncelleştirmelerini Onaylama ve Dağıtma](https://technet.microsoft.com/c4e58e17-d5e3-4194-8f26-b459e0c03b86).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
