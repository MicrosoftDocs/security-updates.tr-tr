---
TOCTitle: Topoloji Hedeflerini Oluşturma
Title: Topoloji Hedeflerini Oluşturma
ms:assetid: '8275a04d-3e5b-40b0-be9d-2f31b7aeca6b'
ms:contentKeyID: 18125163
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747652(v=WS.10)'
---

Topoloji Hedeflerini Oluşturma
==============================

Topoloji tasarımındaki en önemli adımlardan biri uygun hedeflerin belirlenmesidir. RMS topolojisinin tasarımında göz önünde bulundurmanız gereken bazı temel noktalar şunlardır:

-   **Yönetim maliyetleri**. Site topolojisi yönetim maliyetlerini en aza indirmelidir. Bu, sunucu yönetimini olabildiği yerlerde merkezileştirmeyi ve kullanılan sunucu sayısını en aza indirmeyi içerir.
-   **Ağ gecikmesi**. İstemci ve sunucu arasındaki ağdan kaynaklanan gecikme, kullanıcılara, e-posta ve belgelerini açarken fark edecekleri ek gecikme olarak yansır. Genelde, bu gecikmenin, zamanın an az yüzde 90'ında, her iki yönde de iki saniyeden az olmasını sağlayın.
-   **Güvenilirlik**. İstemci ve sunucu arasındaki ağ, tek bir HTTP isteği ve yanıtına yönelik, işlemin kaybolması veya zarar görmesi anlamına gelen hata oranının yüzde 5'ten az olmasını sağlayacak kadar güvenilir olmalıdır.

Bunlar yalnızca genel kurallardır; kuruluşunuzun gereksinim ve kaynaklarına göre kendi hedeflerinizi kendiniz oluşturmalısınız. Hedeflerin belirlenmesi, bir topolojinin gereksinimlerinizi karşılayıp karşılamadığını belirlemek için başlangıç noktasıdır. Kullanıcı sayısı, lisans isteği sayısı, sorgu sayısı, ileti sayısı ve diğer RMS ile ilişkili trafik gibi, hedeflere ulaşılmasını etkileyen pek çok etmen vardır. Ek olarak, RMS'yi dağıtmayı planladığınız etki alanları ve ormanları içeren dağıtım stratejinizin topoloji hedeflerinize ulaşmanızda önemli etkisi olabilir. Topoloji tasarım işleminde ilerlerken hedeflerinizi her zaman göz önünde bulundurmalı ve her tasarım işleminin hedeflerinizi nasıl etkileyeceğini belirlemelisiniz.
