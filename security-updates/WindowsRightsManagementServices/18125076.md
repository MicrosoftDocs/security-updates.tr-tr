---
TOCTitle: 'RMS İptal İşlemi Nasıl Çalışır?'
Title: 'RMS İptal İşlemi Nasıl Çalışır?'
ms:assetid: '469e3938-a59b-4c92-9779-ead64e724d00'
ms:contentKeyID: 18125076
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720263(v=WS.10)'
---

RMS İptal İşlemi Nasıl Çalışır?
===============================

İptal işlemi, bağlanma isteğinde iptal edilen bir varlık bulunduğunda, kullanıcının içeriği kullanmasını sağlayan işlem olan bağlanma işlemini önleyerek çalışır. İptal, istemci bilgisayarlara dağıtılan iptal listeleri aracılığıyla uygulanır. Bu listeler, listeyi yayınlayan sorumlunun iptal ettiği içeriği, uygulamaları, kullanıcıları veya diğer sorumluları belirten, imzalı XrML dosyalarıdır.

Kullanıcı korumalı içerik kullanma girişiminde bulunduğunda, ilişkili RMS etkin uygulama RMS istemcisine bir bağlanma isteği içinde uygun bir hak isteği gönderir. Örneğin kullanıcı bir dosyayı açmak isterse, uygulama dosyanın açılmasını sağlayan bir Görüntüleme hakkı ister. Kullanıcı dosyayı düzenlemeyi denediğinde uygulama bir Düzenleme hakkı ister.

RMS istemcisi bağlanma isteğini işlerken aşağıdaki adımları izler:

1.  Kullanım lisansını tüm iptal listesi gereksinimlerine göre değerlendirir.
2.  Kullanım lisansı iptal gerektiriyorsa, istemci bileşeni kullanım lisansında belirtilen yenileme aralığına uygun şekilde, belirtilen iptal listesinin bulunup bulunmadığını, kayıtlı ve geçerli olup olmadığını doğrular.
3.  İptal listesini imzalayan sorumlunun, kullanım lisansında lisansı iptal etme izni olan sorumlu olarak belirtildiğini doğrular.
4.  Bu denetimler başarılıysa, istemci bileşeni özgün bağlanma isteğinde yer alan sorumlulardan herhangi birinin iptal edilip edilmediğini belirler. İptal edilmişse, bağlanma isteğini reddeder.

İptal listeleri yönetici tarafından istemci bilgisayarlara dağıtılabilir veya bir kullanım lisansı gerektirdiğinde RMS etkin uygulama tarafından bilgisayara yüklenebilir. İptal listesi bir içerik bölümünü bağlamak için kullanıldığında kaydettirilir ve uygulama açık olduğu sürece diğer kullanım lisanslarıyla bağlanma istekleri için kullanılabilir. Uygulama kapatıldığında iptal listesinin kaydı kaldırılır.

Aşağıdaki diyagram bağlanma işlemini ve iptalin bağlanma işleminde nasıl çalıştığını gösteriyor.

![](/security-updates/images/Cc720263.81aa2d70-d261-49ad-b446-96a2eddba1a5(WS.10).gif)

İptal isteğe bağlıdır. RMS yöneticisi, kuruluşun bir veya daha fazla hak ilkesi şablonunda belirterek iptal isteğinde bulunabilir. İptal gerektiğinde, istenen iptal listesi kullanıcı bilgisayarında hazır, kayıtlı ve kullanım lisansında belirtilen yenileme aralığından daha yeni olmadıkça lisans bağlanamaz.

Ancak, kullanım lisansı gerektirmese bile, iptalin belirli bir kullanım lisansı için geçerli olabileceğini unutmamak gerekir. Bağlanma isteğinde yer alan güven zincirindeki bir sertifika veren, istemci bilgisayarda kayıtlı olan bir iptal listesi yayınladığı zaman iptal yürürlüğe girer. Bu senaryoda iptal listesi, söz konusu kullanım lisansları iptal gerektirmese bile bağlanma isteklerini işlemek için kullanılmaktadır. Bu durum RMS etkin uygulama kapatılana kadar geçerlidir; uygulama kapatıldığında iptal listesinin kaydı kaldırılır.

Örneğin bir kullanıcı, A varlığı tarafından verilen kullanım lisansı A varlığı tarafından verilen iptal listesini gerektiren içeriğin bir bölümünü kullanmayı denerse, RMS etkin uygulama kullanım lisansında belirtilen URL'den iptal listesini alır ve sonra bunu kaydettirirr. RMS istemcisi bağlanma isteğini işlerken, olası iptaller için iptal listesini denetler.

RMS etkin uygulamayı açık bırakan kullanıcı daha sonra, kullanım lisansı yine A varlığı tarafından verilen içeriğin ikinci bölümünü kullanmayı dener. Bu kullanım lisansında iptal koşulu bulunmamasına rağmen, A varlığından alınan iptal listesi şu anda kullanıcının bilgisayarında kayıtlıdır. Bu durumda istemci bileşeni bağlanma isteğini işleme koymadan önce iptal listesini inceler.

Bunun ardından, kullanıcı, kullanım lisansı C varlığı tarafından verilmiş bir içerik bölümünü kullanmayı dener. Kullanım lisansı bir iptal koşulu içermez. İstemci bilgisayarda kayıtlı olan tek iptal listesi A varlığının yayınladığı liste olduğu ve A varlığı bu kullanım lisansının güven zincirinde bulunmadığı için, bağlanma için iptal yürürlüğe girmez.

Son olarak, kullanıcı RMS etkin uygulamayı kapatır ve daha sonra içeriğin iptal koşulu içermeyen ikinci bölümünü yeniden açar. Uygulama kapatıldığında A varlığı tarafından verilen iptal listesinin kaydı kaldırıldığından, RMS istemcisi bağlanma isteğini işlemek için bunu incelemez.
