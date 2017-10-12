---
TOCTitle: RMS Yapılandırma Veritabanı Sertifikası Tabloları
Title: RMS Yapılandırma Veritabanı Sertifikası Tabloları
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18125279
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747760(v=WS.10)'
---

RMS Yapılandırma Veritabanı Sertifikası Tabloları
=================================================

Bu başlıkta RMS yapılandırma veritabanında yer alan sertifika tabloları açıklanmaktadır. Tablolar bu yüklemenin kullanıcıları için verilen hak hesabı sertifikalarıyla ilgili bilgileri içerir.

UD\_Machines
------------

Aşağıdaki tabloda tüm bilgisayarların donanım kimlikleriyle ilgili bilgiler listelenir.

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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) NULL değil</td>
<td style="border:1px solid black;">Donanım kimliği karması</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Girdinin tabloya eklendiği tarih ve saat</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
Aşağıdaki tabloda kullanıcıların Microsoft® .NET Passport bilgileriyle ilgili ayrıntılar listelenir.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">.NET Passport kullanıcı kimliği</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
Aşağıdaki tabloda sertifikalı kullanıcılar bilgisayar bilgileriyle ilişkilendirilmektedir.
  
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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Girdinin tabloya eklendiği tarih ve saat</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
Aşağıdaki tabloda kullanıcı verileriyle ilgili bilgiler listelenir.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (1,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) NULL değil</td>
<td style="border:1px solid black;">Şifreli kullanıcı ortak/özel anahtarı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Şifresiz ortak/özel anahtarın uzunluğu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanıcı ortak anahtarı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Ortak/özel anahtar çiftini şifrelemede kullanılan lisans sahibi sertifikası dizini</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Belirtilmiyor</td>
<td style="border:1px solid black;">Kullanılmıyor</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanıcı anahtarının geçerlilik tarihi sonu</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Anahtarın geçici kullanımının bitiş tarihi ve saati</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanılmıyor</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanıcının geçerli kota düzeyi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Ek kota isteklerinin yerine getirilmesinden önceki gün sayısı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Son ek kullanıcı sertifikasının tarihi ve saati</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Girdinin tabloya eklendiği tarih ve saat</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
Aşağıdaki tabloda Windows tarafından kimliği doğrulanmış ve sertifika almış tüm kullanıcıların kimlik listesi bulunmaktadır.
  
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
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanıcının güvenlik kimliği (SID)</td>
</tr>
</tbody>
</table>
