---
TOCTitle: RMS Web Hizmetleri
Title: RMS Web Hizmetleri
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18125328
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747728(v=WS.10)'
---

RMS Web Hizmetleri
==================

RMS, RMS sisteminin sunucu bileşenini sağlar. Ana işlevleri Microsoft® Internet Information Services (IIS) üzerinde çalışan bir grup Microsoft® ASP.NET Web hizmeti olarak uygulanır. RMS Web hizmetleri SOAP arabirimi veya .NET Remoting üzerinden yapılır.

Web hizmetleri şunları sağlar:

-   Sunucuların alt kayıt işlemi
-   Güvenilen varlıkların hesap sertifikası
-   Telif haklı bilgilerin lisanslaması
-   RMS'nin yönetim işlevleri

Aşağıdaki tablo RMS Web hizmetlerini açıklamaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Hizmet</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alt Kayıt</td>
<td style="border:1px solid black;">Yalnızca lisans sağlayıcı kümelerdeki sunuculara alt kayıt sunucu lisans sağlayıcı sertifikalar sağlar. Bu sertifikalar yalnızca lisans sağlayıcı kümenin yayın veya kullanım lisansı vermesini sağlar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hesap sertifikası</td>
<td style="border:1px solid black;">Kullanıcılara haklar hesabı sertifikası sağlar. Bu sertifikalar kullanıcıların telif haklı içeriği yazmak veya kullanmak için yayın ve kullanım lisanslarını alabilmeleri için gereklidir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Etkinleştirme proxy'si</td>
<td style="border:1px solid black;">Bu hizmet RMS sürüm 1 istemcisiyle uyumluluk için bırakılır. Makine etkinleştirme isteklerini Microsoft Etkinleştirme Hizmeti'ne iletir ve RMS sürüm 1 istemcilerine kasa ve RMS makine sertifikalarını döndürür. Bu hizmet RMS Service Pack 1 (SP1) veya daha yeni istemcileri tarafından kullanılmaz.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Yayımlama</td>
<td style="border:1px solid black;">Yazarların telif haklı içerik oluşturmalarını ve dağıtmalarını sağlayan yayımlama lisanslarını verir. Ayrıca kullanıcıların iç ağ ana bilgisayar RMS'sine bağlanmadan telif haklı içeriği yayımlamalarına izin veren istemci lisans sağlayıcı sertifikalarını da verir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lisans</td>
<td style="border:1px solid black;">Kullanıcıların telif haklı içeriği kullanmasına izin veren kullanım lisanslarını verir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Yönetim</td>
<td style="border:1px solid black;">Yöneticinin RMS'yi yönetmesini sağlar.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DrmRemote</td>
<td style="border:1px solid black;">.NET Remoting üzerinden Web hizmetlerinin birbiriyle ve RMS sisteminin diğer bileşenleriyle iletişim kurmasına sağlar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Yetki Alma</td>
<td style="border:1px solid black;">Daha önceki telif haklı içeriğin korumasını kaldırır ve istemciye döndürür. Bu hizmet RMS Kur tarafından yüklenir, ancak yönetici tarafından etkinleştirilene kadar IIS'te karşılık gelen bir sanal kökü olmaz. Bu hizmeti etkinleştirme diğer tüm hizmetleri devre dışı bırakır.</td>
</tr>
</tbody>
</table>
  
Web hizmetlerinin yanında, RMS bir günlük dinleyici hizmeti yükler. Her Web hizmeti günlüğe kaydedilen verileri günlük ileti kuyruğuna gönderir. Günlük dinleme hizmeti daha sonra ileti kuyruğundan günlüğe alınan verileri günlük veritabanına aktarır.
  
Web hizmeti uygulamaları IIS sanal dizinlerinde bulunur. Bu sanal dizinler her RMS sunucusunda sağlama sırasında seçmiş olduğunuz Web sitesinin altına yüklenir.
  
Her sana dizin için kimlik doğrulama ve erişim ayrı olarak yapılandırılır. Bunun yanında her Web hizmeti için ayrı ayrı erişim yapılandırılır. Sana dizinler ve Web hizmetleri dosyalarının güvenlik ayarları hakkında bilgi için, daha sonra bu bölümde bulunan [RMS için Internet Information Services Desteği](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c) konusuna bakın.
  
Her Web hizmeti hakkında daha fazla bilgi için, daha sonra bu bölümde bulunan [RMS Yazılım Bileşenleri](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca) konusuna bakın.
