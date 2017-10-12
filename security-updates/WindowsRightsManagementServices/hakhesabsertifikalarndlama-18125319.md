---
TOCTitle: Hak Hesabı Sertifikalarını Dışlama
Title: Hak Hesabı Sertifikalarını Dışlama
ms:assetid: 'cba5e901-942c-4d06-9865-e6c4648c95e6'
ms:contentKeyID: 18125319
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747670(v=WS.10)'
---

Hak Hesabı Sertifikalarını Dışlama
==================================

Kullanıcı güvenilir olduğu halde RMS kimlik bilgileri kuşkuluysa, kullanıcının ortak anahtarını dışlayarak hak hesabı sertifikasını dışlayabilirsiniz. Bunu yaptığınız zaman, RMS o hak hesabı sertifikasıyla ilgili yeni kullanım lisansı isteklerini reddeder. Hak hesabı sertifikasını dışladıktan sonra kullanıcı yeni içerik için yeni bir kullanım lisansı almayı denediğinde istek reddedilir. Kullanıcı, yeni kullanım lisansı almak için yeni anahtar çiftli bir hak hesabı sertifikası almak zorundadır.

Hak hesabı sertifikaları, yönetim Web sitesinin **Dışlama ilkeleri** sayfası kullanılarak dışlanabilir. Bir kullanıcının hak hesabı sertifikasını dışladığınızda, RMS, kök sertifika kümesinin yapılandırma veritabanının DRMS\_GicExclusionList tablosuna dışlanan anahtarı, kullanıcı hesabının adını ve dışlama tarih ve saatini ekler. Bu bilgiler yönetim Web sitesinin **Dışlama ilkeleri** sayfasında da görüntülenir. Ayrıca, RMS dışlanan hesap sertifikasıyla ilişkili ortak ve özel anahtarları yapılandırma veritabanının UD\_Users tablosundan siler.

Kök sertifika sunucusu veya kümesindeki bir hak hesabı sertifikasını dışlamak için, kullanıcı etki alanı hesabını kök sertifika sunucusunun **Dışlama ilkeleri** sayfasında belirtin. Hak hesabı sertifikasını her sunucunun yönetim Web sitesindeki alt kayıtlı sunucularda dışlamanız gerekir. Kullanıcıyı alt kayıtlı lisans sunucusu veya kümesinde dışlamak için, lisans sunucusu yönetim Web sitesinin **Dışlama ilkeleri** sayfasına hak hesabı sertifikasının ortak anahtar değerini girin. Bu değer kök sertifika kümesi yönetim Web sitesinin **Dışlama ilkeleri** sayfasından alınabilir.

Çok kümeli bir RMS dağıtımında hak hesabı sertifikası dışlama işlemini basitleştirmek için kök sertifika kümesinin yapılandırma veritabanındaki DRMS\_GicExclusionList tablosunu her lisans kümesi yapılandırma veritabanına kopyalayabilirsiniz. Bunu yaparsanız, ortak anahtar değerini her sunucuya tek tek girmeniz gerekmez.
