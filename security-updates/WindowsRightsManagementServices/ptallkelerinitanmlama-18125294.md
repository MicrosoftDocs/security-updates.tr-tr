---
TOCTitle: İptal İlkelerini Tanımlama
Title: İptal İlkelerini Tanımlama
ms:assetid: 'e2fffe9f-def7-439b-a8aa-43f8a065813d'
ms:contentKeyID: 18125294
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747782(v=WS.10)'
---

İptal İlkelerini Tanımlama
==========================

İptal işleminin uygulanması korumalı içerik için daha güçlü güvenlik sağlamasına rağmen, kuruluş iptal ilkelerini tanımlamak, kullanıcının içeriği kullanma yetisini etkileyebileceğinden dikkatli bir değerlendirme ve planlama gerektirir. RMS dağıtımının iptal ilkeleri yönetim Web sitesinden tanımlanabilir.

Üçüncü Parti İptali
-------------------

Microsoft Kayıt Hizmeti RMS dağıtımınız için kök sertifika sunucusunun sunucu lisans sertifikasını verdiğinden, Microsoft sunucu lisans sertifikanızı iptal edebilir. Bununla birlikte, Microsoft sunucu lisans sertifikasını yalnızca mahkeme kararı gerektirdiği zaman iptal edecektir.

Microsoft Kayıt Hizmeti'ne ek olarak, bir RMS sunucunuzun sunucu lisans sertifikasını iptal edebilecek bir üçüncü parti belirleyebilirsiniz. Bu üçüncü parti dışarıdan bir varlık veya yöneticinin kuruluş adına üreteceği ortak ya da özel bir anahtar çifti olabilir. Belirtilen üçüncü parti özel anahtarı, sunucu lisans sahibi sertifikasını iptal eden bir iptal listesi imzalayabilir. Bu üçüncü parti, RMS hazırlık sürecinde ortak anahtarıyla belirtilir. Sunucunuzun hak ilkesi şablonları da, üçüncü partilere RMS yüklemenizin yayınladığı içeriği, uygulama bildirimlerini, lisansları ve sertifikaları iptal etme izni verecek biçimde yapılandırılabilir. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.

| ![](images/Cc747782.Important(WS.10).gif)Önemli                                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kök sertifika sunucusunun sunucu lisans sahibi sertifikasını iptal etmede kullanmak için kendi anahtar çiftinizi üretmeye karar verirseniz, bu anahtar çiftini güvenli bir yerde sakladığınızdan emin olun. |

Sunucu lisans sahibi sertifikasının iptali, RMS yüklemenizin yayınladığı tüm sertifika ve lisanslar bu sertifikanın iptaliyle geçersiz olacağı için önemli bir karardır. Sunucu lisans sertifikalarını iptal etme hakkında daha fazla bilgi için bu konuda daha sonra yer alan "[Sunucu Lisans Sertifikalarını İptal Etme](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)" bölümüne bakın.

İptal Listelerinin Etkisini Dikkate Alma
----------------------------------------

Bir korumalı içerik bölümü için iptal gerektiğinde, istemci bilgisayarlarda kayıtlı olan tüm iptal listeleri kullanılacak ve belirtilen bir koşulla karşılaşıldığında yürürlüğe girecektir. Bu nedenle, iptal işlemi uygularken, bu uygulama iptal listelerinin istemci bilgisayarlara kaydedilmesine ve bu listelerin istediğinizden daha geniş bir biçimde uygulanabilmesine yol açacağı için sağduyunuzu kullanın. Bu seçeneği yapılandırma hakkında daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.

Güvenlik ve Kullanılabilirliği Dengeleme
----------------------------------------

Bir hak ilkesi şablonunda iptal ilkesi belirlerken, yukarıdaki örnekte açıklandığı gibi, kullanıcıların içeriği kullanırken sorunlarla karşılaşmaları olasılığına karşı belgeler için daha geniş güvenlik sağlama gerekliliğini göz önüne alın.

Bir hak ilkesi şablonunda iptal listesi ayarları belirlemenin bir parçası olarak, iptal listesi için bir yenileme aralığı da belirtirsiniz. Bu hak ilkesi şablonunu kullanarak yayımlanan içeriği kullanmak için, kullanıcının bilgisayarında bir iptal listesi olması ve listenin belirtilen yenileme aralığından daha eski olmaması gerekir. Örneğin yenileme aralığı 10 ise, iptal listesinin son 10 gün içinde oluşturulmuş olması gerekir. İptal listesi istemci bilgisayarında yoksa veya listenin oluşturulma tarihi yenileme aralığından eskiyse, RMS etkin uygulama, kullanım lisansında belirttiğiniz konumdan en son iptal listesini alır. Ancak, ağa bağlı olmayan bir kullanıcı geçerli iptal listesini alamaz ve bu nedenle içeriği kullanamaz.

Aşağıdaki öneriler bu sorunun çözümüne yardımcı olabilir:

-   İptal listesi yenileme aralığını belirtirken dikkatli olun ve mutlaka kullanıcıların erişimine hazır güncel bir iptal listesinin bulunduğundan emin olun.
-   İptal listelerini şirket ağının içinden ve dışından erişilebilen URL'lerde tutun.
-   İptal listelerinin güncel kopyalarını belirli bir aralıkta, örneğin her gece, her istemci bilgisayara dağıtmak için Microsoft® Systems Management Server (SMS) veya benzeri bir mekanizma kullanın.
-   Yalnızca en gizli belge türleri için iptal isteyin.
