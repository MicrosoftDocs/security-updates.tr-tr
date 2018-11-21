---
TOCTitle: Kümeye Sunucu Eklemek için
Title: Kümeye Sunucu Eklemek için
ms:assetid: 'db635238-5528-4bec-9cc6-8244e2b3d733'
ms:contentKeyID: 18125286
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747690(v=WS.10)'
---

Kümeye Sunucu Eklemek için
==========================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Her sunucuda, RMS'yi yalnızca tek bir web sitesi için hazırlayabilirsiniz. RMS'yi varsayılan Web sitesinin dışında bir Web sitesinde hazırlamak istiyorsanız, bu hazırlama işlemine başlamadan önce Web sitesini eklemek için Internet Information Services Yöneticisi'ni kullanın. Hazırlamak istediğiniz Web sitesi Web siteleri listesinde görünmüyorsa, **Genel Yönetim** sayfasını kapatın, Web sitesini ekleyin ve sonra hazırlama işlemini yeniden başlatın.

RMS'yi, Active Directory altyapınızın yerel etki alanı işlevsel düzeyi Windows 2000 yereline ayarlı olduğu bir ortamda dağıtıyorsanız, RMS, grup üyeliğini genişletmeye çalışırken Active Directory nesnelerindeki **memberOf** özniteliğini okuyamayabilir. RMS'nin **memberOf** özniteliğini okumasını sağlamak için RMS hizmet hesabı, ormanınızdaki Pre-Windows 2000-Compatible Access (Yerleşik) grubunun üyesi olan bir etki alanı hesabı kullanmalıdır.

Kümeye Sunucu Ekleme
--------------------

#### Kümeye Sunucu Eklemek için

1.  Kök sertifika veya lisans kümesine eklemek istediğiniz sunucuya RMS yükledikten sonra, **Genel Yönetim** sayfasını açın.

2.  RMS sağlamak istediğiniz Web sitesinin yanındaki **Bu sunucuyu bir kümeye ekle** bağlantısını tıklatın. Varsayılan Web sitesini veya bu amaca yönelik olarak Internet Information Services'ta (IIS) oluşturduğunuz başka bir Web sitesini seçebilirsiniz.

    | ![](/security-updates/images/Cc747690.Warning(WS.10).gif)Uyarý                                                                                                                                                                                                      |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | RMS ile aynı sunucuda ek Web sitesi veya hizmeti çalıştırılması desteklenmez. Bu şekilde hareket edilmesi, RMS ile aynı hesap altında çalışan birden çok uygulamaya ve hizmete neden olabilir. Bu da, özel anahtarları garanti edilmeyen işlemlerle karşı karşıya bırakabilir. |

3.  **RMS hizmet hesabı** alanına, etki\_alanı\_adı\\kullanıcı\_adı biçiminde hesap adını ve RMS'nin birçok normal işlem için altında çalışacağı RMS hizmet hesabının parolasını yazın. Bu bir etki alanı hesabı olmalıdır. Kümedeki tüm sunucular aynı RMS hizmet hesabı altında çalışmalıdır.

    | ![](/security-updates/images/Cc747690.Important(WS.10).gif)Önemli                                                                                                                                                                                                |
    |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Güvenlik nedeniyle, RMS hizmet hesabı olarak kullanmak için özel bir etki alanı kullanıcı hesabı oluşturmanız ve ona herhangi bir özel izin vermemeniz önerilir. RMS hizmet hesabı, Service Pack 1 kurulu RMS yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. |

4.  **Yapılandırma veritabanı** alanında, bu kümeye yönelik veritabanı sunucusunun adını ve yapılandırma veritabanının adını belirtin. Seçtiğiniz veritabanı bu sunucunun ekleneceği kümeyi belirler.

5.  **Özel anahtar koruması** alanında, özel anahtarı korumak için bu küme tarafından kullanılan mekanizmayı seçin. Varsayılan yazılım tabanlı özel anahtar koruması için, bu kümedeki ilk sunucu hazırlandığında özel anahtarı şifrelemek için kullanılan parolayı girin.

6.  **Gönder**'i tıklatın.

    Ekranda hata iletileri görüntülenirse, sayfayı kapatmayın. Bunun yerine, hataları düzeltin, IIS'yi durdurmak ve yeniden başlatmak için IISReset'i kullanın, önceki sayfaya geri gidin, sağlama bilgilerini yeniden girin ve sonra **Gönder** seçeneğini yeniden tıklatın. "İstek zaman aşımına uğradı" hatası alırsanız, pencereyi kapatın, sistemin en düşük donanım gereksinimlerini karşıladığını doğrulayın ve sunucuyu yeniden sağlamayı deneyin.
