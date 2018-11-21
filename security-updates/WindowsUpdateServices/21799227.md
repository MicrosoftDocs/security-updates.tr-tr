---
TOCTitle: 'Adım 2: WSUS Sunucusu''nu veya Yönetim Konsolu''nu Yükleme'
Title: 'Adım 2: WSUS Sunucusu''nu veya Yönetim Konsolu''nu Yükleme'
ms:assetid: '6db6fcb0-c55d-43b9-9b07-4040c6267759'
ms:contentKeyID: 21799227
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Dd939859(v=WS.10)'
---

Adım 2: WSUS Sunucusu'nu veya Yönetim Konsolu'nu Yükleme
========================================================

Sunucunun minimum sistem gereksinimlerini karşıladığından ve gerekli hesap izinlerinin verildiğinden emin olduktan sonra, Windows Server Upgrade Services 3.0 Service Pack 2'yi (WSUS 3.0 SP2) yüklemeye hazırsınız demektir. İşletim sisteminiz için uygun yordamı ve yükleme türünü kullanarak (Sunucu Yöneticisi'ni veya WUSSetup.exe dosyasını kullanarak) WSUS 3.0 SP2 yüklemesini başlatın.

Sunucu Yöneticisi Kullanıyorsanız
---------------------------------

**Sunucu Yöneticisi'ni kullanarak WSUS 3.0 SP2 Server yüklemesini başlatmak için**
1.  Üzerine WSUS 3.0 SP2'yi yüklemeyi planladığınız sunucuda, yerel Administrators grubunun üyesi olan bir hesabı kullanarak oturum açın.

2.  **Başlat**'ı tıklatın, **Yönetimsel Araçlar**'ın üzerine gelin ve **Sunucu Yöneticisi**'ni tıklatın.

3.  Sunucu Yöneticisi penceresinin sağ bölmesinde, Rol Özeti bölümünde **Rol Ekle**'yi tıklatın.

4.  Başlamadan Önce sayfası görüntülenirse, **İleri**'yi tıklatın.

5.  Sunucu Rollerini Seç sayfasında, **Windows Server Update Services** seçeneğini belirleyin.

6.  Windows Server Update Services sayfasında **İleri**'yi tıklatın.

7.  Yükleme Seçimlerini Onaylama sayfasında **Yükle**'yi tıklatın.

8.  WSUS 3.0 SP2 Kurulum Sihirbazı başlatıldığında, bir sonraki bölümü atlayıp “WSUS 3.0 SP2 yüklemeye devam etmek için” yordamına bakın.

WUSSetup.exe Dosyasını Kullanıyorsanız
--------------------------------------

**WUSSetup.exe dosyasını kullanarak WSUS 3.0 SP2 Server veya WSUS 3.0 SP2 Yönetim Konsolu'nun yüklemesini başlatmak için**
1.  Üzerine WSUS 3.0 SP2'yi yüklemeyi planladığınız sunucuda, yerel Administrators grubunun üyesi olan bir hesabı kullanarak oturum açın.

2.  **WSUSSetup.exe** yükleyici dosyasını çift tıklatın.

3.  Windows Server Update Services 3.0 SP2 Kurulum Sihirbazı başlatıldığında, “WSUS 3.0 SP2 yüklemeye devam etmek için” yordamına bakın.

WSUS 3.0 SP2 Kurulum Sihirbazı'nı kullanma
------------------------------------------

WSUS Kurulum Sihirbazı, Sunucu Yöneticisi'nden veya WUSSetup.exe dosyasından başlatılır.

**WSUS 3.0 SP2 yüklemeye devam etmek için**
1.  Windows Server Update Services 3.0 Kurulum Sihirbazı'nın Karşılama sayfasında, **İleri**'yi tıklatın.

2.  Yükleme Modu Seçimi sayfasında, WSUS sunucusunu bu bilgisayara yüklemek istiyorsanız **Yönetim Konsolu da dahil tam sunucu yüklemesi**'ni tıklatın veya yalnızca yönetim konsolunu yüklemek istiyorsanız **Yalnızca Yönetim Konsolu**'nu tıklatın.

3.  Lisans Sözleşmesi sayfasında, lisans sözleşmesinin koşullarını okuyun, **Lisans sözleşmesinin koşullarını kabul ediyorum**'u ve sonra **İleri**'yi tıklatın.

4.  Yükleme sihirbazının Güncelleştirme Kaynağı Seç sayfasında, istemcilerin güncelleştirmeleri nereden alacağını belirtebilirsiniz. Varsayılan olarak, **Güncelleştirmeleri yerel olarak depola** onay kutusu seçilidir ve güncelleştirmeler belirttiğiniz konumdaki WSUS sunucusunda depolanır. **Güncelleştirmeleri yerel olarak depola** onay kutusunun işaretini kaldırırsanız, istemci bilgisayarlar Microsoft Update'e bağlanarak onaylanan güncelleştirmeleri alır. Seçiminizi yapın ve **İleri**'yi tıklatın.

5.  Veritabanı Seçenekleri sayfasında, WSUS 3.0 veritabanını yönetmek için kullanılan yazılımı seçin. Yükleme sihirbazı varsayılan olarak, Windows İç Veritabanı yükleme seçeneğini sunar.

    Windows İç Veritabanı kullanmak istemiyorsanız, **Bu bilgisayarda varolan bir veritabanı sunucusu kullan** veya **Uzak bir bilgisayardaki varolan veritabanı örneğini kullan** seçeneğini belirleyerek WSUS'nin kullanması için bir SQL Server örneği sağlayın. İlgili kutuya örnek adını yazın. Örnek adı &lt;*sunucuAdı*&gt;\\&lt;*örnekAdı*&gt; olarak görünmelidir; burada *sunucuAdı* sunucunun adı ve *örnekAdı* SQL örneğinin adıdır. Seçiminizi yapın ve **İleri**'yi tıklatın.

6.  Bir SQL Server'a bağlanmaya karar verdiyseniz, **SQL Server Örneğine Bağlanılıyor** sayfasında WSUS belirtilen SQL Server örneğine bağlanmayı dener. Başarıyla bağlandığında, devam etmek için **İleri**'yi tıklatın.

7.  Web Sitesi Seçimi sayfasında WSUS'nin kullanacağı Web sitesini belirtin. 80 numaralı bağlantı noktasında varsayılan Web sitesini kullanmak istiyorsanız **Varolan IIS Varsayılan Web sitesini kullan** seçeneğini belirleyin. 80 numaralı bağlantı noktasında zaten bir Web sitesi varsa, **Windows Server Update Services 3.0 SP2 Web sitesi oluştur** seçeneğini belirleyerek 8530 numaralı bağlantı noktasında alternatif bir site oluşturabilirsiniz. **İleri**'yi tıklatın.

8.  **Windows Server Update Services Yüklenmeye Hazır** sayfasında, seçimlerinizi gözden geçirin ve sonra **İleri**'yi tıklatın.

9.  Yükleme sihirbazının son sayfasında, WSUS yüklemesinin başarıyla tamamlanıp tamamlanmadığı bildirilir. Siz **Son**'u tıklattıktan sonra yapılandırma sihirbazı başlatılır.

Sonraki adım
------------

[Adım 3: Ağ Bağlantılarını Yapılandırma](https://technet.microsoft.com/42a144c5-f08e-4a6e-b360-47ddea77bd24).

Ek kaynaklar
------------

[Windows Server Update Services 3.0 SP2 Adım Adım Kılavuzu](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
