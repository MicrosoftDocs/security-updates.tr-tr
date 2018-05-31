---
TOCTitle: RMS Yapılandırma Veritabanı
Title: RMS Yapılandırma Veritabanı
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18125137
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747634(v=WS.10)'
---

RMS Yapılandırma Veritabanı
===========================

RMS, yapılandırmasını ve ilke bilgilerini depolamak için Microsoft® SQL Server veya Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A gibi bir veritabanı sunucusu kullanır. Her RMS sunucusu veya kümesi için bir yapılandırma veritabanı vardır; bu veritabanı yapılandırma verilerini ve diğer verileri depolar, paylaşır ve alır.

Kök sertifika sunucusunun veya kümesinin yapılandırma veritabanı, Windows kullanıcı kimliklerinin ve bunların hak hesabı sertifikalarının listesini içerir. Sertifika anahtarı çifti, veritabanında depolanmadan önce RMS sunucu ortak anahtarıyla şifrelenir. Lisans sunucularının yapılandırma veritabanları bu bilgileri içermez.

RMS Service Group, veritabanının saklı yordamları üzerinde yürütme izinlerine sahiptir.

**Önemli   **MSDE 2000'in RMS veritabanlarını sadece deneme ortamlarını desteklemek için kullanılması önerilir, çünkü MSDE 2000 ağ arabirimlerini desteklemez. Ayrıca, MSDE 2000 kullanım koşulları, bir MSDE 2000 veritabanını değiştirmek için SQL Server istemcilerini kullanamayacağınızı belirtir. Bu sınırlama, günlük bilgilerini görüntüleyememenize veya yapılandırma veritabanında saklanan verileri değiştirememenize neden olur.
