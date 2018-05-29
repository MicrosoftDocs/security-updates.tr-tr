---
TOCTitle: RMS Hizmetlerini Yayımlama
Title: RMS Hizmetlerini Yayımlama
ms:assetid: '3cca9325-6bd3-49ad-aa3f-e0693205d3f4'
ms:contentKeyID: 18125059
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720247(v=WS.10)'
---

RMS Hizmetlerini Yayımlama
==========================

RMS hizmetlerinin URL'leri sunucu sağlama işlemi sırasında Active Directory'ye yayımlanır. Sağlama işlemi sırasında, RMS Kurulumu, ilgili ormanda başka bir RMS sunucusunun yüklü olup olmadığını belirlemek için Active Directory'yi sorgular. Başka bir RMS sunucusu yüklü değilse, RMS Kurulumu, sunucuyu kök sertifika sunucusu olarak yapılandırır. RMS'yi kullanmadan önce, istemcilerin kök sertifika sunucusu URL'sini bulmasına olanak tanımak için hizmet bağlantı noktasını (SCP) Active Directory'ye kaydettirmeniz gerekir. Kök sertifika sunucusu üzerinde çalışan hizmetlere bağlanmak isteyen istemciler, bu kök sertifika sunucusu URL'si için Active Directory'yi sorgulayarak işe başlarlar. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Hizmet Bağlantı Noktasını Kaydettirme" konusuna bakın.

| ![](/security-updates/images/Cc720247.note(WS.10).gif)Not                                                                                                                         |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Topolojiniz kök sertifika sunucusu kümesinde bulunan birden fazla sunucuyu içeriyorsa, URL yöneticinin sağlama işlemi sırasında belirttiği, kümeye ait yük dengeleme sunucusunu işaret eder. |
