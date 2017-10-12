---
TOCTitle: 'Adım 2: Sunucunuza WSUS 3.0 Yükleme'
Title: 'Adım 2: Sunucunuza WSUS 3.0 Yükleme'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18154989
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720469(v=WS.10)'
---

Adım 2: Sunucunuza WSUS 3.0 Yükleme
===================================

Sunucunuzun yükleme gereksinimlerini karşıladığından emin olduktan sonra WSUS 3.0 yüklemeye hazırsınız demektir. Üzerine WSUS 3.0'ı yüklemeyi planladığınız sunucuda, yerel Administrators grubunun üyesi olan bir hesabı kullanarak oturum açmalısınız. Yalnızca yerel Administrators grubunun üyeleri WSUS 3.0'ı yükleyebilir.

Aşağıdaki yordam varsayılan WSUS yükleme seçeneklerini kullanır; bunlara WSUS 3.0 veritabanı yazılımı olarak Windows İç Veritabanı yükleme, güncelleştirmeleri yerel olarak depolama ve 80 numaralı bağlantı noktasındaki IIS Varsayılan Web sitesini kullanma dahildir.

**WSUS 3.0'ı yüklemek için**
1.  **WSUSSetup.exe** yükleyici dosyasını çift tıklatın.

2.  Yükleme sihirbazının **Hoş Geldiniz** sayfasında **İleri**'yi tıklatın.

3.  **Yükleme Modu Seçimi** sayfasında, sunucuyu bu bilgisayara yüklemek istiyorsanız **Yönetim Konsolu da dahil tam sunucu yüklemesi**'ni tıklatın veya yalnızca yönetim konsolunu yüklemek istiyorsanız **Yalnızca Yönetim Konsolu**'nu tıklatın.

4.  **Lisans Sözleşmesi** sayfasında, lisans sözleşmesinin koşullarını dikkatlice okuyun, **Lisans sözleşmesinin koşullarını kabul ediyorum**'u tıklatın ve sonra **İleri**'yi tıklatın.

    ![](images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Yükleme sihirbazının **Güncelleştirme Kaynağı Seç** sayfasında, istemcilerin güncelleştirmeleri nereden alacağını belirtebilirsiniz. **Güncelleştirmeleri yerel olarak depola** onay kutusunu seçerseniz, güncelleştirmeler WSUS 3.0 sunucusunda depolanır ve dosya sisteminde güncelleştirmelerin depolanacağı konumu seçersiniz. Güncelleştirmeleri yerel olarak depolamazsanız, onaylanmış güncelleştirmeleri almak için istemci bilgisayarlar Microsoft Update'e bağlanır. Varsayılan seçenekleri koruyun ve **İleri**'yi tıklatın.

    ![](images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  **Veritabanı Seçenekleri** sayfasında, WSUS 3.0 veritabanını yönetmek için kullanılan yazılımı seçin. Varsayılan olarak, yükleme yaptığınız bilgisayar Windows Server 2003 çalıştırıyorsa, WSUS Kurulumu Windows İç Veritabanı yükleme seçeneği sunar.

7.  Windows İç Veritabanı kullanmak istemiyorsanız, **Bu bilgisayarda varolan bir veritabanı sunucusunu** **kullan**'ı tıklatarak ve kutuya örneğin adını yazarak WSUS'nin kullanacağı SQL Server örneğini sağlamalısınız. Örnek adı &lt;*sunucuAdı*&gt;\\&lt;*örnekAdı*&gt; olarak görünmelidir; burada *sunucuAdı* sunucunun adı ve *örnekAdı* SQL örneğinin adıdır. Seçiminizi yapın ve **İleri**'yi tıklatın.

8.  **SQL Server Örneğine Bağlanılıyor** sayfasında, WSUS belirtilen SQL Server örneğine bağlanmaya çalışır. Başarıyla bağlandığında, devam etmek için **İleri**'yi tıklatın.

    ![](images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  **Web Sitesi Seçimi** sayfasında WSUS 3.0'ın kullanacağı Web sitesini belirtin. 80 numaralı bağlantı noktasındaki varsayılan IIS Web sitesini kullanmak istiyorsanız ilk seçeneği seçin. 80 numaralı bağlantı noktasında zaten bir Web siteniz varsa, ikinci seçeneği seçerek 8530 numaralı bağlantı noktasında alternatif bir site oluşturabilirsiniz. Varsayılan seçeneği koruyun ve **İleri**'yi tıklatın.

10. **Windows Server Update Services Yüklenmeye Hazır** sayfasında, seçimlerinizi gözden geçirin ve sonra **İleri**'yi tıklatın.

11. Yükleme sihirbazının son sayfası size WSUS 3.0 yüklemesinin başarıyla tamamlanıp tamamlanmadığını söyler. **Son**'u tıklattığınızda yapılandırma sihirbazı başlatılır.
