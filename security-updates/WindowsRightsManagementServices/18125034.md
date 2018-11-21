---
TOCTitle: Günlük Dosyalarını Görüntüleme
Title: Günlük Dosyalarını Görüntüleme
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18125034
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720228(v=WS.10)'
---

Günlük Dosyalarını Görüntüleme
==============================

Günlük dosyaları, RMS'yi dağıtma şeklinize bağlı olarak, SQL Server veya Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Sürüm A gibi bir veritabanında depolanır. Günlük dosyalarında depolanan bilgileri azaltmak için filtre yazabilirsiniz. Yönergeler için SQL Server Enterprise Manager Yardımı'na bakın.

Tipik bir günlük girdisinin boyutu yaklaşık 300 bayttır. Aşağıdaki tabloda günlüğe kaydedilen alanlar açıklanmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Alan</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">HostMachineName</td>
<td style="border:1px solid black;">İsteği işlemiş olan bilgisayar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">HostMachineRequestId</td>
<td style="border:1px solid black;">Bu isteği bu bilgisayarda benzersiz bir şekilde tanımlar. HostMachineName ve HostMachineRequestId birleşimi, isteği benzersiz bir şekilde küme içinde tanımlar.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestTime</td>
<td style="border:1px solid black;">İsteğin alındığı zaman (Eşgüdümlü Evrensel Saat, Greenwich Saati).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestPath</td>
<td style="border:1px solid black;">.asmx dosyasının göreli URL'si, örneğin: /_wmcs/Lisans/License.asmx.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestType</td>
<td style="border:1px solid black;">Çağırılan Web yönteminin adı, örneğin: AcquireLicense.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestUserAddress</td>
<td style="border:1px solid black;">İstek sahibinin kaynak IP adresi.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestUserAgent</td>
<td style="border:1px solid black;">HTTP üstbilgisindeki User Agent (Kullanıcı Aracısı) değeri.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedState</td>
<td style="border:1px solid black;">HTTP bağlantısı kimliğinin doğrulanıp doğrulanmadığı (Doğru/Yanlış).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SecureConnectionState</td>
<td style="border:1px solid black;">Bir SSL bağlantısı olup olmadığı (Doğru/Yanlış).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedId</td>
<td style="border:1px solid black;">Kimliği doğrulanmış isteklerin oturum açma adı. AuthenticatedState=Yanlış ise boştur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ReceivedXrMLDocument</td>
<td style="border:1px solid black;">İstek sahibinden alınan XrML belgesi.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ReceivedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Alınan XrML belgesine ait veren zinciri.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IssuedXrMLDocument</td>
<td style="border:1px solid black;">İstek sahibine döndürülen XrML belgesi.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">IssuedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Alınan XrML belgesine ait veren zinciri.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SuccessOrFailure</td>
<td style="border:1px solid black;">İsteğin başarılı mı yoksa başarısız mı olduğu (Başarılı/Başarısız).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Metadata</td>
<td style="border:1px solid black;">Meta veriler alanı.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ErrorInformation</td>
<td style="border:1px solid black;">Hata oluşmuşsa açıklayıcı hata iletisi.</td>
</tr>
</tbody>
</table>
