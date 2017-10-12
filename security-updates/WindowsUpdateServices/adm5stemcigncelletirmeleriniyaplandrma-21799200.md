---
TOCTitle: 'Adım 5: İstemci Güncelleştirmelerini Yapılandırma'
Title: 'Adım 5: İstemci Güncelleştirmelerini Yapılandırma'
ms:assetid: '5ae60ead-3e94-456c-a692-c0f193ea5d5a'
ms:contentKeyID: 21799200
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939830(v=WS.10)'
---

Adım 5: İstemci Güncelleştirmelerini Yapılandırma
=================================================

Windows Server Update Services 3.0'da (WSUS 3.0 SP2), WSUS Kurulumu, WSUS sunucusuyla bağlantı kuran her istemci bilgisayara en son Otomatik Güncelleştirmeler sürümünü dağıtmak için otomatik olarak IIS'yi yapılandırır.

Otomatik Güncelleştirmeler'i yapılandırmanın en iyi yöntemi ağ ortamına bağlıdır. Active Directory® dizin hizmetini kullanan bir ortamda, varolan etki alanı tabanlı bir Grup İlkesi nesnesini (GPO) kullanabilir veya yeni bir GPO oluşturabilirsiniz. Active Directory bulunmayan bir ortamda, Yerel Grup İlkesi nesnesini kullanın. Bu aşamada, Otomatik Güncelleştirmeler'i yapılandırır ve istemci bilgisayarları WSUS sunucusunu işaret edecek şekilde ayarlarsınız.

Aşağıdaki yordamlarda, ağınızda Active Directory çalıştırıldığı varsayılır. Bu yordamlarda, Grup İlkesi kullanmayı bildiğiniz ve ağınızı yönetmek için Grup İlkesi kullandığınız da varsayılır.

