---
TOCTitle: Sunucu Lisans Sertifikalarını İptal Etme
Title: Sunucu Lisans Sertifikalarını İptal Etme
ms:assetid: '8020861d-d196-4431-8282-044675ef5616'
ms:contentKeyID: 18125174
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747578(v=WS.10)'
---

Sunucu Lisans Sertifikalarını İptal Etme
========================================

Kuruluşun, RMS sunucusunu kuşkulu kılacak öngörülmeyen durumlar nedeniyle bir sunucu lisans sertifikasını iptal etmesi gerekebilir. Donanım güvenlik modülünde saklamadığınız özel bir anahtar çalınma tehlikesine açıktır. Sunucunun denetimini eline geçiren kötü niyetli bir saldırgan yüzünden kuruluştaki bir sunucu lisans sertifikası ve anahtar güvenilmez hale gelebilir veya küskün bir çalışan sertifikayı veya anahtarı kopyalayabilir ya da silebilir. İptal, kötü niyetli kullanıcının yol açtığı hasarı önlemenin ve kötüye kullanımını sınırlamanın bir yoludur.

Varsayılan olarak, tüm lisanslar veya sertifikalar bunları veren asıl öğe tarafından iptal edilebilir. Korumalı içeriğinizle ilişkili lisansları ve sertifikaları RMS sunucuları verdiği için, gerektiğinde bu sertifika ve lisansları her zaman iptal edebilirsiniz. Bir lisans sunucusu kuşkulu durumdaysa, sunucunun lisans sertifikasını iptal edebilirsiniz. Sunucu lisans sertifikasını iptal ettiğiniz zaman, sunucunun yayınladığı tüm sertifikalar ve lisanslar geçersiz olur. Lisans ve sertifika iptaliyle ilgili yönergeler bu konuda daha önce geçen "[İptal Uygulama](https://technet.microsoft.com/4735f060-7197-4ae2-830a-f91bcc4de30a)" bölümünde verilmiştir.

Bununla birlikte, kök sertifika sunucusu özel bir durum oluşturur. Kök sertifika kümesi sunucu lisans sertifikası, Microsoft Kayıt Hizmeti tarafından verilir ve varsayılan olarak sunucu lisans sertifikasını yalnızca Microsoft Kayıt Hizmeti iptal edebilir.

Microsoft, bir kök sertifika sunucu lisans sertifikasını yalnızca mahkeme kararı çıkartmanız ve sunucunun ortak anahtarını mahkemeye sunmanız durumunda iptal edebilir. Mahkeme Microsoft'a iptal emrinin çıkarıldığını bildirdikten sonra, Microsoft sunucu lisans sertifikasını ortak anahtarıyla iptal listesinde belirtir ve listeyi genel kullanıma açar. Lisansı iptal edilmesi gereken sunucuyla ilgili olarak aşağıdaki koşullardan biri söz konusuysa, mahkemeden iptal emri isteyebilirsiniz:

-   Sahibi olduğunuz sunucu ve özel anahtarı kuşkulu durumdadır.
-   Sunucunun yayımladığı içeriğin sahibisinizdir ve içerik telif hakkınızı ihlal ederek yayımlanmaktadır.

Kök sertifika sunucusunun iptal edilen sunucu lisans sertifikasının bulunduğu Microsoft iptal listelerini almak ve dağıtmak için, bu bölümde daha önce geçen "[İptal Listelerini Dağıtma](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)" konusunda açıklanan adımları izleyin.

Kök sertifika sunucusunu hazırlarken, kök sertifika kümesinin sunucu lisans sertifikasını iptal etme yetkisine sahip bir ortak anahtar belirleyebilirsiniz. Bu ortak anahtar kuruluşa veya bir üçüncü partiye ait olabilir. İlgili özel anahtarın imzaladığı iptal listesi sunucu lisans sahibi sertifikasını iptal edebilir.

Kök sertifika sunucusunun sunucu lisans sertifikasını iptal etmek için, bu sunucu lisans sahibi sertifikasını belirten bir iptal listesi oluşturup kuruluşunuzun veya üçüncü tarafın özel anahtarıyla imzalayabilir ve bu iptal listesini tüm kullanıcılara dağıtabilirsiniz. Yönergeler için, bu konuda daha önce geçen “Kuruluş İptal Listelerini Dağıtma” kısmındaki “[İptal Listelerini Dağıtma](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)” bölümüne bakın.

