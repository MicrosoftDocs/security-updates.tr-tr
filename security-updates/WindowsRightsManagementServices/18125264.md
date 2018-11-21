---
TOCTitle: 'RMS''ye Veritabanı Desteği Sağlamak Üzere Microsoft SQL Server 2000 Desktop Engine''i (MSDE 2000) Yüklemek için'
Title: 'RMS''ye Veritabanı Desteği Sağlamak Üzere Microsoft SQL Server 2000 Desktop Engine''i (MSDE 2000) Yüklemek için'
ms:assetid: 'c9b9cd08-98c4-424f-b3fc-d685f57c002e'
ms:contentKeyID: 18125264
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747667(v=WS.10)'
---

RMS'ye Veritabanı Desteği Sağlamak Üzere Microsoft SQL Server 2000 Desktop Engine'i (MSDE 2000) Yüklemek için
=============================================================================================================

RMS'ye Veritabanı Desteği Sağlamak Üzere Microsoft SQL Server 2000 Desktop Engine'i (MSDE 2000) Yükleme
-------------------------------------------------------------------------------------------------------

#### RMS'ye Veritabanı Desteği Sağlamak Üzere Microsoft SQL Server 2000 Desktop Engine'i (MSDE 2000) Yüklemek için

1.  Microsoft SQL Server 2000 Desktop Engine'i (MSDE 2000) yüklemek istediğiniz sunucudaki yerel Administrators grubunun bir üyesi olan etki alanı hesabını kullanarak oturum açın.

2.  MSDE 2000'i [Microsoft Web sitesinden](http://www.microsoft.com/) (http://www.microsoft.com/) yükleyin ve bilgisayarınızda bir konuma kaydedin.

3.  MSDE 2000 kurulum paketini bir klasöre ayıklamak için MSDE2000A.exe dosyasını çalıştırın. Bu klasör varsayılan olarak MSDERelA olarak adlandırılacaktır, ancak başka bir ad belirtebilirsiniz.

4.  Bir komut istemi açın ve MSDE 2000 yüklemesini kaydettiğiniz konuma gidin.

5.  Microsoft SQL Server 2000 Desktop Engine uygulamasını RMS ile çalışacak şekilde doğru yapılandırmayla yüklemek için aşağıdaki komutu yazın ve *parola* değerini istediğiniz sağlam parolayla değiştirin:

    **Setup.exe /i setup\\sqlrun10.msi INSTANCENAME=RMS DISABLEAGENTSTARTUP=1 SAPWD=***parola*

    | ![](/security-updates/images/Cc747667.Important(WS.10).gif)Önemli                                                                                                                                                                                                             |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | MSDE hizmetinin yüklendikten sonra çalıştırılması gerekir. Hizmeti **Denetim Masası**'ndaki **Hizmetler**'den çalıştırabilirsiniz. RMS çalışırken MSDE veritabanının her zaman kullanılabilir olduğundan emin olmak için hizmeti otomatik olarak başlamak için yapılandırmanız önerilir. |

RMS yapılandırma veritabanını destekleyecek veritabanını yükleyinceye kadar bir sunucuda RMS'yi hazırlamayın.

Microsoft SQL Server Desktop Engine, kuruluş çapındaki veritabanını tam olarak çalıştırmak ve desteklemek için gereken araçları içermediğinden, RMS veritabanlarını desteklemek amacıyla yalnızca sınama ortamlarında kullanılması önerilir. Buna ek olarak, MSDE uzak ağları desteklemediğinden, bunu RMS ile aynı sunucuya yüklemeniz gerekir ve RMS kümesine başka RMS sunucuları yükleyemezsiniz. Microsoft SQL Server Desktop Engine kullanım koşullarında, Microsoft SQL Server Desktop Engine veritabanını denetlemek için SQL Server istemci araçlarını kullanamayacağınız belirtilir. Bu kısıtlama nedeniyle, RMS yapılandırma veritabanını yedekleyemez ve geri yükleyemez, günlük bilgilerini görüntüleyemez veya yapılandırma veritabanında depolanan verileri doğrudan değiştiremezsiniz.
