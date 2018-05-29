---
TOCTitle: RMS Sistemini Yedekleme ve Geri Yükleme
Title: RMS Sistemini Yedekleme ve Geri Yükleme
ms:assetid: 'c11f3ac1-e512-402b-bf13-9ff21f5fe745'
ms:contentKeyID: 18125253
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747745(v=WS.10)'
---

RMS Sistemini Yedekleme ve Geri Yükleme
=======================================

Sistem kurtarma planlarken, planlarınızda veritabanı sunucusunda ve RMS sunucusunda hata oluşma durumları göz önünde bulundurulmalıdır. Veritabanı sunucusu hatası durumunda, yapılandırma veritabanının yedek kopyasını kullanarak RMS sunucusu veya kümesinin işlevselliğini geri yükleyebilirsiniz. Sunucu lisans sertifikası ve özel anahtar yapılandırma veritabanında depolandığından, RMS sunucunuz için yeni bir sunucu lisans sertifikası veya özel anahtar almanız gerekmez.

RMS Sistem Yedeğini Planlama
----------------------------

Sunucu anahtarına ek olarak, yapılandırma veritabanında ortak anahtar bilgilerini içeren kullanıcı verileri de saklanır. Değerli anahtar verilerini saklamak için yapılandırma veritabanını ortama yedekleyin ve ortamı güvenli bir konuma yerleştirin. Kök sertifika kümesinin yapılandırma veritabanı oldukça sık değişir, bu nedenle sık sık yedekleme yapmanız önerilir. Kuruluşunuza ne kadar sık yeni kullanıcı eklenirse o kadar sık yedekleme yapmanız gerekir. Kök sertifika sunucunuzu yedekliyorsanız, yedeğinize asıl veritabanındaki **sysmessages** tablosunu eklediğinizden de emin olmalısınız Bu tablo RMS'ye özgü iletileri içermiyorsa, kök sertifika sunucusu çalışamaz ve hata verir. Bu tablo yedekte yoksa, varolan veritabanı kullanılarak sağlama işleminin yinelenmesi yoluyla yeniden oluşturulabilir.

RMS günlük veritabanı, sorun gidermeye yönelik ve istatistik amaçlı ilgi çekici veriler sağlayan kayıtlar içerir, ancak bu veritabanı RMS sistemi açısından kritik düzeyde önemli değildir. Dizin Hizmetleri veritabanı Active Directory veritabanının yerel önbelleği olduğundan, RMS sistemini geri yüklediğinizde otomatik olarak yeniden oluşturulur. RMS veritabanlarınızı yedeklemek üzere bir plan yapmak için SQL Server yöneticinize başvurun.

RMS özel anahtarlarını korumak için bir donanım güvenlik modülü kullanıyorsanız, donanım güvenlik modülü yapılandırmasını da yedeklemeniz gerekir. Donanım güvenlik modülü yapılandırmasının nasıl yedekleneceği ve geri yükleneceği hakkında daha fazla bilgi için donanım güvenlik modülü belgelerine bakın.

| ![](/security-updates/images/Cc747745.note(WS.10).gif)Not                                                                                                                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS özel anahtarlarını şifrelemek için varsayılan yazılım tabanlı şifreleme hizmet sağlayıcısından (CSP) farklı bir yazılım tabanlı CSP'yi kullandıysanız, RMS ile birlikte kullanmadan önce kuruluş anahtar yönetimi uygulamalarının (yedekleme ve geri yükleme yordamları gibi) yerinde olduğundan emin olun. |

RMS Sistemini Geri Yüklemeyi Planlama
-------------------------------------

Veritabanı sunucusunu yedekten geri yüklüyorsanız, çalışan RMS sürümünün yedek oluşturulduğunda çalışmakta olan sürümle aynı olduğundan emin olun. RMS sistemi kullanıcılarını, RMS sistemini yedekleme tarihinden sonra kullanmaya başladılarsa yeni bir hak hesabı sertifikası almaları gerekeceği konusunda uyarın. Bunun sonucunda korumalı içerik kaybı olmaz.

Kümeden tek bir RMS sunucusunu geri yüklemek için sunucuyu yeniden oluşturun, RMS'yi yeniden yükleyin ve varolan veritabanını kullanarak sunucuyu kümeye ekleyin. Kümelenmiş sunucular tek bir sunucu gibi çalıştığından, bu etkinlik RMS sistemi kullanıcılarını etkilemez.
