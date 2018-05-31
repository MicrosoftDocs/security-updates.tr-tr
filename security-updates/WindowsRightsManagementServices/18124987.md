---
TOCTitle: Kullanıcı Hesaplarını Etki Alanları Arasında Taşıma
Title: Kullanıcı Hesaplarını Etki Alanları Arasında Taşıma
ms:assetid: '0010b0ea-07c0-41c9-81f7-5881343d1d55'
ms:contentKeyID: 18124987
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720179(v=WS.10)'
---

Kullanıcı Hesaplarını Etki Alanları Arasında Taşıma
===================================================

Bir kuruluşta kök sertifika sunucusu kurup sağladığınızda, sunucu Active Directory'deki orman başına ayarında RMS hizmet sağlayıcı olarak kaydettirilir. Her Active Directory ormanı için yalnızca bir kök sertifika kümesi olabilir.

Genellikle, kullanıcı hesabını bir etki alanından aynı ormanda bulunan bir diğerine taşıdığınızda, yeni etki alanında o kullanıcı hesabı için yeni bir SID oluşturulur. Böylece, kullanıcı sunucudan yeni bir hak hesabı sertifikası almayı denediğinde, yeni SID'si nedeniyle sunucu tarafından yeni bir kullanıcı olarak görülür. Sunucu, kullanıcı için yeni anahtarlar üretir ve kullanıcının özgün e-posta adresini kullanarak yeni hak hesabı sertifikasını yayınlar. Kullanıcı yeni hak hesabı sertifikasını varolan lisansıyla kullanmayı denediğinde, SID ve anahtarlar eşleşmeyecek, kullanıcının yeni bir lisans alması gerekecektir. Bu durum, bir kullanıcı hesabını farklı ormandaki bir etki alanına taşımada da geçerlidir.
