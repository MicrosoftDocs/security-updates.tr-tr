---
TOCTitle: Hak İlkesi Şablonlarının Konumunu Belirtmek için
Title: Hak İlkesi Şablonlarının Konumunu Belirtmek için
ms:assetid: 'e1bee46d-33db-424f-ba45-1dcedcb883ab'
ms:contentKeyID: 18125297
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747781(v=WS.10)'
---

Hak İlkesi Şablonlarının Konumunu Belirtmek için
================================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Hak ilkesi şablonlarını paylaşılan klasörde depolar ve sonra paylaşılan klasörün konumunu değiştirirseniz, hak ilkesi şablonlarını önceki konumdan yeni konuma el ile kopyalamanız gerekir.

Hak ilkesi şablonları da yapılandırma veritabanında depolanır. Hak ilkesi şablonlarının dağıtılması hakkında daha fazla bilgi için bkz: "[Hak İlkesi Şablonlarını Dağıtma](https://technet.microsoft.com/ae6fa26f-d744-4ac9-9eb1-728ffab87bfe)".

RMS etkin uygulama olarak Microsoft Office 2003 kullanıyorsanız, hak ilkesi şablonlarının konumu `AdminTemplatePath` kayıt defteri anahtarı ile denetlenir ve RMS istemcisi, şablonları kayıt defteri anahtarında belirtilen konumda bulmaya çalışır.

Hak İlkesi Şablonlarının Konumunu Belirtme
------------------------------------------

#### Hak İlkesi Şablonlarının Konumunu Belirtmek için

1.  **Genel Yönetim** sayfasını açın ve sonra hak ilkesi şablonlarının konumunu belirtmek istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Hak ilkesi şablonları**'nı tıklatın.

3.  **Şablon konumu** alanında, bu küme için hak ilkesi şablonlarını depoladığınız paylaşılan klasörün Evrensel Adlandırma Kuralı'nı (UNC), \\\\*sunucu\_adı*\\*paylaşım\_adı* biçiminde belirtin. **Admin** uygulama havuzunu çalıştıran hesabın paylaşılan klasörde Yazma iznine sahip olması gerekir. Şablonlarınızın, kuruluşun güvenlik kurallarına uygun bir ağdan erişilebilir konumunda depolandığından emin olun. Şablonlar için paylaşılan klasörler RMS tarafından kullanılan Program Dosyaları klasörü veya IISRoot klasörleri gibi temel klasörlerde oluşturulmamalıdır.

4.  **Kaydet**'i tıklatın.

5.  Hak ilkesi şablonlarını oluşturduktan ve bu konuma kaydettikten sonra, kullanıcıların kullanımına sunulması gerekir. Varsayılan olarak, RMS istemcisi yerel bilgisayarda bulunan aşağıdaki konumda hak ilkesi şablonlarını arayacaktır.

    %HOMEPATH%\\Local Settings\\Application Data\\Microsoft\\DRM\\templates

    Hak ilkesi şablonları, kuruluştaki RM kullanacak olan tüm kullanıcılar için 3. adımda belirtilen konumdan bu konuma kopyalanmalıdır.
