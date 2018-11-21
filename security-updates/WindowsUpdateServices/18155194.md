---
TOCTitle: 'Adım 5: Otomatik Güncelleştirmeleri Yapılandırma'
Title: 'Adım 5: Otomatik Güncelleştirmeleri Yapılandırma'
ms:assetid: '5da6d10a-6ff1-4de8-b53a-4893bf8bd9fa'
ms:contentKeyID: 18155194
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720532(v=WS.10)'
---

Adım 5: Otomatik Güncelleştirmeleri Yapılandırma
================================================

WSUS istemci bilgisayarları Otomatik Güncelleştirmeler'in uyumlu bir sürümünü gerektirir. WSUS Kurulumu, WSUS sunucusuyla iletişime geçen her istemci bilgisayarına Otomatik Güncelleştirmeler'in en son sürümünü dağıtmak üzere IIS'yi otomatik olarak yapılandırır.

Otomatik Güncelleştirmeler'i yapılandırmanın en iyi yöntemi ağ ortamınıza bağlıdır. Active Directory bulunan bir ortamda, etki alanı tabanlı bir Grup İlkesi nesnesi (GPO) kullanabilirsiniz. Active Directory bulunmayan bir ortamda, Yerel Grup İlkesi nesnesini kullanın. Yerel Grup İlkesi nesnesini veya etki alanı tabanlı bir GPO kullanmanızdan bağımsız olarak, istemci bilgisayarlarınızı WSUS sunucusunu işaret edecek şekilde ayarlamalı ve sonra Otomatik Güncelleştirmeler'i yapılandırmalısınız.

Aşağıdaki yönergeler ağınızda Active Directory çalıştırıldığını varsayar. Bu yordamlar, Grup İlkesi kullanmayı bildiğinizi ve ağınızı yönetmek için kullandığınızı da varsayar. WSUS ayarları için yeni GPO oluşturmanız ve GPO'yu etki alanına bağlamanız gerekir.

Grup İlkesi hakkında daha fazla bilgi için, Grup İlkesi Teknoloji Merkezi Web sitesine bakın ([http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375)).

**Adım 5 aşağıdaki yordamları içerir**

-   WSUS Yönetimsel Şablonunu ekleme.
-   Otomatik Güncelleştirmeler'i yapılandırma.
-   İstemci bilgisayarınızı WSUS sunucunuzu işaret edecek şekilde ayarlama.
-   WSUS sunucusu tarafından algılamayı el ile başlatma.

İlk üç yordamı etki alanı tabanlı bir Grup İlkesi nesnesinde gerçekleştirin. Yeni bir GPO oluşturmanız veya varolan bir GPO'yu kullanmanız gerekir. GPO'larınızı yönetmek için Grup İlkesi Yönetim Konsolu'nu (GPMC) kullanıyorsanız, değiştirmek istediğiniz GPO'ya gidin ve sonra **Düzenle**'yi tıklatın.

WSUS'yi yönetmek üzere ilke ayarlarını görüntülemek için, wuau.adm adlı WSUS yönetimsel şablon dosyasının Grup İlkesi Nesne Düzenleyicisi'ne eklendiğinden emin olmanız gerekir. wuau.adm dosyası varsayılan olarak işletim sisteminde yayımlandığından, Grup İlkesi Nesne Düzenleyicisi'nde zaten var olmalıdır.

**WSUS Yönetimsel Şablonunu eklemek için**
1.  Grup İlkesi Nesne Düzenleyicisi'nde, **Yönetim Şablonları** düğümlerinden birini tıklatın.

2.  **Eylem** menüsünde, **Şablon Ekle/Kaldır**'ı tıklatın ve sonra **Ekle**'yi tıklatın.

3.  **İlke Şablonları** iletişim kutusunda **wuau.adm** öğesini tıklatın ve sonra **Aç**'ı tıklatın.

4.  **Şablon Ekle/Kaldır** iletişim kutusunda **Kapat**'ı tıklatın.

**Otomatik Güncelleştirmeler'i yapılandırmak için**
1.  Grup İlkesi Nesne Düzenleyicisi'nde sırasıyla **Bilgisayar Yapılandırma**, **Yönetim Şablonları** ve **Windows Bileşenleri**'ni genişletin ve **Windows Update**'i tıklatın.

2.  Ayrıntılar bölmesinde **Otomatik Güncelleştirmeleri Yapılandır**'ı çift tıklatın.

