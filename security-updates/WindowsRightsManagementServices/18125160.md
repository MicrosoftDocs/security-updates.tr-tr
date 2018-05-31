---
TOCTitle: Lisans Sunucusu Alt Kaydı
Title: Lisans Sunucusu Alt Kaydı
ms:assetid: '7bc63397-9186-464c-8824-867038adce9b'
ms:contentKeyID: 18125160
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747640(v=WS.10)'
---

Lisans Sunucusu Alt Kaydı
=========================

Lisans sunucuları sağlama sırasında, alt kayıt olarak adlandırılan bir işlemle otomatik olarak kaydettirilir. Ancak, lisans sunucusu kümesine yeni bir sunucu eklediğinizde, kümenin sunucu lisans sertifikasını ve yapılandırma veritabanını kullandığından, yeni sunucunun alt kaydı açık olarak yapılmaz.

Lisans sunucusu, alt kayıt isteğini Microsoft Kayıt Hizmeti'ne göndermek yerine kök sertifika sunucusuna gönderir. Lisans sunucusu için alt kayıt isteği, kök sertifika sunucusu için kayıt isteğiyle özdeştir.

Kök sertifika sunucusu bir alt kayıt isteği aldığında, isteğin uygun şekilde biçimlendirildiğini doğrular ve sonra kök sertifika sunucusunun lisans sertifikası zincirini içeren sertifika zincirini ve kök sertifika sunucusu tarafından imzalanan bir sertifikayı döndürür. Sertifika, kök sertifika sunucusu ortak anahtarıyla imzalanan sunucu ortak anahtarını içerir. Sertifika lisans sunucusuna yayımlama ve kullanım lisansları verme hakkı verir.

Sunucu lisans sertifikası bir yıl süreyle geçerlidir. Geçerlilik süresi sertifikanın verildiği tarihte başlar. Geçerlilik süresi sonunda sertifika yenilenebilir. Sunucu tarafından verilen sertifikalar ve lisanslar yedi yıl süreyle geçerlidir. Geçerlilik süresi sertifikanın veya lisansın verildiği tarihte başlar.

Varsayılan olarak, kök sertifika sunucusunda alt kayıt isteğini işlemek için gereken SubEnrollService.asmx hizmeti tüm erişimi reddetmek üzere yapılandırılır. Bir isteğin işlenebilmesi için RMS yöneticisi erişimine izin vermek amacıyla DACL'leri değiştirmeniz gerekir.
