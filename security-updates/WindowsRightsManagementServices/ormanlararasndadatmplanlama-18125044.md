---
TOCTitle: Ormanlar Arasında Dağıtım Planlama
Title: Ormanlar Arasında Dağıtım Planlama
ms:assetid: '2dfb40b7-95b1-4362-b32e-72867544b705'
ms:contentKeyID: 18125044
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720233(v=WS.10)'
---

Ormanlar Arasında Dağıtım Planlama
==================================

RMS'yi birden çok ormanı olan bir ortamda dağıtıyorsanız, RMS'nin dağıtıldığı ormanın dışındaki kullanıcı ve gruplar için gerekebilecek desteği belirlemelisiniz. Sorun, diğer ormanlardaki kullanıcı veya grup nesnelerinin genelde RMS'nin bulunduğu ormanda temsilci nesneleri olmamasıdır. RMS'yi diğer ormanlardaki kullanıcı veya grupların izinlerini kısıtlamak için kullanmayı hedefliyorsanız, ormanınızı, ormanlar arasında grup genişletmeye izin verecek şekilde yapılandırmanız gerekir.

RMS için ormanlar arasında grup genişletme desteğini iki yöntemle uygulayabilirsiniz:

-   RMS'yi, grupların tanımlandığı ve bu grupların üyeliğini genişletmek için kullanılacağı ormanda dağıtın.
-   Yerel RMS yüklemesinin herhangi bir kullanıcıya yönelik tam grup üyeliğini belirlemesine olanak vermek için grup tanımlarını ormanlar arasında eşitleyin. Kullanım lisansı isteyen kullanıcının ayrı bir ormanda Windows hesabı varsa, bu kullanıcının grup üyeliğini temsil etmek için yerel ormanda da bir kişi nesnesi olması gerekir. Ormanlar arasında grup nesnelerine tam bağımlı eşitleme uygulamak için Microsoft® Identity Integration Server (MIIS) 2003 veya Identity Integration Feature Pack (IIFP) gibi meta dizinler kullanabilirsiniz.

RMS'yi yalnızca bir orman için kullanmayı planlıyorsanız, RMS yapılandırma veritabanındaki **MaxCrossForestCalls** küme ilkesini değiştirerek, işlemi kullanım lisansları vermek için en iyi hale getirebilirsiniz. Bu ilke, bir grubun üyeliğinin aşabileceği orman sınırı sayısının en üst değerini belirtir. Varsayılan değer 10'dur. Değeri 0 olarak değiştirmek için aşağıdaki SQL komutunu kullanın:

`update DRMS_ClusterPolicies set PolicyData=0 where PolicyName='MaxCrossForestCalls'`
