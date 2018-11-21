---
TOCTitle: 'Adım 3: Ağ Bağlantılarını Yapılandırma'
Title: 'Adım 3: Ağ Bağlantılarını Yapılandırma'
ms:assetid: '42a144c5-f08e-4a6e-b360-47ddea77bd24'
ms:contentKeyID: 21799211
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939815(v=WS.10)'
---

Adım 3: Ağ Bağlantılarını Yapılandırma
======================================

Siz Windows Server Update Services 3.0 Service Pack 2'yi (WSUS 3.0 SP2) yükledikten sonra, yapılandırma sihirbazı otomatik olarak başlatılır. Sonradan, WSUS Yönetim Konsolu'nun **Seçenekler** sayfasından da sihirbazı çalıştırabilirsiniz.

Yapılandırma işlemine başlamadan önce, aşağıdaki soruların yanıtlarını bildiğinizden emin olun:

1. Sunucunun güvenlik duvarı istemcilerin sunucuya erişmesine izin verecek şekilde yapılandırılmış mı?

2. Bu bilgisayar akış yukarı sunucuya (Microsoft Update gibi) bağlanabiliyor mu?

3. Gerekiyorsa, proxy sunucunun adını ve proxy sunucuyla ilgili kullanıcı kimlik bilgilerini edindiniz mi?

Varsayılan olarak WSUS 3.0 SP2, güncelleştirmeleri almak için Microsoft Update'i kullanacak şekilde yapılandırılmıştır. Ağda proxy sunucu varsa, WSUS 3.0 SP2'yi proxy sunucuyu kullanacak şekilde yapılandırabilirsiniz. WSUS ve Internet arasında kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939815.note(WS.10).gif" />Not</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Update'ten güncelleştirmeleri yüklemek için Internet bağlantısı gerekir; bununla birlikte WSUS, Internet'e bağlı olmayan ağlara güncelleştirmeleri alma olanağı sunar.
</td>
</tr>
</tbody>
</table>
 

Adım 3 aşağıdaki yordamları içerir:

