---
TOCTitle: Sertifika ve Lisans Desteği için Sunucu Ekleme
Title: Sertifika ve Lisans Desteği için Sunucu Ekleme
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18124997
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720189(v=WS.10)'
---

Sertifika ve Lisans Desteği için Sunucu Ekleme
==============================================

RMS için kök yüklemeyi oluşturmak üzere ilk sunucuyu yükledikten ve yapılandırdıktan sonra, sertifika ve lisans hizmetleri için aşağıdaki genişletilmiş desteği sağlamak amacıyla ek sunucular kurabilirsiniz:

-   Bir sunucuyu, ek sertifika ve lisans desteği sağlamak için kök sertifika kümesi üyesi olarak ekleyebilirsiniz. Bu kümeye eklenen bir sunucu, kök sertifika sunucusuyla aynı yapılandırmayı ve aynı veritabanlarını kullanır.
-   Lisans sunucusunu kendi başına veya lisans sunucusu kümesinin üyesi olarak kurabilirsiniz. Kök sertifika kümesinin altına kaydettirilir ve sunucu lisans sertifikasını (SLC) kök sertifika sunucusunun sertifika hizmetleri aracılığıyla alır. Lisans sunucusuna gönderilen, sertifika hizmetlerine ilişkin tüm istemci istekleri sertifika sunucusuna iletilir. Lisans sunucusu kök sertifika sunucusuna istek göndermeden kullanım lisanslarını ve yayımlama lisanslarını verebilir.

Dağıtmaya karar verdiğiniz seçenek kuruluşunuzun büyüklüğüne ve artıklığı, ölçeklemeyi, yük dengeleme desteğini ve güvenliği nasıl uygulamak istediğinize bağlıdır. Artan sayıda sertifika, lisans ve yayımlama isteğini karşılamak amacıyla ek RMS sunucuları dağıtıyorsanız, RMS sunucularını kök sertifika kümesinin parçası olarak dağıtmalısınız; böylece artıklık ve yük dengelemeyi tüm sunucular için ayarlayabilirsiniz. Sertifika sunucularıyla küme oluşturabilir ve lisans sunucularını (bunlar da yük dengelemesi için kümelenebilir) bunların altına kaydettirerek lisanslama ve yayımlama hizmetleri işlemlerinin yükünü aktarabilirsiniz, ancak kök sertifika kümesinin altına kaydettirilmiş lisans kümesinin yükünü dengeleyemezsiniz.

Aşağıdaki konularda bu görevle ilgili yardım sağlanmaktadır:

