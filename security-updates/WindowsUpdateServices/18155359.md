---
TOCTitle: 'Adım 3: WSUS 3.0 için Ağ Bağlantısını Yapılandırma'
Title: 'Adım 3: WSUS 3.0 için Ağ Bağlantısını Yapılandırma'
ms:assetid: 'dbc9d9f7-cf52-4539-9f9e-3e823273218a'
ms:contentKeyID: 18155359
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708602(v=WS.10)'
---

Adım 3: WSUS 3.0 için Ağ Bağlantısını Yapılandırma
==================================================

WSUS 3.0 yüklendikten sonra, yapılandırma sihirbazı otomatik olarak başlatılır. Sonradan, WSUS 3.0 konsolunun **Seçenekler** sayfasından da çalıştırabilirsiniz.

Yapılandırma işlemine başlamadan önce, aşağıdaki soruların yanıtlarını bildiğinizden emin olun:

1. Sunucunun güvenlik duvarı istemcilerin sunucuya erişmesine izin verecek şekilde yapılandırılmış mı?

2. Bu bilgisayar akış yukarı sunucuya (Microsoft Update gibi) bağlanabiliyor mu?

3. Gerekiyorsa, proxy sunucunun adını ve proxy sunucuyla ilgili kullanıcı kimlik bilgilerini edindiniz mi?

Varsayılan olarak WSUS, güncelleştirmeleri almak için Microsoft Update'i kullanmak üzere yapılandırılmıştır. Ağınızda proxy sunucu varsa, WSUS'yi proxy sunucuyu kullanmak üzere yapılandırabilirsiniz. WSUS ve Internet arasında kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir.

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Not                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft Update'ten güncelleştirmeleri yüklemek için Internet bağlantınızın olması gerekir; bununla birlikte WSUS, Internet'e bağlı olmayan ağlara güncelleştirmeleri alma olanağı sunar. |

**Adım 3 aşağıdaki yordamları içerir**

