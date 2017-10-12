---
TOCTitle: Lisans Sunucusu Sağlamak için
Title: Lisans Sunucusu Sağlamak için
ms:assetid: '4d67b898-0ba9-4eef-ab7d-ee0ca55a688e'
ms:contentKeyID: 18125089
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747563(v=WS.10)'
---

Lisans Sunucusu Sağlamak için
=============================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Ayrıca, alt kayıt işlemi hem kullanıcı hesabı hem de RMS hizmet grubu için okuma ve yürütme izinleri gerektirir. Daha fazla bilgi için bu konuda daha önce yer alan "[Alt Kayıt Hizmeti Dosyasında İzinler Ayarlama](https://technet.microsoft.com/737bb69b-fe26-4057-9569-e632f7bbf295)" bölümüne bakın. Uzak SQL Server veritabanını kullanıyorsanız, oturum açtığınız hesap SQL Server'da Veritabanı Oluşturucuları rolüne de sahip olmalıdır. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Her sunucuda, RMS'yi yalnızca tek bir web sitesi için hazırlayabilirsiniz. RMS'yi varsayılan Web sitesinin dışında bir Web sitesinde hazırlamak istiyorsanız, bu hazırlama işlemine başlamadan önce Web sitesini eklemek için Internet Information Services Yöneticisi'ni kullanın. Hazırlamak istediğiniz Web sitesi Web siteleri listesinde görünmüyorsa, **Genel Yönetim** sayfasını kapatın, Web sitesini ekleyin ve sonra hazırlama işlemini yeniden başlatın.

RMS'yi, Active Directory altyapınızın yerel etki alanı işlevsel düzeyi Windows 2000 yereline ayarlı olduğu bir ortamda dağıtıyorsanız, RMS, grup üyeliğini genişletmeye çalışırken Active Directory nesnelerindeki **memberOf** özniteliğini okuyamayabilir. RMS'nin **memberOf** özniteliğini okumasını sağlamak için RMS hizmet hesabı, ormanınızdaki Windows 2000 Öncesi Uyumlu Erişim (Yerleşik) grubunun üyesi olan bir etki alanı hesabı kullanmalıdır.

Küme için özel bir URL yazarsanız, onu Etki Alanı Adı Sisteminize (DNS) kaydettiğinizden emin olun ve çalıştığını doğrulayın. Bu Internet etkinleştirilmiş bir dağıtımsa, URL'nin hem Internet'ten hem de kuruluşunuzdan kullanılabildiğini doğrulayın. Web hizmeti dosyaları için SSL'yi etkinleştirdiyseniz, küme URL'nize ilişkin HTTPS'yi belirlemelisiniz.

Lisans Sunucusu Sağlama
-----------------------

#### Lisans sunucusu sağlamak için

1.  **Genel Yönetim** sayfasını açın ve sonra Windows RMS sağlamak istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde hazırla**'yı tıklatın.

    Bu amaç için Internet Information Services'ta (IIS) hazırladığınız varsayılan Web sitesini veya başka bir Web sitesini seçebilirsiniz.

    | ![](images/Cc747563.Warning(WS.10).gif)Uyarý                                                                                                                                                                                                      |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | RMS ile aynı sunucuda ek Web sitesi veya hizmeti çalıştırılması desteklenmez. Bu şekilde hareket edilmesi, RMS ile aynı hesap altında çalışan birden çok uygulamaya ve hizmete neden olabilir. Bu da, özel anahtarları garanti edilmeyen işlemlerle karşı karşıya bırakabilir. |