Grup İlkesi hakkında daha fazla bilgi için, bkz. Grup İlkesi Teknoloji Merkezi Web sitesi [http://go.microsoft.com/fwlink/?LinkID=47375](http://go.microsoft.com/fwlink/?linkid=47375).

 
-

Adım 5 Yordamlar
----------------

Adım 4'te, karşıdan yüklemek istediğiniz güncelleştirmelerin yapılandırmasını tamamladınız. İstemci bilgisayarlar için otomatik güncelleştirmeleri yapılandırmak üzere bu yordamlar dizisini kullanın.

1.  Grup İlkesi'nde Otomatik Güncelleştirmeler'i Yapılandırma.
2.  İstemci bilgisayarınızı WSUS sunucusunu işaret edecek şekilde ayarlama.
3.  WSUS sunucusu tarafından algılamayı el ile başlatma.

İlk iki yordamı istediğiniz etki alanı tabanlı GPO'da, üçüncü yordamı ise istemci bilgisayardaki bir komut isteminde yaparsınız.

**Otomatik Güncelleştirmeler'i yapılandırmak için**
1.  Grup İlkesi Yönetim Konsolu'nda (GPMC), üzerinde WSUS'yi yapılandırmak istediğiniz GPO'ya gözatın ve **Düzenle**'yi tıklatın.

2.  GPMC'de sırayla **Bilgisayar Yapılandırma**'yi, **Yönetim Şablonları**'nı ve **Windows Bileşenleri**'ni genişletip **Windows Update**'i tıklatın.

3.  Ayrıntılar bölmesinde **Otomatik Güncelleştirmeleri Yapılandır**'ı çift tıklatın.

4.  **Etkin**'i tıklatın ve sonra aşağıdaki seçeneklerden birini tıklatın:

    -   **Karşıdan yükleme ve kurma için uyar**. Bu seçenek, yönetici olarak oturum açmış olan kullanıcıyı karşıdan yükleme başlamadan ve güncelleştirmeleri kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurma için uyar**. Bu seçenek güncelleştirmelerin karşıdan yüklenmesini otomatik olarak başlatır ve yönetici olarak oturum açmış kullanıcıyı güncelleştirmeleri kurmadan önce uyarır.
    -   **Otomatik olarak karşıdan yükle ve kurmayı zamanla**. Bu seçenek otomatik olarak güncelleştirmelerin karşıdan yüklenmesini başlatır ve belirttiğiniz gün ve saatte güncelleştirmeleri kurar.
    -   **Yerel yöneticinin ayarı seçmesine izin ver**. Bu seçenek, Yerel yöneticilerin istedikleri yapılandırma seçeneklerini belirlemek üzere Denetim Masası'ndaki Otomatik Güncelleştirmeler'i kullanmalarına olanak verir. Örneğin, kendi zamanlanmış yükleme saatlerini seçebilirler. Yerel yöneticiler Otomatik Güncelleştirmeler'i devre dışı bırakamaz.

5.  **Tamam**'ı tıklatın.

**İstemci bilgisayarları WSUS sunucusunu işaret edecek şekilde ayarlamak için**
1.  **Windows Update** ayrıntılar bölmesinde, **Intranet Microsoft güncelleştirme hizmeti konumunu belirt**'i çift tıklatın.

2.  **Etkin**'i tıklatın ve **Güncelleştirmeleri algılamak için intranet güncelleştirme hizmetini ayarla** kutusunda ve **İntranet istatistik sunucusunu ayarla** kutusunda aynı WSUS sunucusunun HTTP URL'sini yazın. Örneğin, her iki kutuya da *http://sunucuadı* yazın ve sonra **Tamam**'ı tıklatın.

 
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" ><img src="images/Dd939830.note(WS.10).gif" />Not</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Bilgisayarı WSUS'yi işaret edecek şekilde ayarlamak için Yerel Grup İlkesi nesnesini kullanıyorsanız, bu ayar hemen etkin olur ve bu bilgisayar kısa bir süre sonra WSUS yönetici konsolunda görüntülenir. El ile bir algılama döngüsü başlatarak bu süreci hızlandırabilirsiniz.
</td>
</tr>
</tbody>
</table>
 

İstemci bilgisayar kurulduktan sonra, bilgisayarın WSUS Yönetim Konsolundaki **Bilgisayarlar** sayfasında görüntülenmesi birkaç dakika sürer. Etki alanı tabanlı bir Grup İlkesi ile yapılandırılmış istemci bilgisayarlar için, Grup İlkesi'nin yenilenmesi yaklaşık 20 dakika sürebilir (yani, tüm yeni ilke ayarları istemci bilgisayara uygulanır). Varsayılan olarak, Grup İlkesi arka planda 0 ile 30 dakikalık rasgele sapmalarla her 90 dakikada bir güncelleştirilir. Grup İlkesi'nin daha hızlı güncelleştirilmesini istiyorsanız, istemci bilgisayarda komut istemine gidip **gpupdate /force** yazabilirsiniz.

Yerel GPO kullanılarak yapılandırılmış istemci bilgisayarlar için, Grup İlkesi hemen uygulanır ve güncelleştirme yaklaşık 20 dakika sürer.

Algılamayı el ile başlatırsanız, istemci bilgisayarın WSUS ile iletişim kurması için 20 dakika beklemeniz gerekmez.

**WSUS sunucusunun algılamasını el ile başlatmak için**
1.  İstemci bilgisayarda, **Başlat**'ı ve sonra **Çalıştır**'ı tıklatın.

2.  **Aç** kutusuna **cmd** yazın ve sonra **Tamam**'ı tıklatın.

3.  Komut istemine **wuauclt.exe /detectnow** yazın. Bu komut satırı seçeneği Otomatik Güncelleştirmeler'in WSUS sunucusuyla hemen iletişim kurmasını sağlar.

Sonraki adım
------------

[Adım 6: Bilgisayar Gruplarını Yapılandırma](https://technet.microsoft.com/70518732-2179-4e41-9609-7f9999867f41).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
