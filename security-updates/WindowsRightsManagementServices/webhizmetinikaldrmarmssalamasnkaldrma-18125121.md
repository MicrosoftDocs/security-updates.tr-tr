---
TOCTitle: 'Web Hizmetini Kaldırma (RMS Sağlamasını Kaldırma)'
Title: 'Web Hizmetini Kaldırma (RMS Sağlamasını Kaldırma)'
ms:assetid: '68b4e2b0-b1b7-4b0a-8c1a-82ac27c1f12e'
ms:contentKeyID: 18125121
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747602(v=WS.10)'
---

Web Hizmetini Kaldırma (RMS Sağlamasını Kaldırma)
=================================================

RMS sunucusunun yetkisi alındıktan ve tüm RMS koruması kaldırıldıktan sonra, Web hizmeti aşağıdaki adımlar kullanılarak kaldırılabilir:

-   **Genel Yönetim** sayfasından **RMS'yi bu Web sitesinden kaldır**'ı seçin.

Sonraki adım kaldırılan sunucunun türüne bağlı olsa da, RMS her durumda IIS'den kaldırılır.

-   Sunucu bir kümenin bir parçasıysa (ve kümedeki son sunucu değilse), ek adım gerekmez.
-   Sunucu yalnızca lisans sunucusuysa dizin hizmetleri veritabanını kaldırın, ancak (hizmette olan sertifika sunucusu tarafından kullanılan) yapılandırma ve günlük veritabanını koruyun.
-   Sunucu kuruluştaki son RMS sunucusuysa, yapılandırma ve günlük veritabanını koruyun, ancak Active Directory'deki hizmet bağlantı noktasını (SCP) kaldırın.
