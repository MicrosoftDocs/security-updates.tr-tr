---
TOCTitle: Uygulamaları Dışlama
Title: Uygulamaları Dışlama
ms:assetid: 'b68ae4b2-b9ba-44ae-90cb-c88df600ec86'
ms:contentKeyID: 18125233
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747644(v=WS.10)'
---

Uygulamaları Dışlama
====================

Tüm lisans isteklerini denetlemek için kullanılacak bir RMS etkinleştirilmiş uygulama sürümü belirtebilirsiniz. Uygulama dışlama özelliği her kullanım lisansını, lisansın verildiği RMS korumalı içeriğe, lisansı isteyen uygulama dışlanan listesinde bulunmaması durumunda bağlanabileceği koşuluyla damgalar.

Bu, örneğin bir kuruluşun uygulama için güvenlik güncellemesi dağıtması durumunda yararlı olabilir. Sistem yöneticileri istemci bilgisayarların güvenlik güncellemesini yüklemesini sağlamak için olağan mekanizmalarını kullanabilir. Bunun ardından, yönetim Web sitesinin kullanıldığı uygulamanın sürüm bilgilerini kullanarak tanımlanan uygulama dışlama ilkelerini belirleyebilirler. Bu dışlama ilkesi, RMS'nin önceki yazılım sürümlerini kullanan istemcilere lisans vermesini önler.

RMS etkinleştirilmiş uygulamalar dosya adları ve sürüm numaralarıyla dışlanır. Bunu uygulamanın daha yeni, daha güvenli bir sürümü çıktığı zaman kullanıcıların bu sürümü yüklemesini sağlamak için kullanabilirsiniz. Örneğin, kuruluşunuzda 1.0.4.2315 sürüm numaralı bir RMS etkinleştirilmiş uygulama dağıtılmış durumda. Uygulama geliştirici bir güvenlik sorunu buldu ve sorunu gidermek için 1.0.4.4200 numaralı bir sürüm çıkardı. Yeni uygulama sürümünü dağıtmanın yanı sıra, kullanıcıların önceki uygulama sürümünü kullanarak içerik kullanmasını önleyen bir dışlama ilkesi belirleyebilirsiniz.

Diğer dışlama türlerinde olduğu gibi, uygulama dışlama özelliğini, yürürlüğe sokmak istediğiniz her kümede yapılandırmanız gerekir.

Bu dışlama ilkesini sunucunuza uyguladığınız zaman, istemciler yeni kullanım lisansları isteyip RMS korumalı içeriğe bağlamak için dışlanan uygulamayı kullanamaz. Bununla birlikte, istemciler dışlanan ilkeyi önceki lisanslı dosyalar için kullanmaya devam edebilir.

| ![](images/Cc747644.note(WS.10).gif)Not                                                                                                                                                                                                                                                                            |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS, uygulama sürümünün 4 basamaklı, nokta ile ayrılmış biçimde olmasını gerektirir (\#.\#.\#.\# ). Bununla birlikte, belirli uygulamalar, uygulama sürümünü 2 veya 3 basamaklı, nokta ile ayrılmış sayılarla belirtir. Bu durumda, sürüm numarasını RMS'nin gerektirdiği biçime uyarlamak için uygun olacak şekilde, .0 eklemeniz gerekebilir. |
