---
TOCTitle: 'Adım 2: Sunucunuza WSUS Yükleme'
Title: 'Adım 2: Sunucunuza WSUS Yükleme'
ms:assetid: 'f593532c-e92e-47f3-914a-38a6c2519e94'
ms:contentKeyID: 18155374
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708622(v=WS.10)'
---

Adım 2: Sunucunuza WSUS Yükleme
===============================

Yükleme gereksinimlerini inceledikten sonra WSUS'yi yüklemeye hazırsınız. WSUS'yi yüklemeyi planladığınız sunucuya, yerel Administrators grubunun üyesi olan bir hesabı kullanarak oturum açmalısınız. Yalnızca yerel Administrators grubunun üyeleri WSUS'yi yükleyebilir.

Aşağıdaki yordam, WSUS veritabanı yazılımı için Windows SQL Server 2000 Desktop Engine (WMSDE) uygulamasını yükleme, güncelleştirmeleri yerel olarak depolama ve bağlantı noktası 80'de IIS Varsayılan Web sitesini kullanmayı içeren Windows Server 2003 için varsayılan WSUS yükleme seçeneklerini kullanır. Farklı işletim sistemi, veritabanı yazılımı veya özel bağlantı noktası kullanan Web sitesi kullanma gibi özel yükleme seçenekleriyle ilgili yordamları “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesinde bulabilirsiniz (Belge İngilizce'dir).

**Windows Server 2003'e WSUS'yi yüklemek için**
1.  **WSUSSetup.exe** yükleyici dosyasını çift tıklatın.

    | ![](/security-updates/images/Cc708622.note(WS.10).gif)Not                                                                                                                                                           |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | WSUSSetup.exe dosyasının en son sürümü, http://go.microsoft.com/fwlink/?LinkId=47374 adresindeki Windows Server Update Services'a yönelik [Microsoft Web sitesinde](http://go.microsoft.com/fwlink/?linkid=47374) bulunabilir. |

2.  Sihirbazın **Hoş Geldiniz**sayfasında **İleri**’yi tıklatın.

3.  Lisans sözleşmesinin koşullarını okuyun ve **Lisans sözleşmesinin koşullarını kabul ediyorum**'u tıklattıktan sonra **İleri**'yi tıklatın.

4.  **Güncelleştirme Kaynağı Seç** sayfasında istemcilerin güncelleştirmeleri alacağı yeri belirtebilirsiniz. **Güncelleştirmeleri yerel olarak depola** onay kutusunu seçerseniz, güncelleştirmeler WSUS sunucusunda depolanır ve dosya sisteminde güncelleştirmelerin depolanacağı konumu siz seçersiniz. Güncelleştirmeleri yerel olarak depolamazsanız, onaylanmış güncelleştirmeleri almak için istemci bilgisayarlar Microsoft Update'e bağlanır.

    Varsayılan seçenekleri koruyun ve **İleri**'yi tıklatın.

    ![](/security-updates/images/Cc708622.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  **Veritabanı Seçenekleri** sayfasında WSUS veritabanını yönetmek için kullanılan yazılımı seçersiniz. Varsayılan olarak, yükleme yaptığınız bilgisayar Windows Server 2003 çalıştırıyorsa, WSUS Kurulumu WMSDE'yi yükleme seçeneği sunar.

    WMSDE'yi kullanamıyorsanız, **Bu bilgisayarda varolan bir veritabanı sunucusu kullan**'ı tıklatarak ve **SQL örneği adı** kutusuna örnek adını yazarak WSUS'nin kullanacağı SQL Server örneğini sağlamalısınız. WMSDE'nin yanı sıra veritabanı yazılımı seçenekleri hakkında daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir).

    Varsayılan seçenekleri koruyun ve **İleri**'yi tıklatın.

    ![](/security-updates/images/Cc708622.bc0b73ad-b338-437c-a3c7-0299e819840d(WS.10).gif)

6.  **Web Sitesi Seçimi** sayfasında WSUS'nin kullanacağı Web sitesini belirtirsiniz. Bu sayfada aynı zamanda bu seçimi temel alan iki önemli URL de listelenir: güncelleştirmeleri almak için WSUS istemci bilgisayarlarına bildireceğiniz URL ve WSUS'yi yapılandıracağınız WSUS konsolunun URL'si.

    Bağlantı noktası 80'de zaten bir Web siteniz varsa, WSUS Web sitesini özel bir bağlantı noktasında oluşturmanız gerekebilir. WSUS'yi özel bir bağlantı noktasında çalıştırma hakkında daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir).

    Varsayılan seçeneği koruyun ve **İleri**'yi tıklatın.

    ![](/security-updates/images/Cc708622.64ed7643-a050-4f54-bf9f-04cf7931adc0(WS.10).gif)

7.  **Güncelleştirme Ayarlarını Yansıt** sayfasında bu WSUS sunucusu için yönetim rolü belirtebilirsiniz. Bu, ağınızdaki ilk WSUS sunucusuysa veya dağıtılmış yönetim topolojisi istiyorsanız bu ekranı atlayın.

    Merkezi yönetim topolojisi istiyorsanız ve bu, ağınızdaki ilk WSUS sunucusu değilse, onay kutusunu işaretleyin ve **Sunucu adı** kutusuna ek WSUS sunucusunun adını yazın. Yönetim rolleri hakkında daha fazla bilgi için “Microsoft Windows Server Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir).

    Varsayılan seçeneği koruyun ve **İleri**'yi tıklatın.

    ![](/security-updates/images/Cc708622.f26e09d5-983c-418d-8511-8960850403ef(WS.10).gif)

8.  **Windows Server Update Services Yüklenmeye Hazır**sayfasında seçimlerinizi gözden geçirin ve **İleri**’yi tıklatın.

    ![](/security-updates/images/Cc708622.20de7d09-3d30-4867-9253-6f353dd1923d(WS.10).gif)

9.  Sihirbazın son sayfasında WSUS yüklemesinin başarıyla tamamlandığı onaylanıyorsa **Son**'u tıklatın.
