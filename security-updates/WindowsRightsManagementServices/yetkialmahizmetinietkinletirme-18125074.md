---
TOCTitle: Yetki Alma Hizmetini Etkinleştirme
Title: Yetki Alma Hizmetini Etkinleştirme
ms:assetid: '45226e85-b50d-41cc-aca7-0f603f8509d5'
ms:contentKeyID: 18125074
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720261(v=WS.10)'
---

Yetki Alma Hizmetini Etkinleştirme
==================================

RMS sisteminin yetkisini alma işlemi, tüm yayımlanan bilgileri korumak için kullanılan özel anahtarı gerektirir. Bu özel anahtar yapılandırma veritabanında depolanır, Veri Koruma API'si (DPAPI) tarafından şifrelenir ve sağlama sırasında girilmiş olan şifreyi temel alır. RMS özel anahtarı bir donanım güvenlik modülünde (HSM) depolanırsa, özel anahtar, yapılandırma veritabanı yerine HSM'de depolanır.

| ![](images/Cc720261.Caution(WS.10).gif)Dikkat                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS sisteminin yetkisini almadan önce, özel anahtar parolanızı bildiğinizden emin olun. Bu parolayı bilmiyorsanız, RMS sunucusunun yetkisini almadan önce özel anahtarı sıfırlamalısınız. |

RMS sistemini kaldırmak için önce kümedeki sunucunun yetkisi alınır. Yetki alma bir lisans işlevi olduğundan, alt kayıtlı RMS lisans kümesindeki bir sunucunun yetkisi, RMS kök kümesini veya başka bir alt kayıtlı RMS lisans kümesini etkilemeden alınabilir. Bu nedenle, RMS kök kümesinin ve lisans kümelerinin yetkisini ayrı ayrı almalısınız; çünkü her lisans kümesi yayımlama lisansı oluşturmak için kendi özel anahtarını kullanır.

Yetki alma hizmetini etkinleştirmek için aşağıdaki yordamı kullanın:

1.  Windows RMS Yönetimi Web sitesini açın.
2.  **RMS'yi Yönet**'i tıklatın ve ardından **Güvenlik Ayarları**'nı tıklatın.
3.  **RMS yüklemesinin yetkisinin alınmasını etkinleştirin** onay kutusunu işaretleyin.
4.  Yetki alma işlemini onaylamanızı isteyen bir iletişim kutusu görüntülendiğinde **Tamam**'ı tıklatın.

Bir sunucunun yetkisini aldığınızda, standart RMS yapılandırmasına geri yüklenemez. Bu yordam geri alınamaz.

RMS'nin yetkisi alındıktan sonra, başka bir RMS örneği yüklemeyi denemeden önce **Program Ekle veya Kaldır** kullanılarak RMS'nin tamamen kaldırılmış olması gerekir.
