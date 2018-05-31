---
TOCTitle: Microsoft Operations Manager ile İzleme
Title: Microsoft Operations Manager ile İzleme
ms:assetid: 'ce372598-7421-4f1f-b8eb-f62da26e85d1'
ms:contentKeyID: 18125317
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747758(v=WS.10)'
---

Microsoft Operations Manager ile İzleme
=======================================

RMS, Microsoft® Operations Manager (MOM) ile kullanabileceğiniz bir yönetim paketi içerir. MOM, aşağıdakileri yaparak kuruluşunuzdaki sunucu işlemlerini yönetmenize yardımcı olabilir:

-   RMS tarafından Uygulama olay günlüğüne yerleştirilen olayları izleme.
-   Hızlı bir şekilde düzeltici veya önleyici eylemlerde bulunabilmeniz için olası hizmet dışı kalma veya yapılandırma sorunlarını gösteren olayları vurgulama.
-   Sunucu lisans sertifikası süresinin sonu veya Web hizmeti hatası gibi durumlara yönelik uyarı ve hataları bildirme.

RMS ile birlikte, RMS yönetim (RMS\_MOMPack.akm) paketi %programfiles%\\Windows Rights Management Services\\Tools konumuna yüklenir.

Bu yönetim paketi, RMS yöneticisinin RMS sunucu dağıtımını yönetmesine yardımcı olması için kullanılabilecek aşağıdaki kural kümelerini içerir.

**RMS MOM Yönetim Paketi Kuralları**

1.  PMC Önlemi - Etkinleştirme Proxy toplam hata sayısı
2.  PMC Önlemi - Etkinleştirme Proxy Toplam süre
3.  PMC Önlemi - Etkinleştirme Toplam İşlem Süresi
4.  PMC Önlemi - Etkinleştirme Toplam İstekler
5.  PMC Önlemi - Etkinleştirme Proxy toplam istekler
6.  PMC Önlemi - AD önbellek (DB önbelleği) isabetleri
7.  PMC Önlemi - AD önbellek (DB önbelleği) isabetsizlikleri
8.  PMC Önlemi - Ortalama Lisans İşleme süresi
9.  Olay - Yapılandırma Bilgisi bozulması
10. PMC Önlemi - Ölü GC bağlantıları
11. PMC Önlemi - Kayıt hataları
12. Olay - Genel Hata
13. Olay - Başlangıç Hatası
14. Olay - Lisans Sert süresi doldu
15. Olay - Lisans Sert İsteği Hatası
16. Olay - Günlük hizmeti hatası
17. PMC Önlemi - Kullanılabilir en fazla GC bağlantısı
18. Olay - Eksik Lisans Alma Noktası oluşturma eklentisi
19. PMC Önlemi - Tüm RM sunucularındaki MSMQ Kuyruk uzunluğu
20. Olay - Kullanılabilir GC yok
21. Olay - Eklenti Başlangıç Hatası
22. Olay - Özel Anahtar koruma parolası değiştirildi
23. Olay - RM Sunucusu Kapalı
24. Olay - RM Sunucusu Kapatma Hatası
25. Olay - Sunucu Başlatma Hatası
26. PMC Önlemi - Alt kayıt hataları
27. Olay - SuperUser ayrıcalıklı geçersiz kılma yetkisi kullanıldı
28. PMC Eşiği - Çok fazla GetLicensorCert hatası
29. Olay - Yaklaşan Sert Son Kullanım Tarihi - 1 Ay
30. Olay - Yaklaşan Sert Son Kullanım Tarihi - 1 Hafta

Kuruluşunuzda MOM yönetim paketlerini nasıl dağıtacağınız hakkında daha fazla bilgi için bkz: [Microsoft Web sitesi](http://www.microsoft.com/) (http://www.microsoft.com/).