3.  **Etkin**'i tıklatın ve sonra aşağıdaki seçeneklerden birini tıklatın:

    -   **Karşıdan yükleme ve kurma için uyar**: Bu seçenek, yönetici olarak oturum açmış olan kullanıcıyı karşıdan yükleme başlamadan ve güncelleştirmeleri kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurma için uyar**: Bu seçenek güncelleştirmelerin karşıdan yüklenmesini otomatik olarak başlatır ve yönetici olarak oturum açmış kullanıcıyı güncelleştirmeleri kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurmayı zamanla**: Otomatik Güncelleştirmeler zamanlanmış kurulum yapmak üzere yapılandırılmışsa, yinelenen zamanlanmış kurulumlar için gün ve saat de ayarlamalısınız.
    -   **Yerel yöneticinin ayarı seçmesine izin ver**: Bu seçenekle, yerel yöneticilerin istedikleri yapılandırma seçeneklerini belirlemek üzere Denetim Masası'ndaki Otomatik Güncelleştirmeler'i kullanmasına olanak sağlanır. Örneğin, kendi zamanlanmış yükleme saatlerini seçebilirler. Yerel yöneticilerin Otomatik Güncelleştirmeler'i devre dışı bırakmasına izin verilmez.

4.  **Tamam**'ı tıklatın.

| ![](/security-updates/images/Cc720532.note(WS.10).gif)Not                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Yerel yöneticinin ayarı seçmesine izin ver** ayarı yalnızca, Otomatik Güncelleştirmeler kendini WSUS ile uyumlu sürüme güncelleştirmişse görüntülenir. |

**İstemci bilgisayarınızı WSUS sunucunuzu işaret edecek şekilde ayarlamak için**
1.  Grup İlkesi Nesne Düzenleyicisi'nde sırasıyla **Bilgisayar Yapılandırma**, **Yönetim Şablonları** ve **Windows Bileşenleri**'ni genişletin ve **Windows Update**'i tıklatın.

2.  Ayrıntılar bölmesinde **İntranet Microsoft güncelleştirme hizmeti konumunu belirt**'i çift tıklatın.

3.  **Etkin**'i tıklatın ve **Güncelleştirmeleri algılamak için intranet güncelleştirme hizmetini ayarla** kutusunda ve **İntranet istatistik sunucusunu ayarla** kutusunda aynı WSUS sunucusunun HTTP URL'sini yazın. Örneğin, her iki kutuya da *http://sunucuadı* yazın ve sonra **Tamam**'ı tıklatın.

| ![](/security-updates/images/Cc720532.note(WS.10).gif)Not                                                                                                                                                                                                                 |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu bilgisayarı WSUS'yi işaret edecek şekilde ayarlamak için Yerel Grup İlkesi nesnesini kullanıyorsanız, bu ayar hemen etkin olur ve bu bilgisayar kısa bir süre sonra WSUS yönetici konsolunda görüntülenir. El ile bir algılama döngüsü başlatarak bu süreci hızlandırabilirsiniz. |

İstemci bilgisayar yapılandırıldıktan sonra, WSUS konsolundaki **Bilgisayarlar** sayfasında görüntülenmesi birkaç dakika sürer. Etki alanı tabanlı bir Grup İlkesi ile yapılandırılmış istemci bilgisayarlar için, Grup İlkesi yenilendikten sonra yaklaşık 20 dakika sürer (yani, tüm yeni ilke ayarlarını istemci bilgisayara uygular). Varsayılan olarak, Grup İlkesi arka planda 0 ile 30 dakikalık rasgele sapmalarla her 90 dakikada bir yenilenir. Grup İlkesi'nin daha hızlı yenilenmesini istiyorsanız, istemci bilgisayarda komut istemine gidebilir ve aşağıdakini yazabilirsiniz: **gpupdate /force**.

Yerel GPO ile yapılandırılmış istemci bilgisayarlar için, Grup İlkesi hemen uygulanır ve yenileme yaklaşık 20 dakika sürer.

Grup İlkesi uygulandıktan sonra algılamayı el ile başlatabilirsiniz. Algılamayı el ile başlatırsanız, istemci bilgisayarın WSUS ile iletişim kurması için 20 dakika beklemeniz gerekmez.

**WSUS sunucusunun algılamasını el ile başlatmak için**
1.  İstemci bilgisayarda, **Başlat**'ı ve sonra **Çalıştır**'ı tıklatın.

2.  **Aç** kutusuna **cmd** yazın ve sonra **Tamam**'ı tıklatın.

3.  Komut isteminde **wuauclt.exe /detectnow** yazın. Bu komut satırı seçeneği Otomatik Güncelleştirmeler'in WSUS sunucusuyla hemen iletişim kurmasını sağlar.
