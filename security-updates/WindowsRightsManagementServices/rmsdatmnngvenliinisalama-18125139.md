---
TOCTitle: RMS Dağıtımının Güvenliğini Sağlama
Title: RMS Dağıtımının Güvenliğini Sağlama
ms:assetid: '6de8b636-a824-4844-aefc-f26347abfc14'
ms:contentKeyID: 18125139
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720291(v=WS.10)'
---

RMS Dağıtımının Güvenliğini Sağlama
===================================

RMS dağıtımı, kuruluşların altyapılarında bulunan diğer kritik sunucularla aynı fiziksel ve ağ güvenliğine yönelik önlemleri gerektiren önemli bir değerdir. Dağıtımın bir parçası olarak, tehditleri ve bunlara yönelik olarak RMS sunucularında uygulanacak önlemleri tanımlamalısınız.

RMS bir Web hizmeti olarak uygulandığından, RMS erişimini, erişim denetim listelerini ve güvenli yuva katmanını kullanarak diğer Web hizmetleriyle aynı biçimde denetleyebilirsiniz.

**ACL Kullanarak RMS Web Hizmetlerine Erişimi Kısıtlama**

RMS hizmetlerine erişimi, erişim denetim listelerini kullanarak kısıtlayabilirsiniz. RMS bir Web sitesinde yapılandırıldığında oluşturulan her bir sanal kök dizine karşılık gelen klasör yapısının güvenliği sağlanabilir. Klasör yapısı, varsayılan olarak &lt;sistem sürücüsü&gt;:\\&lt;*web\_kök\_klasörü*&gt;\\\_wmcs altında bulunur; burada *web\_kök\_klasörü*, RMS'nin sağlandığı Web sitesine atanan klasörün adıdır. Alt kayıt hizmeti, mobil aygıt sertifika hizmeti ve sunucu hizmet sertifikası hizmeti gibi bazı Web hizmetleri varsayılan olarak kısıtlanır ve hizmeti kullanma olanağı vermek istediğiniz kullanıcı veya grupların, erişim denetim listesine açıkça eklenmesi gerekir.

Sunucu hizmet sertifikası hizmeti, RMS sisteminin uzantısını desteklemek amacıyla Web birlikte çalışma hizmetleri, posta sunucuları ve belge yönetimi sunucuları gibi hizmetler tarafından RMS korumalı içeriğe erişmek için kullanılabilecek hak hesabı sertifikaları (RAC) sağlar. Aşağıda ilgili örnekler yer almaktadır:

-   Kullanıcıların, korumasız belgeleri karşıya yükleyebildiği, ancak karşıdan yüklenen belgelere otomatik olarak içerik türünün hak ilkesine uygun bir RMS korumasının uygulandığı bir belge birlikte çalışma sunucusu. Buna örnek olarak Microsoft Office SharePoint Server 2007 gösterilebilir.
-   Korumalı ve korumasız biçimde, genel bir havuz ve belge arşivi işlevi gören bir belge yönetim sistemi. Sistem, haklarla korunan belgeleri aramak için dizin oluşturabilir ve bunu içerik oluşturucu tarafından tanımlanan hak ilkesini koruyarak gerçekleştirir.
-   Posta sunucusunun, haklarla korunan içeriği, virüsler ve istenmeyen postalar açısından ya da şirketin posta ilkesine veya bir yasal gereksinim şartına uygun şekilde incelemek için hızlı bir şekilde açmasını sağlar.

Bu senaryolarda kullanıcılar adına lisanslar istendiği için, kuruluşunuzda hizmet RAC'si alabilecek sunucuları, bu tür bir işlev üstlenmesi onaylanmış ve güvenliği doğru şekilde sağlanmış sunucularla kısıtlamış olduğunuzdan emin olmalısınız.

**SSL Kullanarak RMS Web Hizmetlerine Erişimi Kısıtlama**

Güvenli Yuva Katmanı'nı (SSL) etkinleştirmeniz ve tüm RMS Web hizmetleri dosyalarında 128 bit şifreleme istemeniz önerilir. Bu dosyaların dosya adı uzantısı .asmx şeklindedir ve Licensing, Certification ve Admin sanal dizinlerinde bulunurlar. SSL, sunucunuzda Web sitesi için yüklenmiş geçerli bir SSL sertifikası olmasını gerektirir. SSL'yi RMS yüklemesinin \_wmcs klasörüne uygularsanız, alt klasörler ve dosyalar da bu ayarı devralır. Web hizmetleri dosyaları ve sanal dizinler hakkında daha fazla bilgi için, bu belge grubundaki "RMS: Teknik Başvuru Kılavuzu" bölümünde bulunan "Internet Information Services" konusuna bakın.

| ![](images/Cc720291.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Windows RMS Yönetimi Web sayfalarını uzak bilgisayardaki bir tarayıcıdan açmak istiyorsanız, SSL'yi etkinleştirmelisiniz. Ancak, SSL etkinleştirilse bile, **Genel Yönetim** sayfasını uzak bilgisayardan açamazsınız. RMS'nin uzaktan yönetimi hakkında daha fazla bilgi için, bu belge grubunda bulunan "RMS: İşlemler" bölümündeki "Yönetim Giriş Sayfasını Kullanma" konusuna bakın. |

**Güçlü Bir Özel Parola Anahtarı Ayarlama**

Özel anahtar parolası, özel anahtarı oluşturmak ve RMS yapılandırma veritabanında güvenli şekilde depolamak için kullanılır. Üst düzeyde güvenlik için bir güçlü parola kullanılması önerilir. Parolanın not alınması gerekiyorsa, bu parolanın fiziksel olarak güvenli bir yerde saklandığından emin olun.

| ![](images/Cc720291.Caution(WS.10).gif)Dikkat                                                                                                                                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Özel anahtar parolası kaybolursa veya bilinmiyorsa ve RMS sunucusu beklenmedik biçimde çevrimdışı duruma geçerse, tüm RMS belgelerinin şifrelerini kaldırmanız, RMS ortamınızı yeniden oluşturmanız ve tüm öğeleri yeni özel anahtar ile yeniden şifrelemeniz gerekir. |
