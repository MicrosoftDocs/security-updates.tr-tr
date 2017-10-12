---
TOCTitle: RMS Güvenlik Grupları
Title: RMS Güvenlik Grupları
ms:assetid: '25749a83-8c12-48ec-96ad-296d31fd55d4'
ms:contentKeyID: 18125028
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720215(v=WS.10)'
---

RMS Güvenlik Grupları
=====================

RMS Kurulumu iki grup oluşturur: RMS Service Group ve Super Users grubu.

RMS Service Group, RMS işlemleri için gerekli olan tüm kaynaklara erişim sağlamak üzere yeterli izinlerin verilmiş olduğu bir yerel güvenlik grubudur. Yükleme sırasında, yönetici RMS hizmet hesabı olarak kullanılacak kullanıcı hesabını belirtir.. Bu kullanıcı hesabı, otomatik olarak RMS Service Group'un bir üyesi haline gelir ve bu hesaba ilgili izinler verilir. RMS çoğu normal işlemi sırasında bu kullanıcı hesabının altında çalışır.

Diğer önemli RMS grubu, Super Users grubudur. Bu grubun tüm içerik üzerinde tam denetimi vardır, başka bir deyişle, bu grubun bir üyesi tüm RMS korumalı içerik dosyalarının şifresini çözebilir ve bunlardan tüm RMS korumasını kaldırabilir. Varsayılan olarak Super Users grubunun üyesi yoktur ve grup, RMS yöneticilerini otomatik olarak içermez. Bu grubun üyeliğini yönetmek RMS korumalı içeriğinizin güvenliği için çok önemlidir. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Super Users Grubunu Kullanma" konusuna bakın.
