---
TOCTitle: 'RMS İstemcisi Nasıl Dağıtılır?'
Title: 'RMS İstemcisi Nasıl Dağıtılır?'
ms:assetid: 'c84f1724-cf71-4385-9003-ff68bc23c927'
ms:contentKeyID: 18125266
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747749(v=WS.10)'
---

RMS İstemcisi Nasıl Dağıtılır?
==============================

Microsoft Windows XP veya Microsoft Windows 2000 kullanıyorsanız, Microsoft® Office Sistemi 2003'teki Bilgi Hakları Yönetimi ve Internet Explorer'daki Hak Yönetimi Eklentisi gibi RMS özelliklerini kullanabilmeniz için Rights Management Services (RMS) istemcisinin yüklü olması gerekir. RMS istemcisi Windows Vista® işletim sisteminde yerleşik olarak bulunur.

Pek çok kuruluş, istemci yazılımlarının kuruluşlarındaki dağıtımını denetlemeyi seçer. RMS Service Pack 2 (SP2) istemcisini dağıtmak için Systems Management Server (SMS) veya Grup İlkesi kullanılabilir.

Dağıtımınıza başlamadan önce, RMS istemcisini yüklemek üzere [http://go.microsoft.com/fwlink/?LinkId=67736](http://go.microsoft.com/fwlink/?linkid=67736) adresine bakın.

| ![](images/Cc747749.Important(WS.10).gif)Önemli                          |
|-------------------------------------------------------------------------------------------------------|
| RMS istemcisi Windows Vista ile tümleşiktir. Bu nedenle, ayrı bir yükleme olarak yüklenmesi gerekmez. |

Yükleme Dosyalarını Ayıklama
----------------------------

WindowsRightsManagementServicesSP2-KB917275-Client-TRK.exe dosyasını karşıdan yükledikten sonra, yürütülebilir paketten Microsoft® Windows® Installer dosyalarını ayıklamanız gerekir.

Bu işlemi yapmak için komut isteminde aşağıdaki komutu kullanabilirsiniz:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x <path>`

Burada &lt;yol&gt;, ayıklanan dosyaları yerleştirmek istediğiniz hedef dizindir.

Bu komutu çalıştırmak, aşağıdaki dosyaların belirttiğiniz hedef dizine ayıklanmasını sağlar:

-   Bootstrap.exe
    Bu dosya, diğer dosyaları yüklemek için yürütülebilir dosya tarafından kullanılan kapsayıcı dosyadır. RMS SP2 istemcisi SMS veya Grup İlkesi kullanılarak yüklenirken kullanılmaz.
-   MSDrmClient.msi
    RMS SP2 istemcisi yükleme dosyasıdır. Bu yükleme, bilgisayarda bulunan önceki tüm RMS istemcisi sürümlerini kaldırır. Bu program önce istemci bilgisayarlara yüklenmelidir.
-   RMClientBackCompat.msi
    RMS SP2 istemcisinin kullanılabilmesini sağlamak amacıyla, RMS istemcisinin önceki sürümüne bağımlı olan RMS etkin uygulamalarda (Microsoft Office Professional 2003 veya 2007 Microsoft Office Sistemi gibi) yeni SP2 istemcisini tanımlayan yükleme dosyasıdır. Bu program istemci bilgisayarlara, MSDrmClient.msi başarılı bir şekilde yüklendikten sonra yüklenmelidir.

| ![](images/Cc747749.note(WS.10).gif)Not                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Uygulamayı seçtiğiniz yükleme yöntemine bağlı olmaksızın, her iki Windows Installer dosyasının da başarılı bir şekilde yüklendiğinden emin olun. MSDrmClient.msi dosyasının yüklenmesini engelleyen bir hata oluşursa, RMClientBackCompat.msi dosyası yüklenmemelidir. |

RMS İstemcisini Bir Katılımsız Yükleme Kullanarak Dağıtma
---------------------------------------------------------

Windows Installer dosyalarını yüklemek üzere dosyaları ayıklamak isteğe bağlıdır. RMS istemcisini, bir katılımsız yükleme yöntemi kullanarak da dağıtabilirsiniz. Bu işlemi yapmak için komut isteminde aşağıdaki komutu kullanabilirsiniz:

`WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q`

Bu komut, RMS istemcisinin katılımsız yüklemesini başlatır.

| ![](images/Cc747749.note(WS.10).gif)Not                                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu bir katılımsız yükleme olduğu için, yükleyici tamamlandığında size bildirmez. Katılımsız yüklemeler genelde bir toplu iş dosyasında veya komut dosyasında çalıştırılır. |

RMS İstemcisini SMS Kullanarak Dağıtma
--------------------------------------

**RMS istemcisini SMS kullanarak dağıtmak için**
1.  SMS Yönetici konsolunu açın.

2.  Kullanmak istediğiniz site veritabanını genişletin.

3.  Soldaki bölmede, **Packages**'ı (Paketler) sağ tıklatın, **New** (Yeni) öğesini seçin ve **Package From Definition**'ı (Tanımdan Paket) tıklatın.

4.  MSDRMClient.msi ve RMClientBackCompat.msi dosyalarından paketleri oluşturun. Paketlerde aşağıdaki özelliklerin olması gerekir:

    **Genel**:

    -   **Komut satırı** için aşağıdaki komutu yazın:
        `msiexec.exe /q ALLUSERS=2 /m MSIDGHOG /i "<file_name>.msi"`
        | ![](images/Cc747749.note(WS.10).gif)Not                                                       |
        |----------------------------------------------------------------------------------------------------------------------------|
        | MSIDGHOG rasgele bir değerdir. &lt;Dosya\_adı&gt; yerine, bu paketin yükleneceği Windows Installer dosyasının adını yazın. |

    -   **Çalıştır** için **Gizli** seçeneğini belirleyin.
    -   **Çalıştırdıktan sonra** için **Herhangi bir eylem gerekmez** seçeneğini belirleyin.
    -   **Kategori** için **Yönetim Yazılımı** seçeneğini belirleyin.

    **Gereksinimler:**

    -   **Hesaplanan disk alanı** için **445 KB** yazın.
    -   **İzin verilen en uzun çalışma süresi** için **Bilinmiyor** seçeneğini belirleyin.
    -   **Bu program tüm platformlarda çalışabilir** onay kutusunu işaretleyin.

    **Environment (Ortam):**

    -   **Programın çalışma koşulu** için **Kullanıcının oturum açmasından bağımsız** seçeneğini belirleyin.
    -   **Çalıştırma modu** için **Yönetim haklarıyla çalıştır** seçeneğini belirleyin.
    -   **Yürütme modu** için **UNC adıyla çalışır** seçeneğini belirleyin.

    **Gelişmiş:**

    -   **Önce başka bir program çalıştır** onay kutusunu temizleyin.
    -   **Program bilgisayara atandığında** seçeneğinin altında bulunan **Program bildirimini engelle** onay kutusundaki işareti kaldırın.
    -   **Bu programı tanıtıldığı bilgisayarlarda devre dışı bırak** onay kutusunu temizleyin.

5.  **Erişim Hesapları ve Dağıtım Noktaları** ayarını kuruluşunuza uygun olan biçimde yapın.

6.  İlgili koleksiyon için bir tanıtım oluşturun. SMS dağıtımında **Katılımsız sistem başına** programını kullanmanız önerilir.

7.  Bu tanıtımı kuruluşunuzun gereksinimlerine göre zamanlayın.

RMS İstemcisini Grup İlkesi Kullanarak Dağıtma
----------------------------------------------

RMS istemcisini hedef bilgisayarlara dağıtmak için Grup İlkesi'nin Yazılım Yüklemesi ve Bakımı özelliğini kullanabilirsiniz.

Grup İlkesi, küçük ve orta ölçekli işletmelerin ya da henüz Systems Management Server 2003 gibi bir şirket yönetim çözümü güncelleştirmesi kullanmayan kuruluşların, RMS istemcileri dağıtımını etkin bir şekilde yönetmeleri için önerilen yöntemdir.

Programı dağıtmak için Grup İlkesi kullandığınızda, programı bilgisayarlara atayabilirsiniz. Program bilgisayar çalışmaya başladığında yüklenir ve bilgisayarda oturum açan tüm kullanıcılar tarafından kullanılabilir. Grup İlkesi hakkında daha fazla bilgi için bkz: Grup İlkesi Alt Yapısını Tasarlama (<http://go.microsoft.com/fwlink/?linkid=24328>). Bu yordam, Grup İlkesi Yönetim Konsolu (GPMC) kullandığınızı varsayar. GPMC'yi karşıdan yüklemek için, Grup İlkesi Yönetim Konsolu Service Pack 1'e (<http://go.microsoft.com/fwlink/?linkid=21813>) bakın.

Aşağıdaki yordam, Grup İlkesi tabanlı yazılım dağıtımı konusunda fazla bilgisi olmayan yöneticiler için hızlı başvuru kılavuzu sağlar. Bu adımları, kuruluşunuzun gereksinimlerini karşılayacak şekilde değiştirebilirsiniz.

**RMS istemcisini Grup İlkesi kullanarak dağıtmak için:**
1.  Etki alanı denetleyicisinde, **Active Directory Kullanıcıları ve Bilgisayarları** Microsoft Yönetim Konsolu (MMC) ek bileşenini açın.

2.  Yeni bir kuruluş birimi oluşturun veya varolan bir kuruluş birimini seçin.

    Yeni bir kuruluş birimi oluşturursanız, RMS İstemcisini yüklemek istediğiniz bilgisayarları ekleyin.

3.  Kuruluş birimini sağ tıklatın ve **Özellikler**'i seçin.

4.  **Grup İlkesi** sekmesini seçin.

5.  Yeni bir Grup İlkesi nesnesi (GPO) oluşturmak için **Yeni**'yi tıklatın.

6.  Yeni GPO'yu düzenlemek için **Düzenle**'yi tıklatın.

7.  Konsol ağacında, **Bilgisayar Yapılandırması, Yazılım Ayarları**'nı genişletin ve **Yazılım yükleme**'yi seçin.

8.  Ayrıntılar bölmesini sağ tıklatın, **Yeni**'yi tıklatın ve sonra da **Paket**'i tıklatın.

9.  İstemci bilgisayarların erişebileceği bir paylaşılan ağ klasöründe bulunan MSDRMclient.msi dosyasının yolunu verin.

10. Paketi atamak için **Tamam**'ı tıklatın.

11. RMClientBackCompat.msi dosyasını yükleyen bir GPO oluşturmak için 5 ile 10 arasındaki adımları yineleyin.

| ![](images/Cc747749.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu adımlar, Grup İlkesi kullanımında deneyimi olmayan kullanıcılara yol göstermek amacıyla verilmiştir. Deneyimli bir Grup İlkesi yöneticisiyseniz, MSDrmClient.msi paketini dağıtmak için kendi işletim yordamlarınızı uygulayabilirsiniz. Buna ek olarak, bu adımlar Windows Server 2003 çalıştıran bir etki alanı denetleyicisine yönelik olduğundan, işlem ve terminoloji Windows 2000 etki alanından farklı olabilir. |

Önceki Bir Sürümden Yükseltme
-----------------------------

        ```
| ![](images/Cc747749.note(WS.10).gif)Not                                                   |
|------------------------------------------------------------------------------------------------------------------------|
| RSM istemcisi işletim sisteminde yerleşik olarak bulunduğu için, bu komut dosyası Windows Vista ile birlikte çalışmaz. |