-   Güvenlik duvarını yapılandırma.
-   Bu sunucunun güncelleştirmeleri alma yöntemini belirtme (Microsoft Update'ten ya da başka bir WSUS sunucusundan).
-   WSUS'nin güncelleştirmeleri alabilmesi için proxy sunucu ayarlarını yapılandırma.

**Güvenlik duvarınızı yapılandırmak için**
-   WSUS ile Internet arasında bir kurumsal güvenlik duvarı varsa, WSUS'nin güncelleştirmeleri alabildiğinden emin olmak için güvenlik duvarını yapılandırmanız gerekebilir. WSUS sunucusu Microsoft Update'ten güncelleştirmeleri almak üzere, HTTP protokolü için 80 numaralı bağlantı noktasını, HTTPS protokolü için de 443 numaralı bağlantı noktasını kullanır. Bu, yapılandırılamaz.

-   Kuruluşunuz 80 veya 443 numaralı bağlantı noktalarının tüm adreslere açık olmasına izin vermiyorsa, WSUS'nin ve Otomatik Güncelleştirmeler'in Microsoft Update ile iletişim kurabilmesi için erişimi yalnızca aşağıdaki etki alanlarıyla sınırlayabilirsiniz:

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

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939815.note(WS.10).gif" />Not</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Güvenlik duvarını yapılandırmayla ilgili bu yönergeler, WSUS ile Internet arasında yer alan kurumsal güvenlik duvarı içindir. WSUS kendi ağ trafiğinin tümünü başlattığından, WSUS sunucusu üzerinde Windows Güvenlik Duvarı'nı yapılandırmanız gerekmez.
</td>
</tr>
</tbody>
</table>
 

Microsoft Update ve WSUS arasındaki bağlantının 80 ve 443 numaralı bağlantı noktalarının açık olmasını gerektirmesine rağmen, özel bir bağlantı noktasıyla eşitlenmek üzere birden fazla WSUS sunucusu yapılandırabilirsiniz.

Sıradaki iki yordam yapılandırma sihirbazını kullandığınızı kabul etmektedir. Bu adımın ilerideki bir bölümünde, WSUS Yönetimi ek bileşenini başlatmayı ve sunucuyu Seçenekler sayfasını kullanarak yapılandırmayı öğreneceksiniz.

**Bu sunucunun güncelleştirmeleri alma yöntemini belirtmek için**
1.  Yapılandırma sihirbazından, Microsoft Geliştirme Programı'na katıldıktan sonra, akış yukarı sunucuyu seçmek için **İleri**'yi tıklatın.

2.  Microsoft Update'ten eşitlemeyi seçerseniz, Seçenekler sayfasında yapacağınız işlemler bitmiştir. **İleri**'yi tıklatın veya gezinti bölmesinde **Proxy Sunucuyu Belirt**'i seçin.

3.  Başka bir WSUS sunucusundan eşitlemeyi seçerseniz, bu sunucunun akış yukarı sunucu ile iletişim kurarken kullanacağı bağlantı noktasını ve sunucu adını belirtin.

4.  SSL kullanmak için, **Güncelleştirme bilgilerini eşitlerken SSL kullan** onay kutusunu seçin. Bu durumda sunucular eşitleme için 443 numaralı bağlantı noktasını kullanır. (Hem bu sunucunun, hem de akış yukarı sunucunun SSL'yi desteklediğinden emin olun.)

5.  Bu sunucu bir çoğaltma sunucuysa, **Bu sunucu akış yukarı sunucunun bir çoğaltmasıdır** onay kutusunu seçin.

6.  Bu noktada, akış yukarı sunucu yapılandırmasını tamamlamış olursunuz. **İleri**'yi tıklatın veya sol gezinti bölmesinde **Proxy sunucuyu belirt**'i seçin.

**Proxy sunucu ayarlarını yapılandırmak için**
1.  Yapılandırma sihirbazının **Proxy Sunucuyu Belirt** sayfasında, **Eşitleme yaparken proxy sunucu kullan** onay kutusunu seçin ve sonra ilgili kutulara proxy sunucu adını ve bağlantı noktası numarasını (varsayılan olarak 80 numaralı bağlantı noktası) yazın.

2.  Özel kullanıcı kimlik bilgileri kullanarak proxy sunucuya bağlanmak istiyorsanız, **Proxy sunucuya bağlanmak için kullanıcı kimlik bilgilerini kullan** onay kutusunu işaretleyin ve ilgili kutulara kullanıcı adını, etki alanını ve kullanıcının parolasını yazın. Proxy sunucuya bağlanan kullanıcı için temel kimlik doğrulamasını etkinleştirmek istiyorsanız, **Basit kimlik doğrulamaya izin ver (parola düz metin olarak gönderilir)** onay kutusunu seçin.

3.  Bu noktada, proxy sunucu yapılandırmasını tamamlamış olursunuz. Eşitleme işlemini ayarlamaya başlayabileceğiniz sonraki sayfaya gitmek için **İleri**'yi tıklatın.

Aşağıdaki iki yordamda yapılandırma için WSUS Yönetimi ek bileşenini kullandığınız kabul edilir. Bu iki yordamda, WSUS Yönetimi ek bileşenini nasıl başlatacağınız ve **Seçenekler** sayfasını kullanarak sunucuyu nasıl yapılandıracağınız gösterilir.

**WSUS Yönetim Konsolu'nu başlatmak için**
-   WSUS Yönetim Konsolu'nu başlatmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'ın üzerine gidin, **Yönetimsel Araçlar**'ın üzerine gidin ve sonra **Microsoft Windows Server Update Services 3.0**'ı tıklatın.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="/security-updates/images/Dd939815.note(WS.10).gif" />Not</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Konsolun tüm özelliklerini kullanmak için, WSUS'nin yüklendiği sunucuda WSUS Administrators veya yerel Administrators güvenlik gruplarının bir üyesi olarak oturum açın. WSUS Reporters güvenlik grubunun üyeleri konsolda salt okuma erişimine sahiptir.
</td>
</tr>
</tbody>
</table>
 

**Güncelleştirme kaynağı ve proxy sunucu belirtmek için**
1.  WSUS konsolunda, sol bölmede bu sunucunun adının altında **Seçenekler**'i tıklatın ve sonra orta bölmede **Güncelleştirme Kaynağı ve Proxy Sunucu**'yu tıklatın.

    **Güncelleştirme Kaynağı** ve **Proxy Sunucusu** sekmeleri bulunan bir iletişim kutusu görüntülenir.

2.  **Güncelleştirme Kaynağı** sekmesinde, sunucunun güncelleştirmeleri alacağı konumu seçin. Microsoft Update'ten eşitlemeyi (varsayılan) seçerseniz, bu sihirbaz sayfasında yapacağınız işlemler bitmiştir.

3.  Başka bir WSUS sunucusundan eşitlemeyi seçerseniz, sunucuların iletişim kurmak için kullanacağı bağlantı noktasını belirtmeniz gerekir (varsayılan bağlantı noktası 80'dir). Farklı bir bağlantı noktası seçerseniz, her iki sunucunun da seçtiğiniz bağlantı noktasını kullanabildiğinden emin olmalısınız.

4.  Akış yukarı WSUS sunucusundan eşitleme yaparken SSL kullanılıp kullanılmayacağını da belirtebilirsiniz. Bu durumda, sunucular akış yukarı sunucudan eşitleme yapmak için 443 numaralı bağlantı noktasını kullanırlar.

5.  Bu sunucu diğer WSUS sunucusunun çoğaltmasıysa, **Bu sunucu akış yukarı sunucunun bir çoğaltmasıdır** onay kutusunu seçin. Bu durumda, tüm güncelleştirmelerin yalnızca akış yukarı WSUS sunucusunda onaylanması gerekir.

6.  **Proxy Sunucu** sekmesinde, **Eşitleme işleminde proxy sunucu kullan** onay kutusunu işaretleyin ve ilgili kutulara proxy sunucu adını ve bağlantı noktası numarasını (varsayılan olarak 80 numaralı bağlantı noktası) yazın.

7.  Özel kullanıcı kimlik bilgileri kullanarak proxy sunucuya bağlanmak istiyorsanız, **Proxy sunucuya bağlanmak için kullanıcı kimlik bilgilerini kullan** onay kutusunu işaretleyin ve ilgili kutulara kullanıcı adını, etki alanını ve kullanıcının parolasını yazın. Proxy sunucuya bağlanan kullanıcı için temel kimlik doğrulamasını etkinleştirmek istiyorsanız, **Temel kimlik doğrulamasına izin ver (parola şifresiz metin ile gönderilir)** onay kutusunu işaretleyin.

8.  **Tamam**'ı tıklatarak bu ayarları kaydedin.

Sonraki adım
------------

[Adım 4: Güncelleştirmeleri ve Eşitlemeyi Yapılandırma](https://technet.microsoft.com/deeaa7e1-9b50-45cb-9537-d75f70de3405).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
