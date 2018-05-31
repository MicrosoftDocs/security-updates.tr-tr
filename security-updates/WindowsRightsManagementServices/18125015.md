---
TOCTitle: Kullanıcı Anahtarları
Title: Kullanıcı Anahtarları
ms:assetid: '12dad6e2-64e7-4bab-bde7-b72f90f5cb05'
ms:contentKeyID: 18125015
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720202(v=WS.10)'
---

Kullanıcı Anahtarları
=====================

RMS kullanıcısının 1024 bit RSA anahtarlarından oluşan bir anahtar çifti vardır. Herhangi bir kullanıcının RMS sistemi içinde her zaman aynı anahtar çiftine sahip olması için, kullanıcının anahtar çifti RMS yapılandırma veritabanında depolanır.

Hak hesabı sertifikası kullanıcı ortak anahtarını içerir. Bu anahtar bir kullanım lisansındaki içerik anahtarını şifrelemek için kullanılır; böylece yalnızca belirli bir kullanıcı bu lisans aracılığıyla RMS korumalı içeriği kullanabilir.

Aynı hak hesabı sertifikasında, istemci makinesi ortak anahtarıyla şifrelenen kullanıcı özel anahtarı da bulunur. Böylece, hak hesabı sertifikasının yalnızca verildiği bilgisayarda kullanılması ve aynı zamanda herhangi bir kullanıcı için verilen her hak hesabı sertifikasının aynı anahtar çiftini içermesi sağlanır. RMS kullanılarak korunan herhangi bir içeriği kullanmak için kullanıcı özel anahtarı gerekir.
