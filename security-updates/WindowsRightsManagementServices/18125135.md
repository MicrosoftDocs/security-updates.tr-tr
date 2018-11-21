---
TOCTitle: Alt Kayıt Hizmeti Dosyasında İzinler Ayarlama
Title: Alt Kayıt Hizmeti Dosyasında İzinler Ayarlama
ms:assetid: '737bb69b-fe26-4057-9569-e632f7bbf295'
ms:contentKeyID: 18125135
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747627(v=WS.10)'
---

Alt Kayıt Hizmeti Dosyasında İzinler Ayarlama
=============================================

Alt kayıt hizmeti kök sertifika sunucusu üzerinde çalışır ve sağlama işlemi sırasında lisans sunucusunu kaydettirir. Varsayılan olarak, alt kayıt hizmeti yalnızca kök sertifika sunucusunda bulunan yerel sistem hesabına erişim izni verir. Bir lisans sunucusunu sağlamak için bu tür bir hesapla lisans sunucusuna oturum açmanız gerekir. Alternatif olarak, kök sertifika sunucusundaki yerel yöneticinin lisans sunucusu üzerinde hazırlık işlemini gerçekleştirecek kullanıcı hesabına erişim izni vermesi için SubEnrollService.asmx alt kayıt hizmeti dosyasındaki DACL'yi değiştirmesi gerekir. SubEnrollService.asmx, kök sertifika sunucusundaki Sertifika sanal dizininde bulunur.
