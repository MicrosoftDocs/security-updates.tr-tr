---
TOCTitle: Super Users Grubunu Kullanma
Title: Super Users Grubunu Kullanma
ms:assetid: '0febcb3e-7124-4e51-971a-1013b928d33b'
ms:contentKeyID: 18125003
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720198(v=WS.10)'
---

Super Users Grubunu Kullanma
============================

RMS hazırlık sırasında tüm hak korumalı içeriğin üzerinde tam denetime sahip özel bir Super Users grubu oluşturur. Super Users grubu üyelerine, Super Users grubunun yapılandırıldığı RMS sunucusu veya kümesi tarafından verilen bütün kullanım lisanslarında tüm sahip olma hakları verilir. Bu, bu grup üyelerinin korumalı içeriğe sahip her türlü dosyanın şifresini çözebileceği ve bunların üzerindeki korumayı kaldırabileceği anlamına gelir. Bu grubun bir üyesi, örneğin yeni sahibin dosyaları yayımlayabilmesi ve yönetebilmesi için, işten çıkarılan bir çalışan tarafından yayımlanmış dosyalar üzerindeki korumayı kaldırabilir.

Varsayılan olarak, Super Users grubunda üye, hatta yönetici bulunmaz. RMS Yönetim Web sitesini kullandığınızda, RMS için Super Users grubu olarak kullanmak üzere bir Active Directory güvenlik grubu belirtebilirsiniz. Varolan Active Directory grubunu kullanabilir veya bu amaç doğrultusunda yeni bir grup oluşturabilirsiniz. Grubun, RMS yüklemesi ile aynı Active Directory ormanında bulunması gerekir. RMS Super Users grubu olarak belirttiğiniz grubun üyeleri olan tüm kullanıcı hesaplarına otomatik olarak Super Users grubu izinleri verilir.

Super Users grubunun RMS'de nasıl belirtileceği hakkında bilgi için, bu konuda daha sonra yer alan "[Super Users Grubu Ayarlamak için](https://technet.microsoft.com/f2ef847e-2824-471f-9079-5c343094aba8)" bölümüne bakın.

| ![](/security-updates/images/Cc720198.note(WS.10).gif)Not                                                                                                                                                                                                                                                                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bir grubu RMS için Super Users grubu olarak tanımlamadan önce, grubun RMS yüklemesi ile aynı Active Directory ormanında bulunması gerekir. Bu grup özelliklerinin hesap adıyla aynı olan tam etki alanı adı (FQDN) dahil olmak üzere e-posta adresini içermesi gerekir. E-posta adresinin *grup\_adı*@*etki\_alanı\_adı* biçiminde olması gerekir. |
