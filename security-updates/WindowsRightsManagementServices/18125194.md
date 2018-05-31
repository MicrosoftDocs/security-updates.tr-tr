---
TOCTitle: İstemci Dağıtımını Desteklemek için SMS veya Grup İlkesi Kurma
Title: İstemci Dağıtımını Desteklemek için SMS veya Grup İlkesi Kurma
ms:assetid: '9e37c27b-8cc1-40c6-adb7-0937aa64c8db'
ms:contentKeyID: 18125194
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747703(v=WS.10)'
---

İstemci Dağıtımını Desteklemek için SMS veya Grup İlkesi Kurma
==============================================================

RMS'yi dağıttığınızda, kullanıcıların içeriği koruyabilmesi ve RMS korumalı içeriği kullanabilmesi için bilgisayarlarında RMS etkin bir uygulamanın yüklü olması gerekir.

Bir uygulamanın RMS etkin olması için, RMS istemcisini kendi işlemleriyle tümleştirmesi gerekir. Windows Vista® öncesinde, RMS istemcisi Microsoft Yükleme Merkezi'nden karşıdan yüklenebilen ayrı bir Windows bileşeni olarak edinilebilir. Ancak, istemciyi kuruluşunuzdaki her bilgisayar için ayrıca karşıdan yüklemek istemiyorsanız, RMS istemcilerinin istemci bilgisayarlara dağıtılmasını otomatikleştirmek için Microsoft Systems Management Server'ı (SMS), Grup İlkesini veya komut dosyalarını kullanabilirsiniz.

| ![](/security-updates/images/Cc747703.Important(WS.10).gif)Önemli                          |
|-------------------------------------------------------------------------------------------------------|
| RMS istemcisi Windows Vista ile tümleşiktir. Bu nedenle, ayrı bir yükleme olarak yüklenmesi gerekmez. |

RMS istemcisini dağıtmak için SMS'yi kullandığınızda, aşağıdakileri yapmanız gerekir:

-   Yeni bir paket tanım dosyası oluşturun.
-   WindowsRightsManagementServicesSP2-KB917275-Client-TRK.exe dosyasından Windows Installer dosyalarını ayıklayın. Bunu yapmak için, önce WindowsRightsManagementServicesSP2-KB917275-Client-TRK.exe dosyasını kaydedin. Bunu yüklemeyin. Bu örnekte, dosyanın c:\\klasör\_adı dizinine kaydedildiğini varsayalım. Komut istemi penceresini açın ve aşağıdaki komutu yazın:
    `c:\folder_name\WindowsRightsManagementServicesSP2-KB917275-Client-ENU.exe /x/t:c:\folder_name`
    Bu komut MSDrmClient.msi ve RMClientBackCompat.msi dosyalarını .exe dosyasından ayıklar ve bunları c:\\*klasör\_adı* klasörüne yerleştirir.
-   Paket tanımı ve kaynak için Windows Installer dosyalarını kullanın.
-   Ağınızda paketlerin kullanılabilirliğini bildirin.

| ![](/security-updates/images/Cc747703.note(WS.10).gif)Not                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Yazılımı yükleyebilmek için yönetici hakları gerekir; kuruluşunuzun güvenlik ilkesi RMS istemci yazılımını bir sistem yöneticisinin yüklemesini gerektirebilir. |

Yazılım dağıtmak için SMS'yi kullanma hakkında daha fazla bilgi için, Systems Management Server 2003 Kavramları, Planlama ve Dağıtım Kılavuzu'na ([http://go.microsoft.com/fwlink/?LinkID=32972](http://go.microsoft.com/fwlink/?linkid=17401)) bakın.

İstemci yazılımını Grup İlkesi kullanarak dağıtma hakkında daha fazla bilgi için, Grup İlkesi tabanlı yazılım dağıtımı hakkındaki konulara ([http://go.microsoft.com/fwlink/?LinkID=32972](http://go.microsoft.com/fwlink/?linkid=38997)) bakın.
