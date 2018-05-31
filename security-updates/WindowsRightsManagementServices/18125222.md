---
TOCTitle: Sağlama Sırasında Güvenlik
Title: Sağlama Sırasında Güvenlik
ms:assetid: '9f1282c5-5642-4870-a9a4-c3a485f8ff76'
ms:contentKeyID: 18125222
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747616(v=WS.10)'
---

Sağlama Sırasında Güvenlik
==========================

Varolan bir Web sitesinde RMS kaynaklarını sağlamak için RMS Yönetimi Web sitesini kullanabilirsiniz. Sağlama sırasında, bu Web sitesinin altında sanal dizinler ve uygulama havuzları oluşturulur; veritabanı sunucusunda RMS veritabanları oluşturulur ve yapılandırılır. İsteğe bağlı olarak, sunucunuz Internet'e bağlıysa, sağlama işlemi sırasında sunucu Microsoft Kayıt Hizmeti'ne kaydettirilebilir.

RMS sağlama sırasında aşağıdaki tabloda açıklanan hesapları kullanır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Hesap</th>
<th style="border:1px solid black;" >Amaç</th>
<th style="border:1px solid black;" >İzinler</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Oturum açan kullanıcının hesabı</td>
<td style="border:1px solid black;">Sanal dizinler ve uygulama havuzları oluşturur. IIS Windows kimlik doğrulaması gerektirir ve RMS yerel olarak oturum açmış olması gereken oturum açan kullanıcının kimliğini kullanır.</td>
<td style="border:1px solid black;">Tam denetim (oturum açan kullanıcının yerel bir yönetici olması gerekir).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sistem hesabı</td>
<td style="border:1px solid black;">Seri durumuna getirme için geçici derleme oluşturur.</td>
<td style="border:1px solid black;">Windows geçici klasörüne (C:\Windows\Temp) yönelik Okuma ve Yazma izinleri.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ASPNET hesabı</td>
<td style="border:1px solid black;">*.aspx dosyalarının geçici derlemesini oluşturur.</td>
<td style="border:1px solid black;">Varsayılan olarak geçici derleme önbelleği dizinine (C:\Windows\Microsoft.NET\Framework\v1.1.4322\Temporary ASP.NET Files) erişim.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ağ Hizmetleri hesabı</td>
<td style="border:1px solid black;">Hizmet bağlantı noktasını Active Directory'ye kaydettirir.</td>
<td style="border:1px solid black;"><ul>
<li>Sağlama sitesine yönelik salt okuma izinleri (genellikle C:\Inetpub\Wwwroot\Provisioning).<br />
<br />
</li>
<li><strong>DRMS</strong> kayıt defteri anahtarına yönelik Okuma ve Yazma izinleri. İzinler aşağıdaki kayıt defteri anahtarını da oluşturan RMS Kurulumu tarafından verilir.<br />
<br />
Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\Microsoft\DRMS\1.0</code><br />
<br />
Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda<br />
<br />
<code>HKEY_LOCAL_MACHINE\Software\WOW6432Node\Microsoft\DRMS\1.0</code><br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

RMS Kurulumu, sağlama sırasında aşağıdaki görevleri gerçekleştirir:

-   Veritabanı sunucusunda:
    -   Yapılandırma, dizin hizmetleri ve günlük veritabanlarını oluşturur.
    -   RMS Service Group'a Oturum Açma izinleri verir.
    -   Saklı yordamları veritabanlarına yükler ve RMS Service Group'a Yürütme izinleri verir.
    -   Ana veritabanında sorguları yürütür.
-   RMS Service Group'u IIS\_WPG grubuna ekler.
-   C:\\Inetpub\\Wwwroot\\\_wmcs yolunda Web hizmetleri ve RMS Yönetimi Web sitesi için sanal dizinler, dosyalar ve uygulama havuzları hiyerarşisi oluşturur.
-   Sanal dizinler, dosyalar ve uygulama havuzları üzerinde DACL'leri ayarlar.
-   RMS Service Group'a geçici klasöre erişim izni verir.
-   Yazılım anahtar korumasını belirttiğinizde, sunucu lisans özel anahtarını, veritabanına depolamadan önce şifreler. RMS sağlama sırasında bir parola isteğinde bulunur ve makine düzeyi DPAPI'ya erişim kazanır.
-   Günlük dinleyici hizmetini yükler.
-   Günlük ileti sırası oluşturur.
-   Kök sertifika sunucusunu sağlıyorsa, Active Directory'de hizmet bağlantı noktası belirler.
