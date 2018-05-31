---
TOCTitle: Yapılandırma Veritabanına Geçiş
Title: Yapılandırma Veritabanına Geçiş
ms:assetid: '980e3e94-7d28-40dd-ad01-d34eb3c8d8e6'
ms:contentKeyID: 18125212
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747607(v=WS.10)'
---

Yapılandırma Veritabanına Geçiş
===============================

Veritabanı sunucusunun geri çekilmesini gerektiren durumlar vardır. RMS veritabanı sunucusu donanım yükseltmesi bir örnektir. Veritabanı sunucusu geri çekildikten sonra, yapılandırma veritabanı farklı bir veritabanı sunucusuna taşınmalıdır. İçerdiği anahtar çiftleri gibi yapılandırma veritabanındaki verileri korumak için, dikkatli bir şekilde bir geçiş planlamanız ve uygulamanız gereklidir.

RMS veritabanı sunucusu için bir CNAME diğer adı oluşturmanızı ve ardından RMS'yi bu diğer adı kullanmak üzere yapılandırmanızı öneririz. Bu sayede sunucunun adı değişirse RMS yapılandırma veritabanındaki veritabanı sunucu adını el ile değiştirmek gerekmez. CNAME diğer adı kullanıldığında, yalnızca diğer ad kaydını güncelleştirmeniz gerekir.

Yapılandırma veritabanı geçişine başlamadan önce, aşağıdaki bilgilere sahip olduğunuzdan emin olun:

-   Bu veritabanını kullanan RMS kümesi içindeki sunucuları sağlamak için önceden kullanılan hesap adı ve parolası.
-   RMS özel anahtarını saklamak için yazılım tabanlı bir şifreleme hizmeti sağlayıcısı (CSP) kullanılıyorsa, sağlama sırasında önceden belirtilmiş olan RMS özel anahtar parolası. RMS özel anahtar parolasını saklamak için bir donanım güvenlik modülü (HSM) kullanılıyorsa, bu adım gerekli değildir.

| ![](/security-updates/images/Cc747607.note(WS.10).gif)Not                                                                                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Yapılandırma veritabanını geçirme yeni bir sunucu lisans sertifikası veya yeni bir sunucu özel anahtarı gerektirmez. Çünkü RMS özgün yapılandırma veritabanındaki ayarları saklar. |

