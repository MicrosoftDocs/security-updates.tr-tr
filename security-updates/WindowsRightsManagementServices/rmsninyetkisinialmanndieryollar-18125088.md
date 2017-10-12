---
TOCTitle: 'RMS''nin Yetkisini Almanın Diğer Yolları'
Title: 'RMS''nin Yetkisini Almanın Diğer Yolları'
ms:assetid: '4d32f35e-997d-4d10-ab66-efe217e853f7'
ms:contentKeyID: 18125088
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720268(v=WS.10)'
---

RMS'nin Yetkisini Almanın Diğer Yolları
=======================================

Kuruluşunuzda RMS kullanmayı planlama aşamasındayken herhangi bir nedenle bazı RMS sunucularını kullanmayı durdurmanız gerekirse, yetki alma için aşağıdaki diğer yollardan birini kullanmayı göz önünde bulundurun.

**Güvenilen yayımlama etki alanı kurun**

Tüm RMS korumalı bilgiler RMS sunucusunun özel anahtarıyla şifrelenir. Güvenilen yayımlama etki alanı bir RMS sunucusunun özel anahtarını başka bir RMS sunucusuna almanıza olanak tanır. Böylece bir RMS sunucusu, farklı bir RMS sunucusu tarafından oluşturulan yayımlama lisanslarına yönelik kullanım lisansları verebilir. Anahtar verildikten sonra, sunucunun yapılandırma ve yüklemesi kaldırılabilir.

**Super Users grubu ayarlama**

Hiçbir kullanıcının içeriğe erişim hakkı olmadığı için RMS korumalı içerik açılamıyorsa, Super Users grubuna, ilgili sunucu tarafından yayımlanan tüm RMS korumalı içerik üzerinde tam denetim izni verebilirsiniz. Super Users grubu üyelerine, grubun yapılandırıldığı RMS sunucusu veya kümesi tarafından verilen tüm kullanım lisansları için tam sahip hakları verilir. Bu, bu grup üyelerinin korumalı içeriğe sahip her türlü dosyanın şifresini çözebileceği ve bunların üzerindeki korumayı kaldırabileceği anlamına gelir. Bu grubun bir üyesi, örneğin yeni sahibin dosyaları yayımlayabilmesi ve yönetebilmesi için, işten çıkarılan bir çalışan tarafından yayımlanmış dosyalar üzerindeki korumayı kaldırabilir.

Super Users grubunda otomatik olarak eklenmiş hiçbir üye yoktur, hatta yöneticiler bile bulunmaz. Bu grubun Active Directory'de, e-posta adresi özniteliği grup adıyla aynı olan ve "*grup\_adı*@*etki\_alanı\_adı*.com" biçimine sahip bir dağıtım grubu olarak bulunması gerekir. Grup adının e-posta adresi özniteliğiyle aynı olması gerekir ve grup adı büyük/küçük harf duyarlıdır.
