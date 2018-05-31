---
TOCTitle: RMS Çekirdek Yapılandırma Veritabanı Tabloları
Title: RMS Çekirdek Yapılandırma Veritabanı Tabloları
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18125180
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747676(v=WS.10)'
---

RMS Çekirdek Yapılandırma Veritabanı Tabloları
==============================================

Bu başlıkta RMS çekirdek yapılandırma veritabanı tabloları açıklanmaktadır.

DRMS\_ApplicationExclusionList
------------------------------

Aşağıdaki tabloda, dışlanmış uygulamalarla ilgili bilgiler listelenmektedir.

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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ad</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Uygulama adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en küçük ana sürüm numarası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en küçük alt sürüm numarası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en küçük oluşturma sürüm numarası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en küçük gözden geçirme sürüm numarası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en büyük ana sürüm numarası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en büyük alt sürüm numarası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en büyük oluşturma sürüm numarası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulamanın en büyük gözden geçirme sürüm numarası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Açıklama</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Uygulama açıklaması</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
Aşağıdaki tabloda ileti sırasıyla ilgili bilgilerin listesi bulunmaktadır.
  
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
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İleti sırası yolu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
Aşağıdaki tabloda, istemciye verilen sertifika türüyle ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Masaüstü, Mobil Aygıt veya Sunucu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
Aşağıdaki tabloda, DRMS\_LicensorCertificate tablosundaki geçerli sunucu lisans sertifikasıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Etkin lisans sahibi sertifikası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
Aşağıdaki tabloda, küme ilkelerinin depolandığı konumlarla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İlke Kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İlke adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İlke verileri</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
Aşağıdaki tabloda kümedeki sunucularla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">Sunucu kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Belirtilmiyor</td>
<td style="border:1px solid black;">Sunucunun bilgisayar adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
Aşağıdaki tabloda, dışlanmış hak hesabı sertifikalarıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Ortak Anahtar baytları</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Kullanıcı kimliği dizini</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Hak hesabı sertifikasının geçerlilik tarihi sonu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Açıklama</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Dışlanmış bu hak hesabı sertifikası anahtarıyla ilişkili NAME</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
Aşağıdaki tabloda etkin sunucu lisans sertifikasıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İlke Kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Anahtar çifti Kimlik Türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Anahtar çifti Kimlik GUID'si</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Gerçek sertifikayı gösteren işaretçi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Aşağıdaki tabloda etkin sunucu lisans sertifikasının özel anahtarıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Anahtar çifti Kimlik Türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Anahtar çifti Kimlik GUID'si</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Anahtarın ikili gösterimi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Şifreleme Hizmeti Sağlayıcısı'nın (CSP) adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">CSP türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Belirtilmiyor</td>
<td style="border:1px solid black;">Anahtar kapsayıcısının adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Anahtar numarası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
Aşağıdaki tabloda, lisans verilmeyecek Microsoft® .NET Passport hesaplarıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Kullanıcı adı/Etki alanı adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
Aşağıdaki tabloda eklentilerle ilgili bilgilerin listesi bulunmaktadır.
  
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
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Eklentinin türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu eklentinin ad alanı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu eklentinin adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Eklentinin yürütme sıra numarası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">DLL dosyası yolu</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Kullanılmıyor</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Eklentinin hata ayıklama modunda çalıştırılıp çalıştırılmayacağını belirler.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Eklentinin ortak anahtarı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Eklentinin sürümü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
Aşağıdaki tabloda, RMS sistemine katılmasına izin verilen eklenti sürümleriyle ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Belirtilmiyor</td>
<td style="border:1px solid black;">Eklentinin sürümü</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
Aşağıdaki tabloda eklenti özellikleriyle ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Özelliğin dahil olduğu eklenti kimliği</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu yapılandırma verisinin özellik adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu yapılandırma verisinin özellik değeri</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
Aşağıdaki tabloda eklenti türüyle ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu eklentinin adı</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
Aşağıdaki tabloda hak ilkesi şablonlarıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Hak ilkesi şablonunun GUID'si</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Bu alan XrML şablon verilerini içerir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
Aşağıdaki tabloda, güvenilen sertifika yetkilileriyle ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika kimliği</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika GUID'si</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika yetkilisi türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
Aşağıdaki tabloda, RMS ortamında güvenilen e-posta etki alanları ile ilgili bilgiler listelenmektedir
  
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
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (FK)t</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güvenilen kullanıcı etki alanı için geçerli e-posta etki alanı adlarının listesi</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
Aşağıdaki tabloda güvenilen kullanıcı etki alanları ve güvenilen yayımlama etki alanlarıyla ilgili bilgiler listelenmektedir.
  
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
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">İç dizin</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Etki alanı türü</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika GUID'si türü</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Sertifika GUID'si</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sertifika kimliği</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Etki alanının SID'i</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Sertifikanın kolay adı</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Güncelleştirme zaman damgası</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Oluşturma zaman damgası</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
Aşağıdaki tabloda, DRMS\_LicensorCertificate tablosuna başvuruda bulunulan XrML sunucusu lisans sertifikalarıyla ilgili bilgiler listelenmektedir. Liste aynı zamanda sertifika zincirini de göstermektedir.
  
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
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY (100,1) NULL değil</td>
<td style="border:1px solid black;">Gerçek sertifikayı gösteren işaretçi</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">NULL değil</td>
<td style="border:1px solid black;">Gerçek sertifikayı gösteren işaretçi</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Gerçek sertifikayı gösteren işaretçi</td>
</tr>
</tbody>
</table>
