---
TOCTitle: RMS Korumalı İçeriği Kullanma
Title: RMS Korumalı İçeriği Kullanma
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18125058
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720251(v=WS.10)'
---

RMS Korumalı İçeriği Kullanma
=============================

Kullanıcılar korumalı içeriği kullanırken, kullanıcının bilgisi dahilinde iki işlem gerçekleşir. İlk olarak, kullanıcı belgeyi açtığında RMS etkin uygulama bir kullanım lisansı ister. Daha sonra, RMS etkin uygulama iptal listesi gerektirip gerektirmediğini belirlemek için kullanım lisansını inceler ve lisansın güven zincirindeki veya hak hesabı sertifikasındaki herhangi bir sertifikanın iptal edilip edilmediğini denetler. Her iki işlem de tamamlandıktan sonra RMS etkin uygulama, tüm haklar ve iptaller işlem yapmasına izin veriyorsa RMS korumalı içeriği işler.

Bir iptal listesi gerekiyorsa, uygulama, iptal listesinin geçerliliği sona ermemiş yerel bir kopyasını arar. Gerekiyorsa iptal listesinin güncel bir kopyasını alır. Uygulama bunun ardından geçerli bağlamla ilgili tüm iptal koşullarını uygular.

İçeriğe erişimi engelleyen bir iptal koşulu yoksa, uygulama içeriği işler ve kullanıcı kendisine tanınan haklardan yararlanabilir.

RMS'yi yetkili dış kullanıcılardan gelen kullanım lisansı isteklerini işleyecek şekilde yapılandırabilirsiniz. Bu, kullanıcıların korumalı içeriği Internet üzerinden paylaşmasına olanak verir.

Bu bölüm aşağıdaki konuları içerir:

-   [Kullanım Lisansı Alma](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)
-   [Kullanım Lisansları ve Dış Kullanıcılar](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)
