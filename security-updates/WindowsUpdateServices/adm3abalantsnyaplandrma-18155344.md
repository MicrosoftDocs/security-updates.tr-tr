---
TOCTitle: 'Adım 3: Ağ Bağlantısını Yapılandırma'
Title: 'Adım 3: Ağ Bağlantısını Yapılandırma'
ms:assetid: 'cd77566d-7780-4ce4-aa56-41183c65c4a7'
ms:contentKeyID: 18155344
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708559(v=WS.10)'
---

Adım 3: Ağ Bağlantısını Yapılandırma
====================================

WSUS'yi yükledikten sonra WSUS'yi yapılandırmak ve kullanmaya başlamak için WSUS konsoluna erişmeye hazırsınız. Varsayılan olarak WSUS, güncelleştirmeleri almak için Microsoft Update'i kullanmak üzere yapılandırılmıştır. Ağınızda proxy sunucu varsa, WSUS'yi proxy sunucuyu kullanmak üzere yapılandırmak için WSUS konsolunu kullanın. WSUS ve Internet arasında kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir.

| ![](/security-updates/images/Cc708559.note(WS.10).gif)Not                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft Update'ten güncelleştirmeleri yüklemek için Internet bağlantınızın olması gerekir; bununla birlikte WSUS, Internet'e bağlı olmayan ağlara güncelleştirmeleri alma olanağı sunar. Daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir). |

Adım 3'te aşağıdaki yordamlar vardır:

-   WSUS'nin güncelleştirmeleri alabilmesi için güvenlik duvarını yapılandırma.
-   WSUS konsolunu açma.
-   WSUS'nin güncelleştirmeleri alabilmesi için proxy sunucu ayarlarını yapılandırma.

**Güvenlik duvarınızı yapılandırmak için**
-   WSUS ve Internet arasında kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir. WSUS sunucusu Microsoft Update'ten güncelleştirmeleri almak üzere, HTTP protokolü için 80 no'lu bağlantı noktasını, HTTPS protokolü için de 443 no'lu bağlantı noktasını kullanır. Bu, yapılandırılamaz.

-   Kuruluşunuz tüm adresler için bu bağlantı noktalarının ve protokollerin açık olmasına izin vermiyorsa, WSUS'nin ve Otomatik Güncelleştirmeler'in Microsoft Update ile iletişim kurabilmesi amacıyla erişimi yalnızca aşağıdaki etki alanlarıyla sınırlayabilirsiniz:

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

| ![](/security-updates/images/Cc708559.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Yukarıdaki güvenlik duvarını yapılandırma adımları, WSUS ve Internet arasında yer alan kurumsal güvenlik duvarı içindir. WSUS kendi ağ trafiğinin tümünü başlattığından, WSUS sunucusu üzerindeki Windows Güvenlik Duvarı'nı yapılandırmaya gerek yoktur. Microsoft Update ve WSUS arasındaki bağlantının 80 ve 443 no'lu bağlantı noktalarının açık olmasını gerektirmesine rağmen, özel bir bağlantı noktasıyla eşitlenmek üzere birden çok WSUS sunucusu yapılandırabilirsiniz. WSUS sunucularını özel bir bağlantı noktasıyla eşitleme hakkında daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir). |

**WSUS konsolunu açmak için**
-   WSUS sunucunuzda **Başlat**'ı tıklatıp **Tüm Programlar**'ın ve sonra **Yönetimsel Araçlar**'ın üzerine gelin ve **Microsoft Windows Server Update Services**'ı tıklatın.

| ![](/security-updates/images/Cc708559.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| WSUS konsolunu kullanabilmeniz için WSUS'nin yüklendiği sunucuda, WSUS Administrators veya yerel Administrators güvenlik gruplarından birinin üyesi olmanız gerekir.**http://&lt;***WSUS Web sitesi adını***&gt;**, Windows Server 2003'te Internet Explorer'ın Yerel Intranet bölgesindeki siteler listesine eklemezseniz, WSUS konsolunu her açtığınızda sizden kimlik bilgileri istenebilir. WSUS'yi yükledikten sonra IIS'de bağlantı noktası atamasını değiştirdiyseniz, **Başlat** menüsündeki kısayolu el ile güncelleştirmeniz gerekir. Ağınızdaki herhangi bir bilgisayar veya sunucuda aşağıdaki URL'yi girerek WSUS konsolunu Internet Explorer'dan da açabilirsiniz: **http://***WSUSsunucuadı***/WSUSAdmin** |

**Proxy sunucu belirlemek için**
1.  WSUS konsolu araç çubuğunda **Seçenekler**'i, sonra da **Eşitleme Seçenekleri**'ni tıklatın.

2.  **Proxy sunucu** kutusunda **Eşitleme işleminde proxy sunucu kullan** onay kutusunu işaretleyin ve ilgili kutulara proxy sunucu adını ve bağlantı noktası numarasını (varsayılan olarak 80 no'lu bağlantı noktası) yazın.

3.  Özel kullanıcı kimlik bilgileri kullanarak proxy sunucuya bağlanmak istiyorsanız, **Proxy sunucuya bağlanmak için kullanıcı kimlik bilgilerini kullan** onay kutusunu işaretleyin ve ilgili kutulara kullanıcı adını, etki alanını ve kullanıcının parolasını yazın. Proxy sunucuya bağlanan kullanıcı için temel kimlik doğrulamasını etkinleştirmek istiyorsanız, **Temel kimlik doğrulamasına izin ver (parola şifresiz metin ile gönderilir)** onay kutusunu işaretleyin.

4.  **Görevler**'in altında **Ayarları kaydet**'i tıklatın, onaylama iletişim kutusunda **Tamam**'ı tıklatın.
