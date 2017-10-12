---
TOCTitle: 'Adım 5: Otomatik Güncelleştirmeleri Güncelleştirme ve Yapılandırma'
Title: 'Adım 5: Otomatik Güncelleştirmeleri Güncelleştirme ve Yapılandırma'
ms:assetid: '4ac8d574-f48e-4d9d-86c9-9aeb0f57e750'
ms:contentKeyID: 18155025
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720533(v=WS.10)'
---

Adım 5: Otomatik Güncelleştirmeleri Güncelleştirme ve Yapılandırma
==================================================================

WSUS istemci bilgisayarları Otomatik Güncelleştirmeler'in uyumlu bir sürümünü gerektirir. WSUS Kurulumu, WSUS sunucusuyla iletişime geçen her istemci bilgisayarına Otomatik Güncelleştirmeler'in en son sürümünü dağıtmak üzere IIS'yi otomatik olarak yapılandırır.

| ![](images/Cc720533.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Otomatik Güncelleştirmeler'in birçok sürümü WSUS sunucusuna işaret edecek şekilde ayarlanabilir ve kendisini otomatik olarak WSUS uyumlu sürüme güncelleştirebilir, ancak hizmet paketi içermeyen bir Windows XP işletim sisteminde bulunan Otomatik Güncelleştirmeler sürümü kendisini otomatik olarak güncelleştiremez. Ortamınızda hizmet paketi içermeyen Windows XP kullanıyorsanız ve Software Update Services (SUS) uygulamasını hiç kullanmadıysanız, yönergeler için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir). |

Otomatik Güncelleştirmeler'e yönelik en iyi yapılandırma yöntemi ağ ortamınıza bağlıdır. Active Directory ortamında, Active Directory tabanlı Grup İlkesi nesnesi (GPO) kullanabilirsiniz. Active Directory dışı bir ortamda Yerel Grup İlkesi nesnesini kullanın. Yerel Grup İlkesi nesnesini veya etki alanı denetleyicisinde depolanan bir GPO'yu kullanmanızdan bağımsız olarak, istemci bilgisayarlarınızı WSUS sunucusunu işaret edecek şekilde ayarlamalı ve ardından Otomatik Güncelleştirmeler'i yapılandırmalısınız.

Aşağıdaki yönergeler ağınızda Active Directory çalıştırıldığını varsayar. Bu yordamlar aynı zamanda, önceden Grup İlkesi ayarladığınızı, bunu nasıl kullanacağınızı bildiğinizi ve ağınızı yönetmek için Grup İlkesi kullandığınızı da varsayar. WSUS ayarları için yeni Grup İlkesi nesnesi (GPO) oluşturmalı ve GPO'yu etki alanı düzeyinde bağlamalısınız.

Grup İlkesi hakkında daha fazla bilgi için http://go.microsoft.com/fwlink/?LinkID=47375 adresindeki [Grup İlkesi](http://go.microsoft.com/fwlink/?linkid=47375) sayfasına bakın.

Adım 5'te aşağıdaki yordamlar vardır:

-   WSUS Yönetimsel Şablonunu yükleme.
-   Otomatik Güncelleştirmeler'i yapılandırma.
-   İstemci bilgisayarları WSUS sunucusunu işaret edecek şekilde ayarlama.
-   İstemci bilgisayarda algılamayı el ile başlatma.

İzleyen üç yordamı Active Directory tabanlı Grup İlkesi nesnesinde gerçekleştirin.

**WSUS Yönetimsel Şablonunu eklemek için**
1.  Grup İlkesi Nesne Düzenleyicisi'nde, **Yönetim Şablonları** düğümlerinden birini tıklatın.

2.  **Eylem** menüsünde **Şablon Ekle/Kaldır**'ı tıklatın.

3.  **Ekle**'yi tıklatın.

4.  **İlke Şablonları** iletişim kutusunda **wuau.adm** öğesini tıklattıktan sonra **Aç**'ı tıklatın.

5.  **Şablon Ekle/Kaldır** iletişim kutusunda **Kapat**’ı tıklatın.

**Otomatik Güncelleştirmeler'in davranışını yapılandırmak için**
1.  Grup İlkesi Nesne Düzenleyicisi'nde sırasıyla **Bilgisayar Yapılandırma**, **Yönetim Şablonları** ve **Windows Bileşenleri**'ni genişletin ve **Windows Update**'i tıklatın.

2.  Ayrıntılar bölmesinde **Otomatik Güncelleştirmeleri Yapılandır**’ı çift tıklatın.

3.  **Etkin**’i tıklatın ve sonra aşağıdaki seçeneklerden birini tıklatın:

    -   **Karşıdan yükleme ve kurma için uyar.** Bu seçenek, yönetici olarak oturum açmış kullanıcıyı güncelleştirmeleri karşıdan yüklemeden ve kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurma için uyar.** Bu seçenek güncelleştirmelerin karşıdan yüklenmesini otomatik olarak başlatır ve yönetici olarak oturum açmış kullanıcıyı güncelleştirmeleri kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurmayı zamanla.** Otomatik Güncelleştirmeler zamanlanmış kurulum yapmak üzere yapılandırılmışsa, yinelenen zamanlanmış kurulumlar için gün ve saat de ayarlamalısınız.
    -   **Yerel yöneticinin ayarı seçmesine izin ver.** Bu seçenekle, yerel yöneticilerin istedikleri yapılandırma seçeneklerini belirlemek üzere Denetim Masası'ndaki Otomatik Güncelleştirmeler'i kullanmasına olanak sağlanır. Örneğin, kendi zamanlanmış yükleme saatlerini seçebilirler. Yerel yöneticilerin Otomatik Güncelleştirmeler'i devre dışı bırakmasına izin verilmez.

4.  **Tamam**'ı tıklatın.

| ![](images/Cc720533.note(WS.10).gif)Not                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Yerel yöneticinin ayarı seçmesine izin ver** ayarı yalnızca, Otomatik Güncelleştirmeler kendisini WSUS ile uyumlu sürüme güncelleştirmişse görüntülenir. |

**İstemci bilgisayarı WSUS sunucusunu işaret edecek şekilde ayarlama**
1.  Grup İlkesi Nesne Düzenleyicisi'nde sırasıyla **Bilgisayar Yapılandırma**, **Yönetim Şablonları** ve **Windows Bileşenleri**'ni genişletin ve **Windows Update**'i tıklatın.

2.  Ayrıntılar bölmesinde **Intranet Microsoft güncelleştirme hizmeti konumunu belirt**’i çift tıklatın.

3.  **Etkin**'i tıklatın ve **Güncelleştirmeleri algılamak için intranet güncelleştirme hizmetini ayarla** kutusunda ve **Intranet istatistik sunucusunu ayarla** kutusunda aynı WSUS sunucusunun HTTP URL'sini yazın. Örneğin, her iki kutuya da **http://***sunucuadı* yazın.

4.  **Tamam**'ı tıklatın.

| ![](images/Cc720533.note(WS.10).gif)Not                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu bilgisayarı WSUS'yi işaret edecek şekilde ayarlamak için Yerel Grup İlkesi nesnesini kullanıyorsanız, bu ayar hemen etkin olur ve bu bilgisayar yaklaşık 20 dakika içinde WSUS yönetici konsolunda görüntülenir. Algılama döngüsünü el ile başlatarak bu işlemi hızlandırabilirsiniz. |

İstemci bilgisayar yapılandırıldıktan sonra, WSUS konsolundaki **Bilgisayarlar** sayfasında görüntülenmesi birkaç dakika sürer. Active Directory tabanlı GPO ile yapılandırılmış istemci bilgisayarlar için bu süre, Grup İlkesi yenilendikten sonra yaklaşık 20 dakikadır (bu, istemci bilgisayardaki tüm yeni ayarlar için geçerlidir). Varsayılan olarak Grup İlkesi, arka planda 0 ile 30 dakikalık rasgele aralıklarla her 90 dakikada bir yenilenir. Grup İlkesi'nin daha hızlı yenilenmesini istiyorsanız, istemci bilgisayarda komut istemine gidebilir ve aşağıdakini yazabilirsiniz: **gpupdate /force**.

Yerel GPO ile yapılandırılmış istemci bilgisayarlar için, Grup İlkesi hemen uygulanır ve bu işlem yaklaşık 20 dakika sürer.

Grup İlkesi uygulandıktan sonra algılamayı el ile başlatabilirsiniz. Bu adımı gerçekleştirirseniz, istemci bilgisayarın WSUS ile iletişim kurması için 20 dakika beklemeniz gerekmez.

**WSUS sunucusunun algılanmasını el ile başlatmak için**
1.  İstemci bilgisayarda **Başlat**’ı ve **Çalıştır**’ı tıklatın.

2.  **cmd** yazın ve **Tamam**'ı tıklatın.

3.  Komut isteminde **wuauclt.exe /detectnow** yazın. Bu komut satırı seçeneği Otomatik Güncelleştirmeler'in WSUS sunucusuyla hemen iletişim kurmasını sağlar.
