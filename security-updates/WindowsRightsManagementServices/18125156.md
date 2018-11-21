---
TOCTitle: RMS Günlük Veritabanı Tabloları
Title: RMS Günlük Veritabanı Tabloları
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18125156
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747569(v=WS.10)'
---

RMS Günlük Veritabanı Tabloları
===============================

Bu bölümde RMS günlük veritabanı tabloları açıklanmaktadır.

DRMS\_Log\_Master
-----------------

Aşağıdaki tabloda her günlük kaydı için bir girdi bulunmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Veri Türü</th>
<th style="border:1px solid black;" >NULL değeri</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">Bu günlük kaydının benzersiz kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_HostMachineName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Bu kaydı üreten sunucu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_HostMachineRequestId</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstek kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_RequestTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstek tarihi ve saati</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestPath</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İsteğin URL yolu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstek türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_RequestUserAddress</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstemcinin IP adresi</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_RequestUserAgent</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstemcinin kullanıcı aracı üstbilgisi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İsteğin kimlik doğrulama durumu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_SecureConnectionState</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İsteğin SSL koruması</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_AuthenticatedId</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Kimliği doğrulanmış kullanıcının kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ReceivedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstekte istemciden alınan XrML</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_IssuedXrML</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İstekte verilen XrML lisansı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Metadata</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Metadata</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_SuccessOrFailure</td>
<td style="border:1px solid black;">nvarchar(32)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İsteğin başarısı veya başarısızlığı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_ErrorInformation</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Hata verileri</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_LogCreateTime</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Günlük oluşturma saati</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
Aşağıdaki tabloda günlük kaydı ek verilerinin listesi bulunmaktadır. Genel olarak XrML verileri günlüğü bu tabloya kaydedilir.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Veri Türü</th>
<th style="border:1px solid black;" >NULL değeri</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_LogDetailID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1)</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_LogID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL değil (FK)</td>
<td style="border:1px solid black;">Üst günlük kaydının kimliği</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_Name</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Özelliğin adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Value</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Özelliğin değeri</td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
Aşağıdaki tabloda günlük dinleyici hizmetinin günlüğe kaydettiği alanların listesi bulunmaktadır.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Veri Türü</th>
<th style="border:1px solid black;" >NULL değeri</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_FieldName</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Alanın adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_FieldDescription</td>
<td style="border:1px solid black;">nvarchar(1024)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Alanın açıklaması</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_IsIncluded</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Alanın günlüğe alınıp alınmadığını gösterir.</td>
</tr>
</tbody>
</table>
