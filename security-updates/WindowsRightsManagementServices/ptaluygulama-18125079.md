---
TOCTitle: İptal Uygulama
Title: İptal Uygulama
ms:assetid: '4735f060-7197-4ae2-830a-f91bcc4de30a'
ms:contentKeyID: 18125079
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747554(v=WS.10)'
---

İptal Uygulama
==============

Sertifikalar ve lisanslar, güven zincirlerinde bulunan herhangi bir asıl öğe tarafından iptal edilebilir. Bir kök sertifika sunucusu tarafından yayınlanan herhangi bir sertifika veya lisans, o kök sertifika sunucusu tarafından iptal edilebilir. Ayrıca, sertifikalar RMS yöneticisinin seçtiği bir üçüncü parti tarafından iptal edilebilir.

RMS sunucunuzun verdiği bir sertifika veya lisansı iptal etmek için, aşağıdaki adımlarda açıklandığı şekilde bir iptal listesi oluşturup dağıtabilir ve listeyi bir hak ilkesi şablonunda isteyebilirsiniz.

1.  İptal edilecek asıl adların belirtildiği bir iptal listesi oluşturun. Bu, XrML sözcük dağarcığına uygun, XML biçiminde düz bir metin dosyasıdır. Daha fazla bilgi için bu konuda daha sonra yer alan "[İptal Listeleri Oluşturma](https://technet.microsoft.com/1ef75199-3344-4225-84de-a863a777696a)" bölümüne bakın.
2.  İptal listesi için bir anahtar çifti üretin. Ardından, dosyayı bu amaç için sağlanmış olan İptal Listesi İmzalama aracını kullanarak özel anahtarla imzalayın. Yönergeler için bu konuda daha sonra yer alan "İptal Listesine İmza Ekleme" bölümüne bakın. Bu süreci düzenli, tercihen günlük olarak gerçekleşmesi için otomatikleştirmelisiniz.
3.  İptal listesi dosyasını, bu dosyaya gereksinim duyan tüm kullanıcıların erişebileceği bir konuma yerleştirin. Dosyayı hem ağdan hem de Internet'ten erişilebilecek bir konuma, tercihen bir Web sitesine koymanız önerilir. Bu, kullanıcıların dosyaya şirket ağının hem içinden hem de dışından erişebilmesini sağlar.
4.  İptal listesi gerekliliği içeren bir hak ilkesi şablonu oluşturun. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.

Kök sertifika sunucusunun sunucu lisans sertifikasını da iptal edebilirsiniz. Bu sertifika Microsoft Kayıt Hizmeti tarafından yayınlandığı için, Microsoft, kök sertifika sunucusunun sunucu lisans sertifikasını iptal edebilir. Microsoft bu iptali gerçekleştirmek için sunucu lisans sertifikasını iptal listesine ekler ve listeyi genel olarak kullanılabilir duruma getirir.

Buna ek olarak, kök sertifika sunucusu lisans sertifikanız, RMS yöneticiniz hazırlık sırasında bu seçeneği etkinleştirmeyi seçtiyse bir üçüncü parti tarafından iptal edilebilir. Bu seçeneği kullanırsanız, üçüncü parti yetkilisinin özel anahtarıyla imzalanmış olan bu sunucu lisans sertifikasını içeren iptal listesinin istemciler tarafından kullanılabilir duruma getirilmesi gerekir. Daha fazla bilgi için bu konuda daha sonra yer alan "[Sunucu Lisans Sertifikalarını İptal Etme](https://technet.microsoft.com/8020861d-d196-4431-8282-044675ef5616)" bölümüne bakın.

| ![](/security-updates/images/Cc747554.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| İptal işlemini uygularken dikkatli olun. Belirttiğiniz yenileme aralığına bağlı olarak iptal listesini düzenli olarak yenilemeniz gerekir; aksi takdirde liste otomatik olarak geçersiz hale gelir ve kullanıcıların o listeyi gerektiren içeriği kullanmasını önler. Kullanıcıların içeriği kullanmasını yanlışlıkla engellememek için iptal listesinin yenilenmesi için gerekli kıldığınız aralığı dikkatle değerlendirin. Ayrıca, iptal listesine ağın hem içinden hem dışından erişilebildiğinden emin olun. Daha fazla bilgi için bu konuda daha önce geçen "[İptal İlkelerini Tanımlama](https://technet.microsoft.com/e2fffe9f-def7-439b-a8aa-43f8a065813d)" bölümüne bakın. |
