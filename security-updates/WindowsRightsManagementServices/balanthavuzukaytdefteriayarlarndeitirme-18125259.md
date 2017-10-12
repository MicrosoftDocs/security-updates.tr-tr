---
TOCTitle: Bağlantı Havuzu Kayıt Defteri Ayarlarını Değiştirme
Title: Bağlantı Havuzu Kayıt Defteri Ayarlarını Değiştirme
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18125259
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747660(v=WS.10)'
---

Bağlantı Havuzu Kayıt Defteri Ayarlarını Değiştirme
===================================================

Sistem performansını artırmak için, RMS'nin kullandığı Basit Dizin Erişimi Protokolü (LDAP) bağlantı havuzunun özelliklerini ayarlamak üzere kayıt defteri anahtarı girdilerini kullanabilirsiniz.

Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda, aşağıdaki kayıt defteri anahtarı, bağlantı havuzu kayıt defteri girdilerine yönelik tam alt anahtar yoludur:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda, aşağıdaki kayıt defteri anahtarı, bağlantı havuzu kayıt defteri girdilerine yönelik tam alt anahtar yoludur:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

Aşağıdaki tabloda Active Directory varsayılan bağlantı havuzu ayarlarını geçersiz kılmak üzere ekleyebileceğiniz girdilerin listesi bulunmaktadır. Görüntülenen değerler varsayılan değerlerdir. RMS'nin sorgu listesini nasıl oluşturduğu ve bu ayarları nasıl kullandığı hakkında daha fazla bilgi için bu konuda daha önce geçen "Active Directory Bağlantı Havuzu Ayarlarını En İyi Duruma Getirme" bölümüne bakın.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ad</th>
<th style="border:1px solid black;" >Tür</th>
<th style="border:1px solid black;" >Varsayılan Değer</th>
<th style="border:1px solid black;" >Açıklama</th>
<th style="border:1px solid black;" >Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">Dize</td>
<td style="border:1px solid black;">name-1, ..., name-n</td>
<td style="border:1px solid black;">Genel katalogların virgülle ayrılan listesi (DNS adları kullanılır). Bu anahtar RMS'yi yalnızca belirtilen genel katalogları kullanacak şekilde kısıtlar.</td>
<td style="border:1px solid black;">RMS'nin sorgu listesi oluşturmasını istemiyorsanız, kullanılacak genel katalogları belirtmek için bu ayarı kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">RMS başlatılmadan önce kullanılabilir olması gereken en az genel katalog sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Topoloji Bulma algoritmasının sorgu listesine ekleyeceği en fazla genel katalog sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">RMS'nin istekleri kabul edebilmesi için DiscoveryServices'in sorgu listesine ekleyeceği genel katalogları aramaya başlamasından önce yanıt verir durumda olması gereken en az bağlantı sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Kesik bir bağlantıyı yanıt vermiyor olarak bildirmeden önce yeniden bağlantı kurma denemesi sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Kesik bir bağlantı için yeniden bağlantı kurmayı denemeden önce beklenecek saniye sayısı.</td>
<td style="border:1px solid black;">Beklenmedik durumlar dışında bu varsayılan ayarı değiştirmeniz gerekmez.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Yavaş bir bağlantıyı yeniden denemeden önce beklenecek saniye sayısı.</td>
<td style="border:1px solid black;">Beklenmedik durumlar dışında bu varsayılan ayarı değiştirmeniz gerekmez.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Yük dengeleme sırasında sürekli çalışmanın ağırlığı.</td>
<td style="border:1px solid black;">Yük dengelemede sürekli çalışmanın göreli önemi. En düşük değer 1'dir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Yük dengeleme sırasında bağlantı başına iş parçacığı sayısının ağırlığı.</td>
<td style="border:1px solid black;">Düşük iş parçacığı sayısının göreli önemi.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Yük dengeleme sırasında yavaş bağlantının ağırlığı.</td>
<td style="border:1px solid black;">Yavaş olmayan bağlantının göreli önemi.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Sorgu listesine bir genel katalog ekleme isteğini zaman aşımına uğratmadan önce beklenecek saniye sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">LDAP API'lerinde zaman aşımından önce beklenecek saniye sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Yukarıdan aşağıya yapılan LDAP genişletme sorgularında zaman aşımından önce beklenecek saniye sayısı.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Dikkat                                                                                                             |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Kayıt defterinde yanlış düzenlemeler yapmak sisteminize ciddi zararlar verebilir. Kayıt defterinde değişiklik yapmadan önce, bilgisayarınızdaki değerli verileri yedeklemeniz gerekir. |
