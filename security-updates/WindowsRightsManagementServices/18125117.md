---
TOCTitle: Sunucu Hizmetleri için RMS Desteğini Etkinleştirme
Title: Sunucu Hizmetleri için RMS Desteğini Etkinleştirme
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18125117
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747593(v=WS.10)'
---

Sunucu Hizmetleri için RMS Desteğini Etkinleştirme
==================================================

RMS, RMS etkin sunucu uygulamaları için hak hesabı sertifikaları ve kullanım lisansları da sağlar. Sunucu hizmetlerini yapılandırırken bilmeniz gereken birkaç önemli nokta vardır:

-   RMS kanallarındaki İsteğe Bağlı Erişim Denetim Listeleri (DACL), varsayılan olarak en güvenli ayarları kullanır. RMS sunucu hizmetlerini kullanırken DACL'yi değiştirmelisiniz.
-   RMS istemcisi Windows Server 2003 tabanlı bir bilgisayarda yüklüyse ve Internet Explorer Artırılmış Güvenlik Yapılandırması etkinleştirilmişse, RMS kümesinin URL'sini Internet Explorer'ın Güvenilen Siteler Bölgesi'ne eklemelisiniz.
-   Birçok sunucu hizmeti yalnızca tüm Active Directory etki alanı denetleyicilerinde Windows Server 2003 çalışıyorsa gelişmiş Active Directory dizin hizmetleri işlevselliğini kullanır. Sunucu hizmetlerinden birini (örneğin, Microsoft Office SharePoint Server 2007 veya Microsoft Exchange Server 2007 kullanıyorsanız), tüm etki alanı denetleyicilerinde Windows Server 2003 çalışması ve hem etki alanının hem de ormanın Active Directory işlevlerinin Windows Sever 2003 düzeyinde olması önerilir.

Sunucu Sertifika Kanalı'nda Varsayılan İsteğe Bağlı Erişim Denetim Listesi (DACL)
---------------------------------------------------------------------------------

Microsoft Office SharePoint Server 2007 veya Microsoft Exchange Server 2007 gibi uygulamalar, kullanım lisanslarını kullanıcı adına istemek üzere RMS etkindir. Varsayılan bir RMS yüklemesinde, RMS sunucu sertifika kanalının DACL'si sınırlıdır; bir başka deyişle, bir uygulama kullanıcıları için sertifika ve lisans edinemez. Ancak, bu bilgisayarlara yönelik bir RMS etkin uygulamanız varsa, DACL'leri ilgili RMS sunucu sertifika kanalında yapılandırarak, bunların RMS sisteminize katılmasını sağlayabilirsiniz.

RMS etkin sunucu uygulamaları ServerCertification.asmx dosyasını kullanarak RMS sertifika hizmetine bağlanır.

RMS bu dosyaları oluşturduğunda, dosyaların DACL'leri yalnızca sistem işlemlerinin erişimine izin verecek biçimde ayarlanır. Sunucu hizmetleri için bir Active Directory güvenlik grubu oluşturmanız ve daha sonra bu grubu, kullanıcıları adına kullanım lisansları isteyen bilgisayarların Active Directory nesneleriyle doldurmanız önerilir.

Grubu oluşturduktan sonra, DACL'yi ServerCertification.asmx dosyası için değiştirerek, grubun bu hizmet için Okuma & Yürütme izinlerinin olmasını sağlayabilirsiniz. RMS Service Group'u da DACL'ye Okuma & Yürütme izinleriyle eklemelisiniz.

| ![](/security-updates/images/Cc747593.note(WS.10).gif)Not                                                                   |
|----------------------------------------------------------------------------------------------------------------------------------------|
| Kümede birden çok RMS sunucusu varsa, ServerCertification.asmx dosyasındaki DACL'nin kümedeki her bir sunucuda değiştirilmesi gerekir. |

Microsoft Exchange Server 2007 için, her bir Exchange köprü sunucusunun Active Directory bilgisayar nesnesi, sunucu hizmetleri grubuna eklenmelidir. Bu yapılmazsa, Exchange köprü sunucusu, e-postayı alan kullanıcılar adına lisansları isteyemez.

Office SharePoint Server 2007 için, Office SharePoint Server 2007 çalışan sunucunun Active Directory bilgisayar nesnesini sunucu hizmetleri grubuna eklemeniz gerekir. Office SharePoint Server 2007 sunucunuz Active Directory'deki varsayılan sunucuyu kullanacak biçimde yapılandırılırsa, RMS Service Group'u ve sunucu hizmetleri için oluşturulan grubu ServiceLocater.asmx dosyasına eklemeniz ve Okuma & Yürütme izinleri atamanız gerekir.

| ![](/security-updates/images/Cc747593.Important(WS.10).gif)Önemli                                                                                                                                                            |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| ServerCertification.asmx ve ServiceLocater.asmx dosyalarında DACL değiştirildikten sonra Internet Information Services'ın (IIS) yeniden başlatılması gerekir. IIS'yi sıfırlamak için, komut isteminde **iisreset** komutunu çalıştırın. |
