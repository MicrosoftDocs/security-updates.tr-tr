---
TOCTitle: Kümeleri Desteklemek için Temel Altyapıyı Genişletme
Title: Kümeleri Desteklemek için Temel Altyapıyı Genişletme
ms:assetid: '78f0f2f0-a075-409c-9f46-26eb62d1d05b'
ms:contentKeyID: 18125141
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747567(v=WS.10)'
---

Kümeleri Desteklemek için Temel Altyapıyı Genişletme
====================================================

Kümeleri daha büyük dağıtımlar için uyguluyorsanız, altyapınızın kümeleme gereksinimlerini destekleyecek şekilde ayarlanmış olduğundan emin olun. Aşağıdaki öğelerin dağıtım planlarınızda bulunması gerekir.

DNS Kaydı
---------

Sanal IP adresini extranet'e açmak için yapılan herhangi bir DNS kaydının, adresi intranet'e de açtığından emin olun.

Intranet için DNS kaydı yapılmadıysa, iç istemci lisansı istekleri başarısız olur. DNS ayarlarını değiştiremiyorsanız, kümedeki her sunucunun hosts tablosu, küme URL'sini kümenin sanal IP adresiyle eşlenecek şekilde değiştirilebilir. DNS kaydının hizmet sağlanmadan önce yapılması gerekir; hizmeti zaten sağladıysanız, RMS'yi sunucudan kaldırmanız ve sağlama işlemini yinelemeniz gerekir.

Yük Dengeleme
-------------

İstekleri kümeye dağıtmak için yük dengeleme sunucularını, Ağ Yük Dengeleme hizmetini veya donanım yük dengelemesini uygun şekilde etkinleştirmek amacıyla gerekli donanım ve yazılımları kurun.
