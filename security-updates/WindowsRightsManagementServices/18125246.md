---
TOCTitle: Güvenilen Yayımlama Etki Alanları
Title: Güvenilen Yayımlama Etki Alanları
ms:assetid: 'bca1c33a-d3ef-42b5-adbe-6e104979a71f'
ms:contentKeyID: 18125246
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747738(v=WS.10)'
---

Güvenilen Yayımlama Etki Alanları
=================================

RMS sunucuları varsayılan olarak, farklı bir kümedeki RMS sunucusu tarafından verilen yayımlama lisansları için kullanım lisansları vermez. Bununla birlikte, aynı sunucunun veya kümenin bir korumalı içerik bölümü için hem yayımlama, hem de kullanım lisansları veremediği durumlar vardır. Örneğin iki firma birleştiğinde, belirli bir RMS kümesi devre dışı bırakılıp başka biri bunun yerini aldığında bu durum oluşabilir. Bu durumda, bir RMS kümesi farklı bir RMS kümesi tarafından oluşturulan yayımlama lisanslarına kullanım lisansları verebilmelidir.

Güvenilen yayımlama etki alanı kullanarak, bir RMS kümesini farklı bir RMS kümesi tarafından verilen yayımlama lisanslarına güvenecek ve bunlar için kullanım lisansları verecek şekilde yapılandırabilirsiniz. Bunun için, diğer sunucudan sunucu lisans sertifikasını ve özel anahtarı alıp, güvenilen yayımlama etki alanlarına ekleyin. Alınan özel anahtarlar yalnızca imzalı yayımlama lisanslarının şifresini çözmek için kullanılır; yeni lisansları imzalamak için kullanılamaz.

Güvenilen kullanıcı etki alanları ve adım adım yönergeler hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Güvenilen Yayımlama Etki Alanı Ekleme ve Kaldırma" ve "Güven İlkeleri Oluşturma" konularına bakın.
