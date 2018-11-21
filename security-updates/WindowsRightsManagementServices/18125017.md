---
TOCTitle: Artıklık ve Yük Dengelemesi Sağlama
Title: Artıklık ve Yük Dengelemesi Sağlama
ms:assetid: '162d547c-78a7-4848-b43e-58e481832af2'
ms:contentKeyID: 18125017
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720199(v=WS.10)'
---

Artıklık ve Yük Dengelemesi Sağlama
===================================

Kullanıcıların lisans alabilmesini ve gerektiğinde içerik yayımlayabilmesini sağlamak için, kümeleri kullanarak yedek RMS sunucuları dağıtmanız önerilir. Buna göre, en az iki sunucu içeren bir kök sertifika kümesi dağıtmanız gerekir. Kuruluşunuzdaki belirli bir grubun özel lisans gereksinimlerini desteklemek üzere ayrı bir lisans sunucusu da dağıtıyorsanız, lisans sunucusunu da en az iki sunucudan oluşan bir küme olarak dağıtmanız gerekir.

Kök sertifika kümesinin veya herhangi bir lisans kümesinin birden çok fiziksel sunucusu, paylaşılan bir URL'nin veya sanal adresin arkasında bir “Web grubu” oluşturur. Kuruluşunuz bir sunucu grubu kullanıyorsa, RMS'yi, sanal adreslemede kullandığınız her yöntemle (hepsinin bir kez denendiği DNS, Ağ Yük Dengeleme hizmeti veya özel bir donanım çözümü gibi) tümleştirebilirsiniz.

Yük dengelemeye ek olarak sanal adresleme, sertifika veya lisans hizmetleri için fiziksel bir sunucuya bağımlılığı ortadan kaldırdığından, RMS'yle kullandığınızda çok yararlı olur. Hiçbir son kullanıcı bilgisayarı kümedeki tek bir sunucuya doğrudan erişim gerektirmez.
