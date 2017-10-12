---
TOCTitle: Yönetim Giriş Sayfasını Kullanma
Title: Yönetim Giriş Sayfasını Kullanma
ms:assetid: '6c155977-bd0e-47d6-ac65-1746cddb505e'
ms:contentKeyID: 18125125
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720290(v=WS.10)'
---

Yönetim Giriş Sayfasını Kullanma
================================

**Yönetim Giriş** Web sayfasından, sunucu veya küme hakkındaki bilgileri görüntüleyebilir ve yönetim seçeneklerine erişebilirsiniz. Bu sayfa yalnızca sunucu hazırlandıktan sonra kullanılabilir.

Yönetmek istediğiniz sunucudan bu Web sayfasına erişmek için aşağıdaki adımları izleyin:

1.  Yerel yönetici olarak oturum açın.
2.  **Başlat**'ı tıklatın, **Tüm Programlar**'ın ardından **Windows RMS**'nin üzerine gelin ve **Windows RMS Yönetimi**'ni seçin.
3.  **Genel Yönetim** sayfasından, **RMS'yi bu Web sitesinde yönet**'i tıklatın.

Güvenli Yuva Katmanı'nı (SSL) kullanarak uzaktan yönetimi etkinleştirdiyseniz, aşağıdaki adımları izleyerek **Yönetim Giriş** sayfasına farklı bir bilgisayardan da erişebilirsiniz:

1.  Web tarayıcınızın adres çubuğuna aşağıdaki URL'yi yazın:
    https://*küme\_adı:bağlantı\_noktası\_numarası*/\_wmcs/admin
    *küme\_adı:bağlantı\_noktası\_numarası* hazırlık sırasında bu küme için belirttiğiniz URL'dir. Bağlantı noktası numarasını yalnızca varsayılan bağlantı noktası olan 80'den farklı bir bağlantı noktası numarası belirttiyseniz verin.
2.  İstendiğinde, erişmekte olduğunuz sunucudaki bir yerel yöneticinin kimlik bilgilerini yazın.

**Yönetim Giriş** sayfasında küme URL'si, yapılandırma veritabanı adı ve konumu, sunucu lisans sahibi sertifikası son kullanım tarihi gibi küme hakkındaki bilgiler görüntülenir. Bu sayfada, küme için aşağıdaki yönetim seçeneklerini yapılandırabileceğiniz sayfalara bağlantılar da verilir:

-   **Güven ilkeleri.** Güvenilen etki alanları ekleme ve kaldırma. Daha fazla bilgi için bu konuda daha sonra yer alan "[Güven ve Güven İlkesini Yönetme](https://technet.microsoft.com/1c96ee74-fd28-4511-be21-087e2b04c3ee)" bölümüne bakın.
-   **Hak ilkesi şablonları**. Hak ilkesi şablonlarını oluşturun ve değiştirin. Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Yönetme](https://technet.microsoft.com/718286dc-3399-4556-96c9-ec3a33d31877)" bölümüne bakın.
-   **Günlük ayarları**. Günlüğü açıp kapatın ve günlük sunucusunun ve veritabanının adını görüntüleyin. Daha fazla bilgi için bu konuda daha sonra yer alan "[Günlüğü Yönetme](https://technet.microsoft.com/8fccfc57-2135-494e-8e44-f6191bf5e4a0)" bölümüne bakın.
-   **Extranet küme URL'si ayarları.** Lisans ve hesap sertifikası istekleri için kullanılabilir bir dış URL belirtin. Daha fazla bilgi için bu konuda daha sonra yer alan "[Extranet URL'sini Yapılandırma](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572)" bölümüne bakın.
-   **RMS proxy ayarları.** Proxy sunucusunun adresini, kimlik doğrulama türünü ve RMS sunucusunun bir proxy sunucusu üzerinden Internet'e bağlanması gerektiğinde kullanılacak kullanıcı adını belirtin. Daha fazla bilgi için bu konuda daha sonra yer alan "[RMS Proxy Ayarlarını Yapılandırma](https://technet.microsoft.com/179d2970-62e9-4487-aa5b-f4334234991e)" bölümüne bakın.
-   **Güvenlik ayarları.** Sunucu özel anahtar parolasını sıfırlayın, üyelerinin tüm lisanslı içeriğin şifresini çözebildiği ve RMS'nin yetkisini aldığı Super Users grubunu belirtin. Daha fazla bilgi için bu konuda daha sonra yer alan "[RMS Çalıştırırken Güvenliği Yönetme](https://technet.microsoft.com/62050812-de4f-4392-8d63-f2f89aa01ed4)" bölümüne bakın.
-   **Sertifika ayarları.** Hak hesabı sertifikalarının geçerlilik dönemini ve yönetim ilgili kişisini belirtin. (Bu seçenek yalnızca kök sertifika kümesinde kullanılabilir, lisans sunucularında kullanılamaz.) Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak Hesabı Sertifikalarını Yönetme](https://technet.microsoft.com/49c5c2ba-e197-4e4b-b3b3-b3248f068bcc)" bölümüne bakın.
-   **Dışlama ilkeleri.** Kasa sürümünü, hak hesabı sertifikasını, Windows sürümünü veya RMS etkin uygulamayı temel alan bir dışlama ilkesi belirtin. Daha fazla bilgi için bu konuda daha sonra yer alan "[Dışlama İlkesini Yönetme](https://technet.microsoft.com/ee31e099-e095-4648-95da-0009fbeb48cb)" bölümüne bakın.
-   **RM hesap sertifikası raporu.** Verilen hak hesabı sertifikası sayısını görüntüleyin. (Bu seçenek yalnızca kök sertifika kümesinde kullanılabilir, lisans sunucularında kullanılamaz.) Daha fazla bilgi için bu konuda daha sonra yer alan "[Hak Hesabı Sertifikalarını İzleme](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)" bölümüne bakın.

Bu bölümdeki kalan konularda bu özelliklerin nasıl kullanılacağı açıklanmaktadır. Adım adım yönergeler için bu konuda daha sonra yer alan "[RMS - Nasıl yapılır?](https://technet.microsoft.com/82032075-f361-438f-a2c4-93ab29ae6cff)" bölümüne bakın.

| ![](images/Cc720290.note(WS.10).gif)Not                                                                                                                                                                                                                     |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS Yönetim Web sitesi bazı özelliklerin yapılandırılması için açılır pencereler kullanır. Web tarayıcınız ile birlikte açılır pencere engelleyicisi kullanıyorsanız, tarayıcı ayarlarınızı RMS Yönetim Web sitesinin açılır pencerelerine izin verecek şekilde yapılandırmanız gerekir. |
