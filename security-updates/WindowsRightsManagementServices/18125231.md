---
TOCTitle: RMS Sunucusunu Komut İsteminden Yükleme
Title: RMS Sunucusunu Komut İsteminden Yükleme
ms:assetid: 'b55b1e2a-dd14-4168-a37f-9cdedbec660b'
ms:contentKeyID: 18125231
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747733(v=WS.10)'
---

RMS Sunucusunu Komut İsteminden Yükleme
=======================================

RMS Service Pack 2'yi (SP2), yüklemeyi otomatikleştirmenize olanak sağlayan bir komut isteminden yükleyebilirsiniz. Yükleme, şu iki yoldan biriyle otomatikleştirilebilir: karşıdan yüklediğiniz EXE istemcisini kullanarak bir katılımsız yükleme gerçekleştirmek veya karşıdan yüklediğiniz EXE dosyasından ayıklanan MSI dosyalarını kullanarak RMS istemcisini yüklemek. Karşıdan yüklediğiniz EXE dosyasını kullanarak yüklemek için, aşağıdaki sözdizimini kullanın:

**WindowsRightsManagementServicesSP2-KB917275-Client-TRK.exe -override 1 /I MsDrmClient.msi REBOOT=ReallySuppress /q -override 2 /I RmClientBackCompat.msi REBOOT=ReallySuppress /q**

Windows® Installer (.msi) dosyalarını kullanarak yüklemek için, ilk olarak msi dosyalarını RMS SP2 yürütülebilir dosyasından ayıklamalısınız. msdrmclient.msi ve RmClientBackCompat.msi dosyalarını ayıklamak için komut isteminde aşağıdaki komut çalıştırılabilir:

**WindowsRightsManagementServiceSP2-KB917275-Server-TRK.exe /X:C:\\***Yükleme\_Konumu*

.msi dosyaları ayıklandıktan sonra, aşağıdaki komutları kullanarak RMS'yi yükleyebilirsiniz:

**msiexec.exe /I MSDrmClient.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Yükleme\_Konumu*

**msiexec.exe /I RMClientBackCompat.msi /qn ALLUSERS=2 /m MSIDHOG /lei logfile.log DISPLYPAGE="NO" TARGETDIR=c:\\***Yükleme\_Konumu*

Aşağıdaki tabloda, her bir komuttaki sözdizimi açıklanmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametre</th>
<th style="border:1px solid black;" >Tanım</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/I MSDrmClient.msi</strong> veya <strong>/I RMClientBackCompat.msi</strong></td>
<td style="border:1px solid black;">Gerekli. Yüklenecek ürünü belirtir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/qn</strong></td>
<td style="border:1px solid black;">İsteğe bağlı. Kullanıcı etkileşimi olmadan sessiz yüklemeyi belirtir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/lei</strong> <em>günlükdosyası.log</em></td>
<td style="border:1px solid black;">İsteğe bağlı. Hata ve durum iletilerinin günlüğe kaydedileceği dosyayı belirtir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>DISPLAYPAGE=”NO”</strong></td>
<td style="border:1px solid black;">İsteğe bağlı. <strong>Genel Yönetim</strong> sayfasının yüklemeden sonra görüntülenmeyeceğini belirtir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>TARGETDIR=c:\</strong><em>Yükleme_Konumu</em></td>
<td style="border:1px solid black;">İsteğe bağlı. RMS Service Pack 2 yüklenecek dizini belirtir. Konum belirtmezseniz, varsayılan yükleme konumu kullanılır.</td>
</tr>
</tbody>
</table>
  
| ![](/security-updates/images/Cc747733.note(WS.10).gif)Not                                                                                                                                                                                             |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Uygulamayı seçtiğiniz yükleme yöntemine bağlı olmaksızın, her iki .msi dosyasının da başarılı bir şekilde yüklendiğinden emin olmalısınız. MSDrmClient.msi dosyasının yüklenmesini engelleyen bir hata oluşursa, RMClientBackCompat.msi dosyası yüklenmemelidir. |