2.  **Yapılandırma veritabanı** alanında, varsayılan seçenek yapılandırma veritabanını yerel sunucuda oluşturmaktır. Yerel veritabanı olarak, SQL Server™ 2000 SP3 veya Microsoft SQL Server 2000 Desktop Engine (MSDE) gibi bir veritabanı sunucusu kullanabilirsiniz. Uzak veritabanı kullanıyorsanız veya veritabanı sunucunuzu yerel sunucuda çalıştırıyorsanız, ancak veritabanı örneği sunucu adından farklı bir ada sahipse, **Uzak veritabanı**'nı seçin ve veritabanı sunucusunun adını girin.

    | ![](images/Cc747563.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Microsoft SQL Server Desktop Engine, herhangi bir ağ arabirimini desteklemediği için, Microsoft SQL Server Desktop Engine'in RMS veritabanlarını yalnızca sınama ortamlarında desteklemek için kullanılması önerilir. Ayrıca, Microsoft SQL Server Desktop Engine'in kullanım koşulları, Microsoft SQL Server Desktop Engine veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınızı belirtir. Bu sınırlama, günlük bilgilerini görüntüleyememenize veya yapılandırma veritabanında saklanan verileri değiştirememenize neden olur. |

3.  **RMS hizmet hesabı** alanında, RMS'nin, normal işlemlerin birçoğu için altında çalışacağı RMS hizmet hesabını belirleyin. Tek sunuculu yükleme için, Local System hesabını veya bir etki alanı hesabı belirleyebilirsiniz. Diğer tüm yüklemeler için bir etki alanı hesabı belirtmelisiniz. Bir etki alanı hesabı için, *etki\_alanı\_adı*\\*kullanıcı\_adı* şeklinde hesap adını ve parolayı verin.

    | ![](images/Cc747563.Warning(WS.10).gif)Uyarý                                                                                                                                                                                                                                                                                                                                                                            |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Local System hesabının işletim sistemindeki hemen hemen tüm kaynaklara erişimi vardır ve dolayısıyla ciddi güvenlik etkileri vardır. Olanak olduğu sürece, Local System hesabını RMS hizmet hesabı olarak kullanmayın. Bunun yerine, RMS hizmet hesabı olarak kullanmak için özel bir etki alanı kullanıcı hesabı oluşturun ve bu hesaba özel izin vermeyin. RMS hizmet hesabı, RMS'yi yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. |

4.  **Küme URL'si** alanına, iç ağdaki istemciler için kullanılacak sunucu veya kümenin URL'sini yazın. Varsayılan girdi sunucu adını kullanır; örneğin Contoso-cert. Bunu gereken şekilde düzenleyebilirsiniz, örneğin küme veya kümeye hizmet eden yük dengeleyici için bir URL yapılandırmak amacıyla. HTTP veya HTTPS'yi de seçebilirsiniz. Küme URL'sini yapılandırma hakkında daha fazla bilgi için bu yordam listesinin sonundaki **Notlar** bölümüne bakın. Sağlama işleminden sonra, iç ağınızın dışındaki istemcilerin kullanması için yönetim Web sayfalarından bir dış küme URL'si yapılandırabilirsiniz.

5.  **Özel anahtar koruması ve alt kayıt** alanında, aşağıdakilerden birini yaparak sunucu özel anahtarını koruma mekanizmasını seçin:

    -   **Varsayılan yazılım tabanlı özel anahtar korumasını kullan**. Bu seçeneği seçerseniz, özel anahtar RMS yapılandırma veritabanında depolanır. Anahtarı veritabanında şifrelemek için sağlam bir parola vermelisiniz.

    | ![](images/Cc747563.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                                                                  |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Bu parolayı ileride kullanmak için güvenli bir arşivde saklayın. Güvenli arşivde yapılandırma veritabanının yedek kopyasını depolayın (bu parolayla güvence altına alınır). Böylece, SQL Server veritabanı bozulursa RMS'yi geri yüklemek için bir mekanizmaya sahip olursunuz. Herhangi bir nedenle parolayı değiştirirseniz, o parolaya anahtarlanan yapılandırma veritabanının yeni bir yedeğini yapın ve sonra her ikisini de güvenli arşive yerleştirin. |

    -   **Şifreleme hizmet sağlayıcısı (CSP) kullanın**. CSP veya donanım güvenlik modülü (HSM) kullanmak için, **Varsayılan yazılım tabanlı özel anahtar korumasını kullan** onay kutusunu temizleyin. **Şifreleme hizmet sağlayıcınızı seçin** listesinde, yüklediğiniz CSP veya HSM'yi seçin.

    | ![](images/Cc747563.note(WS.10).gif)Not                                           |
    |----------------------------------------------------------------------------------------------------------------|
    | RMS, tam Rivest-Shamir-Adleman (RSA) sağlayıcısı gerektirir; yalnızca bu sağlayıcılar CSP listesinde yer alır. |

    | ![](images/Cc747563.note(WS.10).gif)Not                                                                                                                                                                                                                              |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Varsayılan yazılım tabanlı özel anahtar korumasını veya HSM'yi kullanmanız önerilir. Farklı bir yazılım tabanlı CSP kullanıyorsanız, RMS ile kullanmadan önce o CSP'nin yerine kurumsal anahtar yönetimi uygulamalarına (yedekleme ve geri yükleme yordamları gibi) sahip olduğunuzdan emin olun. |

6.  Bu adım yalnızca CSP seçtiyseniz uygulanır. Kullanılacak sunucu anahtarı çiftini belirlemek için aşağıdakilerden birini yapın:

    -   Yeni bir yükleme için, **Yeni ortak/özel anahtar çifti oluştur**'u seçin.
    -   Varolan RMS sunucusunu kurtarıyor veya ondan yükseltme yapıyorsanız, **Varolan ortak/özel anahtar çiftini kullan**'ı seçin. Varolan anahtar kapsayıcısı altında, **Gözat**'ı tıklatın ve sonra sunucu anahtar çiftinin anahtar kapsayıcısını seçin.

    | ![](images/Cc747563.note(WS.10).gif)Not                  |
    |---------------------------------------------------------------------------------------|
    | Microsoft Taban, Daha İleri ve Güçlü CSP'ler aynı anahtar depolama konumunu paylaşır. |

    | ![](images/Cc747563.note(WS.10).gif)Not                                                                                                                                                                                                                                                          |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Varolan RMS sunucusunu kurtarırken veya yükseltirken varolan bir anahtar çifti kullanmıyorsanız, varolan tüm RMS istemcilerin lisans depolarının temizlenmesi (kullanım lisansları ve hak hesabı sertifikaları silinir) gerekir. Daha sonra, içeriği kullanabilmek için istemcilerin sunucudan yeni lisanslar alması gerekir. |

7.  **Sunucu lisans sertifikası adı**'nda, sunucu lisans sertifikasında kullanılmak üzere bir ad girin. Varsayılan olarak, bu, sunucunun adıdır.

8.  Kuruluşunuz Internet'e bağlanmak için proxy sunucusu kullanıyorsa, **Bu bilgisayar Internet'e bağlanmak için proxy sunucusu kullanıyor** onay kutusunu seçin ve sonra proxy sunucusunun adresini ve bağlantı noktasını yazın.

    Proxy sunucusu kimlik doğrulama gerektiriyorsa, kimlik doğrulama türünü seçin ve proxy sunucusu tarafından kimliği doğrulanabilecek bir kullanıcı adı ve parolası sağlayın. Tümleşik Windows kimlik doğrulaması kullanıyorsanız bir etki alanı da belirtmelisiniz.

9.  **Gönder**'i tıklatın.

    RMS alt kayıt hizmeti, lisans sunucusu için ortak/özel anahtar çifti oluşturur ve ortak anahtarı kök sertifika sunucusu özel anahtarıyla imzalar. Ayrıca lisans sunucusu için sunucu lisans sertifikası oluşturur. Bu öğeleri birkaç dakika içinde yapılandırma veritabanına gönderir.

    | ![](images/Cc747563.Important(WS.10).gif)Önemli                                                                                                                                                                                                                                                                                                                                                                           |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Ekranda hata iletileri görüntülenirse, sayfayı kapatmayın. Bunun yerine, hataları düzeltin, IIS'yi durdurmak ve yeniden başlatmak için IISReset'i kullanın, önceki sayfaya geri gidin, sağlama bilgilerini yeniden girin ve sonra **Gönder** seçeneğini yeniden tıklatın. "İstek zaman aşımına uğradı" hatası alırsanız, pencereyi kapatın, sistemin en düşük donanım gereksinimlerini karşıladığını doğrulayın ve sunucuyu yeniden sağlamayı deneyin. |

Ek lisans sunucuları sağlama ve kümeye eklemeyle ilgili yönergeler için, bu konuda daha sonra yer alan "[Kümeye Sunucu Eklemek için](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)" bölümüne bakın.
