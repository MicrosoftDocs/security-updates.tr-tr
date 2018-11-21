---
TOCTitle: 'Adım 6: Güncelleştirmeler için Bilgisayar Grubu Oluşturma'
Title: 'Adım 6: Güncelleştirmeler için Bilgisayar Grubu Oluşturma'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18155378
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708629(v=WS.10)'
---

Adım 6: Güncelleştirmeler için Bilgisayar Grubu Oluşturma
=========================================================

Bilgisayar grupları, söz konusu olan bir temel dağıtım olsa bile WSUS dağıtımlarının önemli bir bölümüdür. Bilgisayar grupları, güncelleştirmeleri belirli bilgisayarlara yönlendirmenizi sağlar. İki varsayılan bilgisayar grubu vardır: Tüm Bilgisayarlar ve Atanmamış Bilgisayarlar. Varsayılan olarak, her istemci bilgisayar WSUS sunucusuyla ilk kez iletişim kurduğunda, sunucu istemci bilgisayarı bu iki gruba da ekler.

Özel bilgisayar grupları oluşturabilirsiniz. Bilgisayar grupları oluşturmanın yararlarından biri, güncelleştirmeleri tamamen dağıtmadan önce sınamanıza olanak sağlamasıdır. Sınama sorunsuz tamamlanırsa, güncelleştirmeleri Tüm Bilgisayarlar grubuna dağıtabilirsiniz. Oluşturabileceğiniz özel grupların sayısı için sınırlama yoktur.

**Bilgisayar gruplarını ayarlamak için**
1.  Bilgisayarları bilgisayar gruplarına nasıl atayacağınızı belirtin. İki seçenek vardır: sunucu tarafında hedef belirleme ve istemci tarafında hedef belirleme. Sunucu tarafında hedef belirleme, WSUS kullanarak her bilgisayarı grubuna el ile eklemeyi içerir. İstemci tarafında hedef belirleme, Grup İlkesi veya kayıt defteri anahtarları kullanarak istemcileri otomatik olarak eklemeyi içerir.

2.  Bilgisayar grubunu WSUS üzerinde oluşturun.

3.  1. adımda seçtiğiniz yöntemi kullanarak bilgisayarları gruplara taşıyın.

Bu bölümde, sunucu tarafında hedef belirlemenin nasıl kullanılacağı ve WSUS Yönetimi konsolu kullanılarak bilgisayarların el ile gruplarına taşınması anlatılmaktadır. Bilgisayar gruplarına atanacak birden fazla istemci bilgisayarınız varsa, bilgisayarları bilgisayar gruplarına taşımayı otomatikleştiren istemci tarafında hedef belirleme yöntemini kullanabilirsiniz.

En az bir sınama bilgisayarı içeren bir test grubu ayarlamak için Adım 6'yı kullanabilirsiniz.

**Adım 6 aşağıdaki yordamları içerir:**

-   Grup oluşturma.
-   Gruba bilgisayar ekleme.

**Grup oluşturmak için**
1.  WSUS Yönetimi konsolunda, **Bilgisayarlar**'ı genişletin ve **Tüm Bilgisayarlar**'ı seçin

2.  **Tüm Bilgisayarlar**'ı sağ tıklatın veya **Eylemler** bölmesine gidin ve sonra **Bilgisayar Grubu Ekle**'yi tıklatın.

3.  **Bilgisayar Grubu Ekle** iletişim kutusunu görürsünüz. Yeni grubun adını belirtin.

Bir istemci bilgisayarı sınama grubuna atamak için izleyen yordamı kullanın. Sınamaya uygun istemci bilgisayar, ağınızdaki bilgisayarların büyük çoğunluğunda bulunan yazılım ve donanıma sahip, ancak önemli bir rol üstlenmemiş herhangi bir bilgisayardır. Böylece, sınama bilgisayarına benzer bilgisayarların onayladığınız güncelleştirmeler uyumunun nasıl olacağını belirleyebilirsiniz.

**Gruba bilgisayar eklemek için**
1.  WSUS Yönetimi konsolunda, **Bilgisayarlar**'ı tıklatın.

2.  Taşımak istediğiniz bilgisayarı grubunu tıklatın.

3.  Bilgisayar listesinde, taşımak istediğiniz bilgisayarı seçin.

4.  **Üyeliği Değiştir**'i sağ tıklatın.

5.  Bir grup listesi içeren **Bilgisayar Grup Üyeliğini Ayarla** iletişim kutusunu görürsünüz.

6.  Bilgisayarı taşımak istediğiniz grubu işaretleyin ve sonra **Tamam**'ı tıklatın.
