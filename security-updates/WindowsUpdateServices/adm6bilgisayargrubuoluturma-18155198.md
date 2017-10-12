---
TOCTitle: 'Adım 6: Bilgisayar Grubu Oluşturma'
Title: 'Adım 6: Bilgisayar Grubu Oluşturma'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18155198
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720536(v=WS.10)'
---

Adım 6: Bilgisayar Grubu Oluşturma
==================================

Bilgisayar grupları, söz konusu olan bir temel dağıtım olsa bile WSUS dağıtımlarının önemli bir bölümüdür. Bilgisayar grupları, güncelleştirmeleri belirli bilgisayarlara yönlendirmenizi sağlar. İki varsayılan bilgisayar grubu vardır: Tüm Bilgisayarlar ve Atanmamış Bilgisayarlar. Varsayılan olarak her istemci bilgisayar başlangıçta WSUS sunucusuyla iletişim kurar; sunucu, bilgisayarı bu iki gruba da ekler.

Özel bilgisayar grupları oluşturabilirsiniz. Bilgisayar grupları oluşturmanın yararlarından biri, tamamen dağıtmadan önce güncelleştirmeleri sınamanıza olanak sağlamasıdır. Sınama düzgün giderse, güncelleştirmeleri Tüm Bilgisayarlar grubuna dağıtabilirsiniz. Oluşturabileceğiniz özel grupların sayısı için sınırlama yoktur.

Bilgisayar grupları ayarlama üç adımlı bir işlemdir. Önce bilgisayarları, bilgisayar gruplarına nasıl atayacağınızı belirlersiniz. İki seçenek vardır: *sunucu tarafında hedef belirleme* ve *istemci tarafında hedef belirleme*. Sunucu tarafında hedef belirleme, WSUS kullanarak her bilgisayarı grubuna el ile eklemeyi içerir. İstemci tarafında hedef belirleme, Grup İlkesi veya kayıt defteri anahtarları kullanarak istemcileri otomatik olarak eklemeyi içerir. İkinci olarak, bilgisayar grubunu WSUS üzerinde oluşturursunuz. Son olarak, ilk adımda seçtiğiniz yöntemi kullanarak bilgisayarları gruplara taşırsınız.

Bu inceleme, sunucu tarafında hedef belirlemenin nasıl kullanılacağını ve WSUS konsolu kullanarak bilgisayarları gruplarına taşımayı açıklar. Bilgisayar gruplarına atanacak çok sayıda istemci bilgisayarınız varsa, bilgisayarları bilgisayar gruplarına taşımayı otomatik olarak yapan istemci tarafında hedef belirlemeyi kullanabilirsiniz.

En az bir sınama bilgisayarı içeren bir test grubu ayarlamak için Adım 6'yı kullanabilirsiniz.

Bu adım aşağıdaki yordamları içerir:

-   Sunucu tarafında hedef belirleme.
-   Grup oluşturma.
-   Bilgisayarları gruba taşıma.

**Bilgisayarları gruplara atamak üzere yöntem belirlemek için**
1.  WSUS konsolu araç çubuğunda **Seçenekler**'i, sonra **Bilgisayar Seçenekleri**'ni tıklatın.

2.  **Bilgisayar Seçenekleri** kutusunda, **Windows Server Update Services'taki Bilgisayarları taşıma görevini kullan**'ı tıklatın.

3.  **Görevler**'in altında **Ayarları kaydet**'i tıklatın, onaylama iletişim kutusu görüntülendiğinde **Tamam**'ı tıklatın.

**Grup oluşturmak için**
1.  WSUS konsolu araç çubuğunda, **Bilgisayarlar**’ı tıklatın.

2.  **Görevler**'in altında **Bilgisayar grubu oluştur**'u tıklatın.

3.  **Bilgisayar Adı** kutusuna **Test** yazın ve **Tamam**’ı tıklatın.

Sınamaya uygun istemci bilgisayarı test grubuna atamak için izleyen yordamı kullanın. Sınamaya uygun istemci bilgisayar, ağınızdaki bilgisayarların büyük çoğunluğunda bulunan yazılım ve donanıma sahip, ancak önemli bir rol üstlenmemiş herhangi bir bilgisayardır. Böylece, sınama bilgisayarıyla karşılaştırarak, onayladığınız güncelleştirmelerin bilgisayarlarla uyumunun nasıl olacağını belirleyebilirsiniz.

**Test grubuna bilgisayarı el ile eklemek için**
1.  WSUS konsolu araç çubuğunda, **Bilgisayarlar**’ı tıklatın.

2.  **Gruplar** kutusunda, taşımak istediğiniz bilgisayar grubunu tıklatın.

3.  Bilgisayar listesinde, taşımak istediğiniz bilgisayarı tıklatın.

4.  **Görevler**'in altında **Seçili bilgisayarları taşı**'yı tıklatın.

5.  **Bilgisayar grubu** listesinde, bilgisayarı taşımak istediğiniz grubu seçin ve **Tamam**'ı tıklatın.