-   [Yükleme ve Sağlama için Gerekli Roller, İzinler ve Haklar](#bkmk_1)
-   [Ek Sertifika ve Lisans Sunucuları için Sağlama İşlemleri](#bkmk_2)
-   [Kümeleri ve Yük Dengelemesini Ayarlama](#bkmk_3)

<span id="BKMK_1"></span>
Yükleme ve Sağlama için Gerekli Roller, İzinler ve Haklar
---------------------------------------------------------

Ek sunucular yüklemek ve bunları yapılandırmak için, ilk sunucuyu kurmak için gerekenlerle aynı rollere, izinlere ve haklara gereksinim duyarsınız. Bunun yanında, ayrı bir lisans sunucusu kurmak için kök sertifika sunucusundan izin almanız gerekir ve bu işlem alt kayıt olarak adlandırılır. Kök sertifika sunucusu SubEnrollService.asmx dosyasının DACL'si aracılığıyla denetlenir. Kök sertifika sunucusunu yapılandırırken belirttiğiniz RMS hizmet hesabı da dahil olmak üzere RMS Service Group üyelerinin alt kayıt gerçekleştirme izni vardır. Daha fazla bilgi için, bu konuda daha önce yer alan “[İlk Sunucuda Sertifika ve Lisans Hizmetlerini Kurma](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b)” bölümüne bakın.

<span id="BKMK_2"></span>
Ek Sertifika ve Lisans Sunucuları için Sağlama İşlemleri
--------------------------------------------------------

Sertifika ve lisans kümelerine sunucu ekleme, sunucunun sağlama işlemini tamamlamasını gerektirir. Sağlama işlemi, bu işlemi gerçekleştirdiğiniz sunucunun türüne göre farklılık gösterir.

-   Ayrı bir lisans sunucusu sağlıyorsanız yapılandırma veritabanını, RMS hizmet hesabını, küme URL'sini ve özel anahtar koruma bilgilerini, bir kök sertifika sunucusu için belirttiğiniz şekilde belirtin. Bununla birlikte, bir sunucu lisans sertifikası iptal ilkesi belirtmezsiniz; bu ilke kök sertifika sunucusu tarafından denetlenir.
-   Sunucuyu küme üyesi olarak sağlıyorsanız, sağlama işlemi sırasında belirtmeniz gereken bilgiler yalnızca RMS hizmet hesabı, yapılandırma veritabanı ve özel anahtar koruması için paroladır (veya varolan kümeyle aynı CSP'yi ve özel anahtarı kullanın). Kümedeki tüm sunucular aynı sunucu lisans sertifikası ve sunucu anahtar çiftini paylaşır.

| ![](/security-updates/images/Cc720189.Important(WS.10).gif)Önemli                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------|
| RMS kurulumunu ilk sunucuda, yükleme ve sağlama işlemini içerecek şekilde tamamlamadan önce diğer sunuculara RMS yüklemeye başlamayın. |

Ek sunucu yüklendikten ve sağlandıktan sonra otomatik olarak küme üyesi olarak yapılandırılır. Ancak, yük dengelemesi uyguladıysanız, yük dengelemesi yazılımını yeni sunucuyla çalışmak üzere yapılandırmanız gerekir

<span id="BKMK_3"></span>
Kümeleri ve Yük Dengelemesini Ayarlama
--------------------------------------

RMS, sunucu kümelerini destekleyecek şekilde tasarlanmıştır. RMS sunucusu kümeleri oluşturulması, RMS dağıtımınız için daha fazla ölçeklenebilirlik, güvenilirlik ve yük dengelemesi sağlar.

**Küme Oluşturma**

Küme ayarlama işlemine bir kök sertifika sunucusu veya lisans sunucusuyla başlayın. Her kümedeki ikinci ve sonraki sunucular için yeni sunucuya RMS yükleyin, **Genel Yönetim** sayfasına gidin ve sonra gerekli kaynakları sağlamak ve sunucuyu kök sertifika kümesine veya lisans kümesine eklemek için **Bu sunucuyu bir kümeye ekle**'yi tıklatın.

Sunucuyu eklemek istediğiniz kümenin veritabanı adını belirtin.

**Yük Dengeleme Kümeleri**

RMS otomatik olarak yük dengelemesi uygulamaz. Tüm RMS sunucuları üzerindeki yükü dengelemek için Ağ Yükü Dengelemesi de dahil olmak üzere donanım veya yazılım yükü dengelemesi kullanabilirsiniz.

Aşağıdaki başlıklarda bu konuyla ilgili ek ayrıntılar sağlanmaktadır:

-   Sertifika ve lisans hizmetleri arasındaki farklar hakkında daha fazla bilgi için, bu belge grubundaki “RMS Teknik Başvuru Kılavuzu” bölümünde bulunan “RMS Sistemine Genel Bakış” konusuna bakın.
-   Sunucu dağıtımlarının kuruluşunuzun kullanılabilirlik ve performans gereksinimleriyle nasıl eşleneceği konusunda daha fazla bilgi için, bu belge grubundaki “RMS Dağıtımı Planlama” bölümünde bulunan “Artıklık ve Yük Dengelemesi Sağlama” konusuna bakın.
-   Kuruluşunuzda RMS dağıtımını desteklemek için gereken sunucu sayısının nasıl belirleneceği hakkında daha fazla bilgi için, bu belge grubundaki “RMS Dağıtımı Planlama” bölümünde bulunan “Ölçeklendirme Gereksinimlerini Değerlendirme” konusuna bakın.
-   RMS dağıtımınızla BT güvenliğinin nasıl uygulanacağı konusunda daha fazla bilgi için, bu konunun sonraki bölümlerinde yer alan “[RMS Dağıtımının Güvenliğini Sağlama](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14)” konusuna bakın.
-   RMS'nin nasıl yükleneceği konusunda bilgi almak için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “RMS Service Pack 1'i Yüklemek için” konusuna bakın.
    RMS'yi komut isteminden de yükleyebilirsiniz. Daha fazla bilgi için bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "RMS'yi Komut İsteminden Yükleme" konusuna bakın.
-   Lisans sunucusunun nasıl hazırlanacağı konusunda bilgi almak için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “Lisans Sunucusu Hazırlamak İçin” konusuna bakın.
-   Kümedeki ek sunucuların nasıl sağlanacağı konusunda bilgi almak için, bu belge grubundaki “RMS Sunucusunu Çalıştırma” bölümünde bulunan “Kümeye Sunucu Eklemek İçin” konusuna bakın.