-   Güvenlik duvarını yapılandırma.
-   Bu sunucunun güncelleştirmeleri alma yöntemini belirtme (Microsoft Update'ten ya da başka bir WSUS sunucusundan).
-   WSUS'nin güncelleştirmeleri alabilmesi için proxy sunucu ayarlarını yapılandırma.

**Güvenlik duvarınızı yapılandırmak için**
-   WSUS ile Internet arasında bir kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir. WSUS sunucusu Microsoft Update'ten güncelleştirmeleri almak üzere, HTTP protokolü için 80 numaralı bağlantı noktasını, HTTPS protokolü için de 443 numaralı bağlantı noktasını kullanır. Bu, yapılandırılamaz.

-   Kuruluşunuz 80 ve 443 numaralı bağlantı noktalarının tüm adreslere açık olmasına izin vermiyorsa, WSUS'nin ve Otomatik Güncelleştirmeler'in Microsoft Update ile iletişim kurabilmesi amacıyla erişimi yalnızca aşağıdaki etki alanlarıyla sınırlayabilirsiniz:

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

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Not                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Güvenlik duvarını yapılandırmayla ilgili bu yönergeler, WSUS ile Internet arasında yer alan kurumsal güvenlik duvarı içindir. WSUS kendi ağ trafiğinin tümünü başlattığından, WSUS sunucusu üzerinde Windows Güvenlik Duvarı'nı yapılandırmaya gerek yoktur. |

Microsoft Update ve WSUS arasındaki bağlantının 80 ve 443 numaralı bağlantı noktalarının açık olmasını gerektirmesine rağmen, özel bir bağlantı noktasıyla eşitlenmek üzere birden fazla WSUS sunucusu yapılandırabilirsiniz.

Sıradaki iki yordam yapılandırma sihirbazını kullandığınızı kabul etmektedir. Bu adımın ilerideki bir bölümünde, WSUS Yönetimi ek bileşenini başlatmayı ve sunucuyu **Seçenekler** sayfasını kullanarak yapılandırmayı öğreneceksiniz.

**Bu sunucunun güncelleştirmeleri alma yöntemini belirtmek için**
1.  Yapılandırma sihirbazından, Microsoft Geliştirme Programı'na katıldıktan sonra, akış yukarı sunucuyu seçmek için **İleri**'yi tıklatın.

2.  Microsoft Update'ten eşitlemeyi seçerseniz, bu sayfada yapacağınız işlemler bitmiştir. **İleri**'yi tıklatın veya sol bölmede **Proxy Sunucuyu Belirt**'i seçin.

3.  Başka bir WSUS sunucusundan eşitlemeyi seçerseniz, bu sunucunun akış yukarı sunucu ile iletişim kurarken kullanacağı bağlantı noktasını ve sunucu adını belirtin.

4.  SSL kullanmak için, **Güncelleştirme bilgilerini eşitlerken SSL kullan** onay kutusunu işaretleyin. Bu durumda sunucular eşitleme için 443 numaralı bağlantı noktasını kullanır. (Hem bu sunucunun, hem de akış yukarı sunucunun SSL'yi desteklediğinden emin olmalısınız).

5.  Bu sunucu bir çoğaltma sunucuysa, **Bu sunucu akış yukarı sunucunun bir çoğaltmasıdır** onay kutusunu işaretleyin.

6.  Bu noktada akış yukarı sunucu yapılandırmasını tamamlamış olursunuz. **İleri**'yi tıklatın veya sol bölmede **Proxy Sunucuyu Belirt**'i seçin.

**Proxy sunucu ayarlarını yapılandırmak için**
1.  Yapılandırma sihirbazının **Proxy Sunucuyu Belirt** sayfasında, **Eşitleme yaparken proxy sunucu kullan** onay kutusunu seçin ve sonra ilgili kutulara proxy sunucu adını ve bağlantı noktası numarasını (varsayılan olarak 80 numaralı bağlantı noktası) yazın.

2.  Özel kullanıcı kimlik bilgileri kullanarak proxy sunucuya bağlanmak istiyorsanız, **Proxy sunucuya bağlanmak için kullanıcı kimlik bilgilerini kullan** onay kutusunu işaretleyin ve ilgili kutulara kullanıcı adını, etki alanını ve kullanıcının parolasını yazın. Proxy sunucuya bağlanan kullanıcı için temel kimlik doğrulamasını etkinleştirmek istiyorsanız, **Basit kimlik doğrulamaya izin ver (parola düz metin olarak gönderilir)** onay kutusunu seçin.

3.  Bu noktada proxy sunucu yapılandırmasını tamamlamış olursunuz. Eşitleme işlemini ayarlamaya başlayabileceğiniz sonraki sayfaya gitmek için **İleri**'yi tıklatın.

Aşağıdaki iki yordamda yapılandırma için WSUS Yönetimi ek bileşenini kullandığınız kabul edilir. Bu iki yordamda, WSUS Yönetimi ek bileşenini nasıl başlatacağınız ve **Seçenekler** sayfasını kullanarak sunucuyu nasıl yapılandıracağınız gösterilir.

**WSUS Yönetimi konsolunu başlatmak için**
-   WSUS Yönetimi konsolunu başlatmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gidin, **Yönetimsel Araçlar**'ın üzerine gidin ve sonra **Microsoft Windows Server Update Services 3.0**'ı tıklatın.

| ![](/security-updates/images/Cc708602.note(WS.10).gif)Not                                                                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| WSUS konsolunun tüm özelliklerini kullanabilmeniz için, WSUS'nin yüklendiği sunucuda WSUS Administrators WSUS'nin yüklendiği sunucuda ya da yerel Administrators üyesi olmanız gerekir. Ancak, WSUS Reporters güvenlik grubunun üyeleri yönetim konsolunda salt okuma erişimine sahiptir. |

**Güncelleştirme kaynağı ve proxy sunucu belirtmek için**
1.  WSUS konsolunda, sol bölmede bu sunucunun adının altında **Seçenekler**'i tıklatın ve sonra orta panelde **Güncelleştirme Kaynağı ve Proxy Sunucu**'yu tıklatın.

2.  **Güncelleştirme Kaynağı** ve **Proxy Sunucusu** sekmeleri bulunan bir iletişim kutusu görüntülenir.

3.  **Güncelleştirme Kaynağı** sekmesinde, sunucunun güncelleştirmeleri alacağı konumu seçin. Microsoft Update'ten eşitlemeyi (varsayılan) seçerseniz, bu sihirbaz sayfasında yapacağınız işlemler bitmiştir.

4.  Başka bir WSUS sunucusundan eşitlemeyi seçerseniz, sunucuların iletişim kurmak için kullanacağı bağlantı noktasını belirtmeniz gerekir (varsayılan bağlantı noktası 80'dir). Farklı bir bağlantı noktası seçerseniz, her iki sunucunun da seçtiğiniz bağlantı noktasını kullanabildiğinden emin olmalısınız.

5.  Akış yukarı WSUS sunucusundan eşitleme yaparken SSL kullanılıp kullanılmayacağını da belirtebilirsiniz. Bu durumda, sunucular akış yukarı sunucudan eşitleme yapmak için 443 numaralı bağlantı noktasını kullanırlar.

6.  Bu sunucu diğer WSUS sunucusunun çoğaltmasıysa, **Bu sunucu akış yukarı sunucunun bir çoğaltmasıdır** onay kutusunu seçin. Bu durumda, tüm güncelleştirmelerin yalnızca akış yukarı WSUS sunucusunda onaylanması gerekir.

7.  **Proxy Sunucu** sekmesinde, **Eşitleme işleminde proxy sunucu kullan** onay kutusunu işaretleyin ve ilgili kutulara proxy sunucu adını ve bağlantı noktası numarasını (varsayılan olarak 80 numaralı bağlantı noktası) yazın.

8.  Özel kullanıcı kimlik bilgileri kullanarak proxy sunucuya bağlanmak istiyorsanız, **Proxy sunucuya bağlanmak için kullanıcı kimlik bilgilerini kullan** onay kutusunu işaretleyin ve ilgili kutulara kullanıcı adını, etki alanını ve kullanıcının parolasını yazın. Proxy sunucuya bağlanan kullanıcı için temel kimlik doğrulamasını etkinleştirmek istiyorsanız, **Temel kimlik doğrulamasına izin ver (parola şifresiz metin ile gönderilir)** onay kutusunu işaretleyin.

9.  **Tamam**'ı tıklatarak bu ayarları kaydedin.
