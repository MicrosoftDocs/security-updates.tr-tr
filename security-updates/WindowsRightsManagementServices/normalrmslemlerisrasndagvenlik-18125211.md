---
TOCTitle: Normal RMS İşlemleri Sırasında Güvenlik
Title: Normal RMS İşlemleri Sırasında Güvenlik
ms:assetid: '98f3d584-6320-4aa1-9959-7133cfdb6df7'
ms:contentKeyID: 18125211
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747609(v=WS.10)'
---

Normal RMS İşlemleri Sırasında Güvenlik
=======================================

RMS'yi yükleyip yapılandırmanızdan sonra, RMS Web hizmetleri IIS uygulamaları gibi çalışarak kimlik doğrulama ve yetkilendirme gerektiren çeşitli sistem kaynaklarına erişir. Tüm sistem kaynakları kimlik doğrulama gerektirir ve aksi şekilde yapılandırılamaz. Bu sayfanın kalan kısmında RMS'de yetkilendirme tasarımı açıklanmaktadır.

RMS Web hizmetleri IIS uygulama havuzu bağlamında çalışır. IIS'teki her uygulama havuzu, bir etki alanı kullanıcı hesabı, yerel kullanıcı hesabı, Ağ Hizmeti yerel hesabı veya Yerel Sistem yerel hesabına karşılık gelebilen benzersiz bir kimliğe sahiptir. Bu hesapların her biri, sistem içinde çeşitli derecelerde yetkilere sahiptir. RMS sağlandığında, RMS Web hizmetlerini, Yerel Sistem hesabı veya etki alanı kullanıcı hesabı olarak çalıştırmayı seçebilirsiniz. Bu hesap daha sonra RMS uygulama havuzu için uygulama havuzu kimliği olur. Genel Yönetim Web sitesinin uygulama havuzu "DRMS Uygulama Havuzu"dur. Sağladığınız Web sitesinin uygulama havuzu "\_DRMSAppPool1" olarak adlandırılır. RMS Günlük Hizmeti, RMS uygulama havuzu kimliği için belirtilen hesabın altında ayrı bir Windows hizmeti olarak çalışır.

RMS Web hizmetlerinin erişmesi gereken kaynaklar arasında sistemdeki çeşitli dosyalar ve klasörler, veritabanı sunucusundaki veritabanları ve saklı yordamlar, yerel kayıt defteri, Active Directory, derleme önbelleği, bellek ve sistemde çalışan diğer işlemler bulunur. RMS Günlük Hizmeti'nin de yerel sistemdeki günlük sırasına erişmesi gerekir. Bu kaynakların her biri, kaynağa erişim yetkisi olan ve kaynakla ne yapılabileceğini tanımlayan kendi DACL'sine sahiptir.

İzin atama ve hizmet hesaplarını yönetmeyi basitleştirmek için, gerekin tüm izinler RMS'nin sağlama işlemi sırasında oluşturduğu yerel RMS Service Group grubuna atanır. RMS hizmet hesabı bu grubun üyesi olduğundan, gruba atanan tüm izinleri alır.

Aşağıdaki listede Windows RMS Service Group'a verilen izinler özetlenmektedir:

-   Sanal kök dizinlerini Okuma izni
-   Derleme önbelleği dizinine Yazma izni
-   Sistem geçici dizinine Yazma izni
-   Günlük sırasına Yazma izni
-   Active Directory'de Okuma izni

Veritabanı sunucusu olarak Microsoft SQL Server 2000 kullanıyorsanız, bunun Windows Server 2003'tekinden biraz farklı bir izin atama yöntemi kullandığına dikkat etmelisiniz. RMS sağlama işlemi, SQL Server'da RMS hizmet hesabı için bir oturum açma hesabı oluşturur. RMS'yi Yerel Sistem hesabını kullanarak sağlamayı seçtiyseniz, SQL Server oturum açma hesabı *ETKİ\_ALANI\\bilgisayar\_adı* biçimi kullanılarak oluşturulur; burada, *ETKİ\_ALANI* bilgisayarın üyesi olduğu Active Directory etki alanının adıdır, *bilgisayar\_adı* ise sunucunun adıdır. rms\_service adlı bir SQL rolü oluşturulur ve gerekli tüm izinler atanır. RMS hizmet hesabı için oturum açma hesabı bu gruba eklenir. RMS hizmet hesabına açık olarak hiçbir izin verilmez.

Ayrıca SQL Server her veritabanına bir veritabanı sahibi (DBO) atar. Sağlama sırasında veritabanı sahipliği aşağıdaki gibi atanır:

-   Yapılandırma veritabanının DBO'su RMS'yi sağlamak için kullanılan etki alanı hesabına verilir.
-   Dizin Hizmetleri'nin ve Günlük veritabanlarının DBO'su RMS hizmet hesabına verilir

RMS tarafından oluşturulan tüm kaynakların izinleri, RMS'nin tasarımı sırasında güvenlik göz önünde bulundurularak dikkatle seçilmiştir. Herhangi bir kaynağın sağlanması sırasında atanan izinleri değiştirmek için neden olmamalıdır. Sağlamadan sonra hizmet hesabının kullanıcı hesabını veya parolasını değiştirmeniz gerekirse, bu işlemi RMS Genel Yönetimi Web sayfasından yapabilirsiniz. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "RMS Hizmet Hesabını Değiştirmek İçin" konusuna bakın.
