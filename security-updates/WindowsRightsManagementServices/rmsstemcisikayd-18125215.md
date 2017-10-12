---
TOCTitle: RMS İstemcisi Kaydı
Title: RMS İstemcisi Kaydı
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18125215
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747613(v=WS.10)'
---

RMS İstemcisi Kaydı
===================

Bilgisayarları kuruluş ağına bağlı olmadığında yazarlara RMS korumalı içerik yayımlama olanağı sağlayan RMS istemci lisans sertifikası almak için, istemci bilgisayarlar RMS yayımlama hizmetine kaydolabilirler. Bu durumda, bu bilgisayardan yayımlanan RMS korumalı içeriğin kullanım hakları bilgilerini içeren yayımlama lisanslarını, yayımlama hizmeti yerine istemci bilgisayar imzalar ve verir.

İstemci lisans sertifikalarını RMS yayımlama hizmeti verir.

İstemci kaydı şu adımları içerir:

1.  İstemci bilgisayar kullanıcının hak hesabı sertifikasını bir kayıt isteği içinde kök sertifika sunucusunda veya kümesinde ya da lisans sunucusunda veya kümesinde çalışan yayımlama hizmetine gönderir.
2.  Sunucu, ağ yöneticisi ayarlarını temel alarak istemci kaydına izin verildiğini ve hak hesabı sertifikasının yapılandırma veritabanındaki bir dışlama listesinde olmadığını doğrular. Dışlama listeleri oluşturma konusunda daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Dışlama İlkesini Yönetme" konusuna bakın.
3.  Yayımlama hizmeti istemci bilgisayar için bir anahtar çifti oluşturur. Bir istemci lisans sertifikası oluşturur ve ortak anahtarı sertifikaya yerleştirir. Özel anahtarı hak hesabı sertifikası ortak anahtarıyla şifreler ve sonra bu anahtarı sertifikaya yerleştirir.
4.  Yayımlama hizmeti istemci bilgisayara bir istemci lisans sertifikası verir.
