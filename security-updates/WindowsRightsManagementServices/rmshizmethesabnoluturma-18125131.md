---
TOCTitle: RMS Hizmet Hesabını Oluşturma
Title: RMS Hizmet Hesabını Oluşturma
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18125131
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747546(v=WS.10)'
---

RMS Hizmet Hesabını Oluşturma
=============================

Yükleme sırasında, RMS yerel bilgisayarda **RMS Service Group** adlı bir güvenlik grubu oluşturur ve bu gruba RMS'nin çalışması için gereken kaynakların ilgili izinlerini verir.

Bir sunucuda RMS sağladığınızda, RMS hizmeti hesabı olarak bir kullanıcı hesabı belirtirsiniz. Belirttiğiniz hesap RMS Service Group üyesi haline getirilir ve böylece hesaba bu grupla ilişkili izinler verilir. RMS, normal işlemler sırasında çoğu amaç için RMS hizmet hesabının altında çalışır.

| ![](images/Cc747546.note(WS.10).gif)Not                    |
|-----------------------------------------------------------------------------------------|
| RMS hizmet hesabı, RMS'yi yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. |

Güvenlik nedeniyle, RMS hizmet hesabı olarak kullanmak üzere özel bir kullanıcı hesabı oluşturmanız ve bu hesabı başka hiçbir amaç için kullanmamanız önerilir. Ayrıca, bu hesaba herhangi bir ek izin vermemelisiniz.

| ![](images/Cc747546.Important(WS.10).gif)Önemli      |
|-----------------------------------------------------------------------------------|
| Bu özel kullanıcı hesabını RMS'yi yüklemeden ve sağlamadan önce oluşturmalısınız. |

RMS Service Group'a verilen izinler ve RMS'nin altında çalıştığı hesaplar hakkında daha fazla bilgi için, bu belge grubundaki “RMS Teknik Başvuru Kılavuzu” bölümünde bulunan “RMS Güvenlik Modülü” konusuna bakın.
