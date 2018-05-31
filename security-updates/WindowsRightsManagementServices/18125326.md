---
TOCTitle: Dışlama İlkesini Yönetme
Title: Dışlama İlkesini Yönetme
ms:assetid: 'ee31e099-e095-4648-95da-0009fbeb48cb'
ms:contentKeyID: 18125326
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747730(v=WS.10)'
---

Dışlama İlkesini Yönetme
========================

Sertifika ve lisans isteklerini hak hesabı sertifikası veya kasa sürümünü temel alarak reddetmek için sunucu tarafı dışlama ilkeleri uygulayabilirsiniz. Dışlama ilkeleri kuşkulu sorumlular tarafından yapılan yeni sertifika ve lisans isteklerini reddeder, ancak iptalin aksine dışlama ilkeleri sorumluları geçersiz kılmaz. Yöneticiler, potansiyel olarak zararlı veya kuşkulu uygulamaları da RMS korumalı içeriğin şifresini çözememeleri için dışlayabilir. Ek olarak, yöneticiler Windows işletim sistemlerinin bazı sürümlerini de dışlayabilirler. Böylece, hak korumalı içeriğin söz konusu Windows işletim sistemi sürümlerini çalıştıran istemci bilgisayarlarda kullanılmasını engellerler.

Bir varlık dışlandığında, RMS sunucusu tarafından oluşturulan kullanım lisansları dışlama listesinde belirtilen varlığa sahip olur. Dışlama ilkesine dahil ettiğiniz bir varlığı bir süre sonra silmeye karar verirseniz, varlığı yönetim Web sitesinin Dışlama ilkeleri sayfasından silebilirsiniz. Bu, varlığı dışlama listesinden kaldırır. Tüm yeni sertifika veya lisans istekleri bu varlığı dışlanmış olarak kabul etmez.

Bir varlığı istemeyerek dışlamadıkça, dışlama ilkesi yaratılmadan önce verilen tüm sertifikaların kullanım süresinin dolduğundan emin olana kadar varlığı dışlama ilkesinden kaldırmamanız önerilir. Aksi takdirde hem eski hem de yeni sertifikalar içeriğin şifresinin çözülmesine olanak sağlar ve bu da kuruluşunuzun istemediği bir durum olabilir.

Bu başlıkta dışlama ilkesini yönetme hakkında bilgiler verilmektedir. Varlıkları dışlamayla ilgili adım adım yönergeler için bu konuda daha sonra yer alan "[Dışlama İlkelerini Etkinleştirme](https://technet.microsoft.com/bbb1ce50-bc11-41cf-b75b-a6756141908f)" bölümüne bakın.

Bu bölüm şunları kapsar:

-   [Kasa Sürümlerini Dışlama](https://technet.microsoft.com/e287f026-aab2-43ab-93bc-48087da82f36)
-   [Hak Hesabı Sertifikalarını Dışlama](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)
-   [Windows Sürümlerini Dışlama](https://technet.microsoft.com/8b8a184d-ac0e-4a43-822c-d2fae2faf484)
-   [Uygulamaları Dışlama](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)