İptal listesindeki bir sunucu lisans sertifikasını aşağıdaki parametreleri kullanarak iptal edebilirsiniz:

-   **GUID**. Bir sunucu lisans sertifikası genel benzersiz tanımlayıcısına (GUID) göre iptal edilebilir. Bu parametreyi iptal listesinde kullanma hakkında bilgi için, bu konuda daha önce geçen "Sertifikaları ve Lisansları GUID'ye Göre İptal Etme" kısmındaki "[İptal Listeleri Oluşturma](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)" bölümüne bakın.
-   **Karma değeri**. Sunucu lisans sertifikası, yapısındaki SHA-1 Unicode karakter karmasına göre iptal edilebilir. Bu parametreyi iptal listesinde kullanma hakkında bilgi için, bu konuda daha önce geçen "Sertifikaları ve Lisansları Karma Değerine Göre İptal Etme" kısmındaki "[İptal Listeleri Oluşturma](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)" bölümüne bakın.

Bir RMS yüklemesinin sunucu lisans sertifikasını almak için RMS yapılandırma veritabanını sorgulamanız gerekir. Aşağıdaki adımlarda, bir SQL yapılandırma veritabanından bu bilgilerin nasıl alınacağı ve tarayıcı ile rahatlıkla okunabilecek bir dosyaya nasıl kaydedileceği açıklanmaktadır:

1.  SQL Query Analyzer'ı açıp kök sertifika sunucusunun yapılandırma veritabanına bağlanın.
2.  **Sorgu** menüsünde **Metindeki Sonuçlar** seçeneğini tıklatın.
3.  **Araçlar** menüsünde, **Seçenekler** iletişim kutusunu açmak için **Seçenekler** seçeneğini tıklatın. **Sonuçlar** sekmesini tıklatın ve **Sütun başına en fazla karakter** seçeneğini **8192** yapın.
        ```
1.  **Sonuçlar** penceresinden sonuçları kopyalayıp, Not Defteri gibi bir metin düzenleyiciye yapıştırın. Sonuçları .xml dosya adı uzantılı bir dosyaya kaydedin.

Bu bilgilerin iptal listesinde nasıl kullanıldığı hakkında daha fazla bilgi için bkz: "[İptal Listeleri Oluşturma](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)".

Sunucu lisans sahibi sertifikası bilgilerini XML dosyası olarak kaydettikten sonra, sertifikadan ortak anahtarı aşağıdaki adımları izleyerek ayıklayabilirsiniz:

1.  Sunucu lisans sertifikası XML dosyasını bir XML veya metin dosyası düzenleyicide açın.
2.  &lt;ISSUEDPRINCIPALS&gt; bölümünde &lt;PUBLICKEY&gt;öğesini kopyalayın.
3.  Bu bilgileri mahkemeye veya kuruluşa ait iptal listesindeki bir yere gönderebileceğiniz bir dosyaya kaydedin.

Kök sertifika sunucu kümesinin sunucu lisans sertifikası iptal edildikten sonra, RMS yüklemesinin verdiği tüm sertifikalar ve lisanslar, iptal listesi gerektiren içerik için geçersiz olur ve içerik erişilemez duruma gelir. Bu işlem, kullanıcının sahip olduğu lisansın türünden etkilenmez. Lisansı iptal edilen sunucunun yayımladığı içeriği korumak için, iptal listesini uygulamaya koymadan önce aşağıdaki önlemlerden birini almanız gerekir:

-   İçeriği RMS koruması olmadan kaydetmek.
-   İçeriği iptal listesi gerekliliği olmaksızın yeniden yayımlamak.

Her iki senaryoda da (Microsoft'uniptal etmesi veya üçüncü tarafın iptal etmesi), iptal listesi, kullanım lisansının güven zincirindeki bir yetkilinin özel anahtarıyla imzalandığından, tüm bağlantı istekleri için geçerli olur. Bu nedenle, RMS yüklemesinin iptal edilen sunucu lisans sertifikasını kullanarak verdiği lisansları kapsayan tüm bağlama istekleri başarısız olur.

| ![](/security-updates/images/Cc747578.note(WS.10).gif)Not                                      |
|-----------------------------------------------------------------------------------------------------------|
| Microsoft, sunucu lisans sahibi sertifikasını yalnızca mahkeme kararı gerektirdiği zaman iptal edecektir. |
