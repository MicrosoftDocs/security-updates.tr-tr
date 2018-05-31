---
TOCTitle: RMS Yapılandırmasını Geri Almak için
Title: RMS Yapılandırmasını Geri Almak için
ms:assetid: '9fa63daa-5fb9-4afd-8371-b38248619857'
ms:contentKeyID: 18125195
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747706(v=WS.10)'
---

RMS Yapılandırmasını Geri Almak için
====================================

Bu yordamı uygulamak için, eriştiğiniz bilgisayarda Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesine yerel olarak oturum açmış olmalısınız. Domain Admins grubunun üyeleri de bu yordamı uygulayabilir. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

**Genel Yönetim** sayfasını açmak için, **Başlat**'ı tıklatın, **Tüm Programlar**'a gidin, **Windows RMS'**ye gidin ve sonra **Windows RMS Yönetimi**'ni tıklatın.

Sunucu hazırlığını kaldırdığınız zaman, yapılandırma veritabanının ClusterServer tablosundan kaldırılır. Kümedeki son sunucunun hazırlığını kaldırdığınız zaman, dizin hizmetleri veritabanı SQL Server'dan silinir. Bir kümedeki son kök sertifika sunucusunun hazırlığını kaldırırken, sertifika hizmet bağlantı noktasının (SCP) kaydını el ile silin. Hazırlığı ve yüklemeyi kaldırmak, SCP'yi Active Directory’den kaldırmaz.

Kök sertifika sunucusunu hazırlamadan kaldırmayı seçerseniz, sitenin henüz hazırlanmadığı ve SCP'nin Active Directory'den kaldırılmayacağı uyarısını alırsınız. Ancak, devam etmek için **Evet**’i seçerseniz sitenin hazırlığı sizin için kaldırılacaktır. Yüklemeyi kaldırmak, hizmet bağlantı noktasını Active Directory’den kaldırmaz.

RMS Yapılandırmasını Geri Alma
------------------------------

#### RMS Yapılandırmasını Geri Almak için

1.  RMS hazırlığını kaldırmak istediğiniz sunucuya oturum açın.

2.  **Genel Yönetim** sayfasını açın.

3.  Windows RMS'nin sağlandığı Web sitesinin yanındaki **RMS'yi bu Web sitesinden kaldır**'ı tıklatın ve sonra **Tamam**'ı tıklatın.

4.  Sertifika hizmet bağlantısının kaydını Active Directory’den silmek için RMS hizmet bağlantı noktası Web sayfasındaki **URL kaydını sil**'i tıklatın.
