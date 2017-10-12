---
TOCTitle: 'RMS''yi Kaldırma ve Yapılandırmasını Geri Alma'
Title: 'RMS''yi Kaldırma ve Yapılandırmasını Geri Alma'
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18125270
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747753(v=WS.10)'
---

RMS'yi Kaldırma ve Yapılandırmasını Geri Alma
=============================================

Çeşitli nedenlerden dolayı, bir sunucudan RMS'yi kaldırmak isteyebilirsiniz. Kök sertifika sunucusu için ilk adım sunucu üzerinde bulunan RMS'nin yapılandırmasını geri almaktır. Bu işlemi, yapılandırmasını geri almak istediğiniz sunucunun **Genel Yönetim sayfasındanRMS'yi bu Web sitesinden kaldır**'ı tıklatarak yapabilirsiniz. RMS'yi kaldırmadan önce lisans sunucusunun yapılandırmasını geri almanız gerekmez.

| ![](images/Cc747753.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Active Directory ormanındaki son kök sertifika sunucusunun yapılandırmasını geri aldığınızda hizmet bağlantı noktası nesnesi Active Directory'den kaldırılır. RMS'yi kaldırmadan önce bu sunucunun yapılandırmasını geri almazsanız, hizmet bağlantı noktası nesnesini Active Directory'den el ile kaldırana kadar bu ormanda yeni bir kök sertifika sunucusu sağlayamazsınız. |

Ardından, RMS'yi kaldırın.

Tek başına çalışan bir sunucu veya kümede bulunan son sunucudan RMS'yi ve yapılandırmasını kaldırdığınızda, Dizin Hizmetleri veritabanı da kaldırılır. Yapılandırma ve günlük veritabanları kaldırılmaz; ancak, sunucuda RMS'yi yükseltir veya yeniden yüklerseniz, yeni bir günlük veritabanı günlük veritabanının üzerine yazılır.

Bir kümede bulunan sunucudan RMS'yi ve yapılandırmasını kaldırdığınızda kümenin yapılandırma, günlük ve dizin hizmetleri veritabanları kaldırılmaz. Ancak, yapılandırma veritabanının DRMS\_ClusterServer tablosu sunucunun kümeden kaldırıldığını gösterecek şekilde güncelleştirilir.

Sunucuları hizmetten çekme ve sunucuları hizmetten çekerken karşılaşılan sorunlar hakkında daha fazla bilgi için, bu konuda daha önce geçen "[Sunucuları Hizmetten Çekme](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f)" bölümüne bakın.
