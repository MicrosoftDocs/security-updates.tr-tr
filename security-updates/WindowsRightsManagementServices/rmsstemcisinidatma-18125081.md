---
TOCTitle: RMS İstemcisini Dağıtma
Title: RMS İstemcisini Dağıtma
ms:assetid: '4b8dd930-4105-4e73-918c-12d2b05d5fb5'
ms:contentKeyID: 18125081
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720266(v=WS.10)'
---

RMS İstemcisini Dağıtma
=======================

RMS istemcisi Windows Vista® işletim sisteminde yerleşik olarak bulunduğu için, ayrı bir yükleme olarak yüklenmesi gerekmez. Windows Vista öncesindeki işletim sistemlerinde, RMS istemci yazılımının yüklenmesi ve daha sonra etkinleştirilmesi gerekiyordu.

Etkinleştirme işlemi oturum açmış olan kullanıcı için bir kasa ve bilgisayar sertifikası oluşturur. Etkinleştirme yerel bir işlemdir ve ağ bağlantısı gerektirmez. Etkinleştirme başarılı olduğunda, RMS etkin bir uygulama tarafından bir kullanım lisansı ilk istendiğinde kullanıcı için bir kullanıcı sertifikası sağlanır. Grup İlkesi, Windows Update veya bir yönetimsel komut dosyası kullanılarak kuruluştaki her istemci bilgisayara RMS istemcisi yüklenebilir.

| ![](images/Cc720266.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Hangi istemci dağıtma yöntemi kullanılırsa kullanılsın, RMS istemcisi, RMS sunucusuyla iletişim kurmak için varsayılan olarak 80 numaralı bağlantı noktasını veya 443 numaralı bağlantı noktasını kullanır. İstemci bilgisayarın bu bağlantı noktalarından RMS köküne ve yalnızca lisanslı kümelere giden isteklerde bulunabildiğinden emin olmanız gerekir. |

**Grup İlkesi Kullanma**

Kuruluşunuz yazılımları Grup İlkesi kullanarak dağıtıyorsa, RMS istemcisini yükseltilmiş ayrıcalıklarla dağıtmak için bu yöntemi kullanabilirsiniz. RMS istemcisi bu yolla dağıtılırsa, kullanıcının yönetici ayrıcalıklarına sahip olması gerekmez ve **Denetim Masası**'ndaki **Program Ekle veya Kaldır**'ı kullanarak veya RMS etkin bir uygulamadan haklarla korunan içeriği açarak RMS istemcisini yükleyebilir.

**Windows Update'i Kullanma**

Windows Update bir bilgisayara RMS istemcisi yüklemenin en kolay yolunu sağlar. Bu yöntem kullanıcının tanıdığı bir yöntem kullanıldığı için yararlıdır, ancak RMS istemcisini yükleyen kullanıcının bilgisayarda yerel yönetici hakları olmasını gerektirir.

**Komut Dosyasıyla Yüklemeyi Kullanma**

İstemci yüklemesi işlemi üzerinde en yüksek düzeyde denetime sahip olmak için, yazılımı edinebilir ve yükleme işleminin her adımında bir komut dosyası çalıştırarak bütünlüğünü doğrulayabilirsiniz. Bu komut dosyası yazılarak bir Grup İlkesi Nesnesi'ne (GPO) başlangıç komut dosyası olarak eklenebilir. Bu yöntem kullanıldığında, kullanıcının bilgisayarda bir yerel yönetici olması gerekmez ve önyükleme sonrasında RMS istemcisi otomatik olarak yüklenir.

        ```
RMS istemcisini Grup İlkesi kullanarak dağıtma konusunda temel bilgiler için, bu konuda daha sonra yer alan [İstemci Dağıtımını Desteklemek için SMS veya Grup İlkesi Kurma](https://technet.microsoft.com/9e37c27b-8cc1-40c6-adb7-0937aa64c8db) bölümüne bakın.

RMS istemci dağıtımı hakkında yordam yardımı için, bu konuda daha sonra yer alan [RMS İstemcisi Nasıl Dağıtılır?](https://technet.microsoft.com/c84f1724-cf71-4385-9003-ff68bc23c927) bölümüne bakın.
