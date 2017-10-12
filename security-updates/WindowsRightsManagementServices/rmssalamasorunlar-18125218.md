---
TOCTitle: RMS Sağlama Sorunları
Title: RMS Sağlama Sorunları
ms:assetid: 'b0e6ef48-ab38-4426-be5b-811cf64c45c0'
ms:contentKeyID: 18125218
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747638(v=WS.10)'
---

RMS Sağlama Sorunları
=====================

RMS sağlama işlemi yaptığınızda, RMS'nin bağlı olduğu çeşitli bileşenler arasındaki kaynak dosyalar ve bağlantılar yapılandırılır ve oluşturulur. RMS kaynak ayarlamaya çalışırken hata oluşursa, sağlama işlemi başarısız olur ve bir hata görüntülenir. Bu bölümde, RMS sağlama işleminin tamamlanmasını engelleyen beklenmedik sorunları gidermenize yardımcı olmak için, bu hataların en yaygın nedenleri ele alınmıştır.

Kök Sertifika Sunucusu Sağlanamıyor
-----------------------------------

Doğru sağlama sayfaları görünmediğinden kök sertifika sunucusu sağlayamıyorsunuz. Bu davranış, ilk kök sertifika sunucusunu sağlamak için Genel Yönetim sayfasından RMS'yi bu Web sitesinde hazırla'yı tıklattığınızda oluşabilir. Kök sertifika sunucusuna yönelik sağlama sayfaları yerine lisans sunucusu sağlama sayfaları görüntülenir.

Bu sorun, bu Active Directory ormanındaki son kök sertifika sunucusundan RMS'yi kaldırmadan önce söz konusu sunucunun yapılandırmasını geri almadığınızda ve sonra da bir kök sertifika sunucusu sağlamaya çalıştığınızda ortaya çıkar. Active Directory ormanındaki tek kök sertifika sunucusunun yapılandırmasını geri aldığınızda, hizmet bağlantı noktasını Active Directory'den kaldırırsınız. RMS'yi kaldırmadan önce ormandaki son kök sertifika sunucusunun yapılandırmasını geri almazsanız, Active Directory'den hizmet bağlantı noktasını kendiniz kaldırmadan bu ormanda yeniden bir kök sertifika sunucusu sağlayamazsınız.

Active Directory ormanında ilk kök sertifika sunucusunu sağlamaya çalıştığınızda lisans sunucusuna ait sağlama sayfaları görüntüleniyorsa, hizmet bağlantı noktasını Active Directory'den aşağıda belirtildiği şekilde kaldırın:

**RMS'ye ait hizmet bağlantı noktasını kaldırmak için**
1.  Gerekiyorsa, Windows Server Destek Araçları'nı yükleyin:

    Windows Server 2003 için, yükleme CD'sindeki \\Support\\Tools klasöründen Suptools.msi dosyasını çalıştırın.

    Windows 2000 Server için, yükleme CD'sindeki \\Support Tools klasöründen Setup.exe dosyasını çalıştırın.

2.  Domain Admins grubu üyesi olan bir hesap kullanarak, kök sertifika sunucusunun üyesi olduğu etki alanının etki alanı denetleyicisine oturum açın.

3.  Komut isteminde aşağıdaki komutu yazın ve ENTER tuşuna basın:

    **ldp**

4.  **Bağlantı**'yı ve sonra **Bağlan**'ı tıklatın.

5.  ENTER tuşuna basın. Herhangi bir bilgi yazmayın.

6.  **Bağlantı**'yı ve sonra **Bağla**'yı tıklatın.

7.  ENTER tuşuna basın. Herhangi bir bilgi yazmayın.

8.  **Görünüm**'ü ve sonra **Ağaç**'ı tıklatın.

9.  ENTER tuşuna basın. Herhangi bir bilgi yazmayın.

    Sol bölmede **dc=EtkiAlanınız,dc=com** görüntülenir.

10. **dc=EtkiAlanınız,dc=com** öğesini genişletin.

11. **Yapılandırma**'yı genişletin.

12. **Hizmetler**'i genişletin.

13. **RightsManagementServices**'i silin.

-veya-

1.  Karşıdan RMS Administration Toolkit'i yükleyin ve kurun. Araç seti [Microsoft Web sitesinden](http://go.microsoft.com/fwlink/?linkid=33841) yüklenebilir.
2.  **Başlat**'ı ve sonra **Çalıştır**'ı tıklatarak komut istemini açın. **Çalıştır** iletişim kutusuna, **cmd** yazın ve sonra **Tamam**'ı tıklatın.
3.  Komut isteminde aşağıdaki komut yazın:
    **ADSCPRegister.exeunregisterscp** &lt;*KayıtSilmeURL*&gt;
4.  &lt;*KayıtSilmeURL*&gt; için RMS hizmet bağlantı noktasının URL'sini yazın, örneğin: https://etkialanım/\_wmcs/Certification.

Bu adımları tamamladıktan sonra, kök sertifika sunucusunu sağlayabilirsiniz.

SSPI İçeriği Üretilemiyor
-------------------------

Kök sertifika sunucusu Microsoft Kayıt Hizmeti'ne kaydettirilirken RMS hizmet hesabının kimliği doğrulanmazsa, sağlama işlemi sırasında "SSPI içeriği üretilemiyor" hata iletisini alabilirsiniz.

Bu hata iletisini alırsanız, RMS hizmet hesabının geçerli bir etki alanı hesabı olduğunu doğrulayın. Hesap bir grup hesabıysa, grup üyeliğinin geçerli olduğunu, etki alanındaki grupta yer alan tüm kullanıcı hesaplarını çözümleyebildiğinizi ve hesapların SQL veritabanları için izinleri olduğunu doğrulayın.
