---
TOCTitle: Yapılandırma Veritabanında Değişiklikler Yapma
Title: Yapılandırma Veritabanında Değişiklikler Yapma
ms:assetid: '6a7bec73-09e4-4060-b551-5990836df4bc'
ms:contentKeyID: 18125128
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747606(v=WS.10)'
---

Yapılandırma Veritabanında Değişiklikler Yapma
==============================================

Yönetim Web sitesini kullanarak yaptığınız yapılandırma değişiklikleri, sunucu veya kümeye yönelik yapılandırma veritabanına yansıtılır. Yapılandırma veritabanındaki verileri el ile değiştirmek yerine yönetim Web sitesinden yapılandırma ayarlarını değiştirmeniz ısrarla önerilir. Ancak veritabanında el ile değişiklik yapmanızı gerektirebilecek iki durum vardır:

-   **Günlük veritabanını farklı bir sunucuya taşıma.** Günlük veritabanı varsayılan olarak yapılandırma veritabanıyla aynı sunucuya yüklenir. Günlük veritabanını farklı bir sunucuya taşımaya karar verirseniz, yapılandırma veritabanını yeni konuma başvuracak şekilde değiştirmeniz gerekir. Yapılandırma veritabanının yeni konumla nasıl güncelleştirileceği de dahil olmak üzere günlük veritabanını taşıma hakkında daha fazla bilgi için, bu konuda daha önce geçen "[Günlük Veritabanının Yerini Değiştirme](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)" bölümüne bakın.
-   **Hak hesabı sertifikalarıyla ilişkili kullanıcı anahtarlarını kaldırma**. Active Directory'den bir kullanıcı hesabını kaldırdığınızda veya yönetim Web sitesini kullanarak bir hak hesabı sertifikasını dışladığınızda veya iptal ettiğinizde, hak hesabı sertifikasıyla ilişkili kullanıcı anahtarları yapılandırma veritabanından kaldırılmaz. Etkin olmayan kullanıcı anahtarlarını, hem güvenlik nedeniyle hem de istemci erişim lisanslarının (CAL) sayısını izlemeye yardımcı olması için yapılandırma veritabanından kendiniz kaldırmalısınız. Kullanıcı anahtarlarını yapılandırma veritabanından kaldırma hakkında daha fazla bilgi için bu konuda daha önce geçen "[Kullanıcı Hesaplarını Silme](https://technet.microsoft.com/bf73b141-d4d1-4807-a773-3aaff58b0db6)" bölümüne bakın. CAL'leri izleme hakkında daha fazla bilgi için bu konuda daha önce geçen "[Hak Hesabı Sertifikalarını İzleme](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)" bölümüne bakın.

Doğrudan yapılandırma veritabanında değişiklik yapma gereksinimi duyarsanız, veritabanı sunucusu yöneticinize başvurun.