Veritabanı sunucusu üzerinde herhangi bir şey yapmadan önce RMS veritabanlarını yedeklemeniz gereklidir. Bu bir seçenek değilse, en azından sunucu lisans sertifikanızı vermeniz gereklidir. Sunucu lisans sertifikasını verme hakkında daha fazla bilgi için, bkz. [Sunucu Lisans Sertifikanızı Dosyaya Vermek için](https://technet.microsoft.com/d683a629-71b3-4b11-932b-4ab0317334af). Veritabanı geçirilirken bir hata oluşursa, sunucu lisan sertifikasını yeni RMS yüklemesi içine alabilir ve eski yüklemede korunan içeriği kullanabilirsiniz.

Yapılandırma veritabanını geçirmek için aşağıdaki adımları kullanın:

-   Yeni veritabanı sunucusunun adını yansıtmak için RMS yapılandırma veritabanını güncelleştirin.
-   Yeni veritabanı sunucu adını kullanmaları için RMS kümesinde bulunan her sunucudaki web.config dosyasını ve kayıt defterini güncelleştirin

| ![](/security-updates/images/Cc747607.Important(WS.10).gif)Önemli                                                          |
|---------------------------------------------------------------------------------------------------------------------------------------|
| Bu konu RMS veritabanlarını barındıracak olan yeni veritabanı sunucusuna, RMS veritabanlarının önceden kopyalanmış olduğunu varsayar. |

RMS yapılandırma dosyasını yeni veritabanı sunucusu adını kullanacak şekilde güncelleştirin
-------------------------------------------------------------------------------------------

RMS veritabanlarını barındıran veritabanı sunucusunun adı RMS yapılandırma veritabanında saklanır. Veritabanı dosyaları yeni veritabanı sunucusuna geçirildikten sonra, RMS yapılandırma veritabanını güncelleştirmeniz gerekir. Bu, RMS Yönetim Araç Seti'ndeki RMS Config Editör aracını kullanarak veya SQL Management Studio ile yapılabilir.

RMS veritabanı sunucu adını RMS Config Editor kullanarak güncelleştirmek için, aşağıdaki adımları kullanın:

**RMS yapılandırma veritabanını RMS Config Editor kullanarak güncelleştirmek için**
1.  Kümedeki RMS sunucusuna System Administrators veritabanı rolünün bir üyesi olarak oturum açın.

2.  Microsoft Yükleme Merkezi'nden ([http://go.microsoft.com/fwlink/?LinkId=98961](http://go.microsoft.com/fwlink/?linkid=98961)) RMS Yönetim Araç Seti'ni yükleyin.

3.  %SystemDrive%:\\Program Files\\RMS SP2 Administration Toolkit\\RMSConfigEditor dizinine gidin ve **RMSCONFIGEDITOR.EXE** dosyasını çift tıklatın.

4.  **Server** kutusuna RMS yapılandırma veritabanını barındıran yeni sunucunun adını yazın ve ardından **Go**'yu tıklatın.

5.  **Database** kutusunda **DRMS\_Config\_***&lt;RMS küme adı&gt;***\_***&lt;BağNok&gt;* seçeneğini tıklatın, burada *&lt;RMS küme adı&gt;* RMS kümesinin adı ve *&lt;BağNok&gt;* RMS'nin iletişim kurduğu TCP bağlantı noktasıdır, ardından **Go**'yu tıklatın.

6.  **DRMS\_ClusterPolicies**'i tıklatın.

7.  Sonuçlar bölmesinde, **LoggingDatabaseServer** satırının **PolicyData** sütunundaki değeri yeni RMS veritabanı sunucusu adıyla değiştirin.

8.  **Persist**'i tıklatın.

9.  **CertificationUserKeyStorageConnectionString** satırının **PolicyData** sütunundaki değeri yeni veritabanı sunucusunu yansıtacak şekilde değiştirin. Değer **data source=***&lt;yeni veritabanı sunucu adı&gt;***;integrated** burada *&lt;yeni veritabanı sunucu adı&gt;* yeni veritabanı sunucusunun adıdır.

10. **Persist**'i tıklatın.

11. **DirectoryServicesCacheDatabase** satırının **PolicyData** sütunundaki değer için 9. ve 10. adımları yineleyin.

12. Sol bölmede, **DRMS\_PluginProperties**'i tıklatın.

13. **PERSISTENT\_STORAGE** adlı **PropertyID** 101 için, **PropertyValue** sütununu yeni veritabanı sunucusunu yansıtacak şekilde değiştirin. Değer **data source=***&lt;yeni veritabanı sunucu adı&gt;***;integrated** burada *&lt;yeni veritabanı sunucu adı&gt;* yeni veritabanı sunucusunun adıdır.

14. **Persist**'i tıklatın.

15. RMS Config Editor'ü kapatın.

RMS yapılandırma veritabanını SQL Server Management Studio kullanarak güncelleştirmek için, aşağıdaki adımları uygulayın:

**RMS yapılandırma veritabanını SQL Server Management Studio kullanarak güncelleştirmek için**
1.  RMS yapılandırma sunucusunda yerel Administrator veya yerel Administrators grubunun bir üyesi olarak oturum açın.

2.  **Başlat**'ı tıklatın, **Tüm Programlar**'ın, **Microsoft SQL Server 2005**'in üzerine gelin ve ardından **SQL Server Management Studio**'yu tıklatın.

3.  **Sunucuya Bağlan** sayfasında, yeni veritabanı sunucusu adının **Sunucu adı** kutusunda listelendiğinden emin olduktan sonra **Bağlan**'ı tıklatın.

4.  **Veritabanları**'nı, **DRMS\_Config\_***&lt;RMS küme adı&gt;***\_***&lt;BağNok&gt;* düğümünü genişletin ve ardından **Tablolar**'ı açın.

5.  **DRMS\_ClusterPolicies**'i sağ tıklatın ve **Open Table**'ı tıklatın.

6.  Sonuçlar bölmesinde, **LoggingDatabaseServer** satırının **PolicyData** sütunundaki değeri yeni RMS veritabanı sunucusu adıyla değiştirin.

7.  **CertificationUserKeyStorageConnectionString** satırının **PolicyData** sütunundaki değeri yeni veritabanı sunucusunu yansıtacak şekilde değiştirin. Değer **data source=***&lt;yeni veritabanı sunucu adı&gt;***;integrated** burada *&lt;yeni veritabanı sunucu adı&gt;* yeni veritabanı sunucusunun adıdır.

8.  **DirectoryServicesCacheDatabase** satırının **PolicyData** sütunundaki değer için 6. ve 7. adımları yineleyin.

9.  Object Explorer bölmesinde, **DRMS\_PluginProperties**'i sağ tıklatın ve ardından **Open Table**'ı tıklatın.

10. **PERSISTENT\_STORAGE** adlı **PropertyID** 101 için, **PropertyValue** sütununu yeni veritabanı sunucusunu yansıtacak şekilde değiştirin. Değer **data source=***&lt;yeni veritabanı sunucu adı&gt;***;integrated** burada *&lt;yeni veritabanı sunucu adı&gt;* yeni veritabanı sunucusunun adıdır.

11. Microsoft SQL Server Management Studio'yu kapatın.

RMS kümesindeki her sunucuyu yeni veritabanı sunucu adını kullanacak şekilde yapılandırın
-----------------------------------------------------------------------------------------

RMS kümesindeki her sunucuyu yeni veritabanı sunucu adını kullanacak şekilde yapılandırmak için, web.config dosyalarını ve üç kayıt defteri girdisini güncelleştirin. Bu işlem tamamlandıktan sonra, değişikliklerin etkinleşmesi için Internet Information Services'ı (IIS) yeniden başlatmanız gerekir.

RMS kümesindeki her sunucuda web.config dosyalarını güncelleştirmek için:

**RMS kümesindeki her sunucuda web.config dosyalarını güncelleştirmek için**
1.  RMS kümesindeki bir sunucuda yerel Administrators grubunun bir üyesi olarak oturum açın.

2.  %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\admin klasörüne gidin.

3.  **web.config** dosyasını çift tıklatın ve **Listeden bir program seçmek** seçeneğini ve ardından **Tamam**'ı tıklatın.

4.  **Not Defteri**'ni tıklatın ve **Bu tür dosyaları açmak için her zaman seçili programı kullan**'ı temizleyerek **Tamam**'ı tıklatın.

5.  **Düzen** ve sonra **Değiştir**'i tıklatın.

6.  **Aranan** kutusuna, RMS veritabanlarını barındırmakta olan geri çekilecek veritabanı sunucusunun adını yazın.

7.  **Yeni değer** kutusuna, RMS veritabanlarını barındıran olan yeni veritabanı sunucusunun adını yazın.

8.  **Tümünü Değiştir** ve ardından **İptal**'i tıklatın.

9.  **Dosya**'yı ve daha sonra **Kaydet**'i tıklatın.

10. Not Defteri'ni kapatın.

11. %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\certification ve %Systemdrive%\\inetpub\\wwwroot\\\_wmcs\\licensing dizinlerinde bulunan web.config dosyaları için 2 ile 9 arasındaki adımları yineleyin.

12. RMS kümesindeki her sunucu için 1 ile 11 arasındaki adımları yineleyin.

Yeni veritabanı sunucu adını kullanmaları için RMS kümesinde bulunan her sunucudaki kayıt defterini güncelleştirin

| ![](/security-updates/images/Cc747607.Caution(WS.10).gif)Dikkat                                                                                        |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kayıt defterinin yanlış düzenlenmesi sisteminize zarar verebilir. Kayıt defterinde değişiklik yapmadan önce, bilgisayarınızdaki önemli verileri yedeklemelisiniz. |

**RMS kümesindeki her sunucuda kayıt defterini güncelleştirmek için**
1.  RMS kümesindeki bir sunucuda yerel Administrators grubunun bir üyesi olarak oturum açın.

2.  **Başlat**'ı ve sonra **Çalıştır**'ı tıklatın.

3.  **regedit.exe** yazın ve ardından **Tamam**'ı tıklatın.

4.  **KEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\KeyProtection**'a gidin.

5.  PASSWORDDERIVEDKEY\_*&lt;eski veritabanı sunucusu adı&gt;*\_DRMS\_CONFIG\_*&lt;RMS küme adı&gt;*\_*&lt;bağnok&gt;* kayıt defteri girişini:

    PASSWORDDERIVEDKEY\_*&lt;eski veritabanı sunucusu adı&gt;*\_DRMS\_CONFIG\_*&lt;RMS küme adı&gt;*\_*&lt;bağnok&gt;*

    burada:

    -   *&lt;eski veritabanı sunucusu&gt;* eski veritabanı sunucusunun adıdır.
    -   *&lt;RMS küme adı&gt;* RMS kümesinin adıdır.
    -   *&lt;bağnok&gt;* RMS'nin iletişim kurduğu TCP bağlantı noktasıdır.
    -   *&lt;yeni veritabanı sunucusu&gt;* yeni veritabanı sunucusunun adıdır.

6.  **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet001\\Services\\DRMS\_Logging\_&lt;RMS küme adı&gt;\_&lt;bağnok&gt;\\Params** girişine gidin.

7.  Veri kaynağı adı yeni veritabanı sunucusu adıyla eşleşecek şekilde **ConnectionString** kayıt defteri girişini değiştirin.

8.  **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\DRMS\_Logging\_&lt;RMS küme adı&gt;\_&lt;bağnok&gt;\\Params** için 6. ve 7. adımları yineleyin.

9.  Komut satırında **IISRESET** yazıp ENTER tuşuna basın.

10. RMS kümesindeki her sunucu için 1 ile 9 arasındaki adımları yineleyin.
