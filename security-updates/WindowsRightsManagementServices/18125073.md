---
TOCTitle: Hizmet Bağlantı Noktasını Kaydetme
Title: Hizmet Bağlantı Noktasını Kaydetme
ms:assetid: '446d83ec-3224-45e2-9697-625e7db338f3'
ms:contentKeyID: 18125073
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720260(v=WS.10)'
---

Hizmet Bağlantı Noktasını Kaydetme
==================================

RMS'ye ait hizmet bağlantı noktası (SCP), kuruluşunuzda bulunan RMS etkin istemciler için hizmet bağlantı URL'sini tanımlar. İstemciler, geçerli bir SCP olmadan kullanım lisansı, yayımlama lisansı veya hak hesabı sertifikası istemek için RMS'yi bulamayacaktır.

Yönetim Web sitesindeki RMS **Hizmet Bağlantı Noktası** sayfasından kök sertifika kümeniz için SCP URL'sini kaydettirebilirsiniz. URL'yi herhangi bir nedenden dolayı sıfırlama gereksinimi duyarsanız, SCP URL'sinin kaydını **Hizmet Bağlantı Noktası** sayfasından da silebilirsiniz. SCP URL'sini kaydettirmek veya URL'nin kaydını silmek için, Hizmetler kapsayıcısının altında bir kapsayıcı nesnesi oluşturmak üzere yeterli ayrıcalıklara sahip, geçerli bir etki alanı kullanıcı hesabıyla oturum açmanız gerekir.

Active Directory'de bulunan hizmetler kapsayıcısı altında, "RightsManagementServices" adlı yeni bir kapsayıcı nesnesi oluşturulacaktır. Bu kapsayıcı altında, "MSRMRootCluster" adlı bir SCP nesnesi oluşturulacaktır. Bu SCP nesnesi keywords özniteliği için iki değere sahiptir:

-   MSRMRootCluster
-   1.0

Bunlar, Active Directory'deki kök kümesi URL'sini bulmak üzere istemciler ve diğer sunucular tarafından kullanılan özniteliklerdir. SCP nesnesinde bulunan serviceBindingInformation, http://*kümeadı*/\_wmcs/Certification biçiminde kök küme URL'sini içerecektir.
