---
TOCTitle: Active Directory Önbellek Ayarlarını Değiştirme
Title: Active Directory Önbellek Ayarlarını Değiştirme
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18125184
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747586(v=WS.10)'
---

Active Directory Önbellek Ayarlarını Değiştirme
===============================================

Kayıt defterindeki ayarlar Active Directory önbelleğinde saklanacak girdi sayısını belirtir. İstemci isteklerini yanıtlama süresini artırmak için bu ayarları değiştirebilirsiniz. Daha fazla bilgi almak için bu konuda daha önce geçen "Dizin hizmetleri performansını en iyi duruma getirme" bölümüne bakın. Önbellekte saklanan bilgiler için geçerlilik dönemi de belirtebilirsiniz.

Windows Server 2003'ün 32 bit sürümünü çalıştıran bilgisayarlarda, aşağıdaki kayıt defteri anahtarı, önbellek girdilerine yönelik tam alt anahtar yoludur:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Windows Server 2003'ün 64 bit sürümünü çalıştıran bilgisayarlarda, aşağıdaki kayıt defteri anahtarı, önbellek girdilerine yönelik tam alt anahtar yoludur:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Aşağıdaki tabloda bellek içi önbellek davranışını denetleyen girdilerin listesi bulunmaktadır.

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
<th style="border:1px solid black;" >Tür</th>
<th style="border:1px solid black;" >Varsayılan Değer</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Önbellekte saklanabilecek en fazla asıl öğe, asıl öğe e-posta adresi ve SID sayısı.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Asıl öğeler için önbelleğe alınan bilgilerin geçerlilik dönemi.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Önbellekte saklanabilecek en fazla grup, grup e-posta adresi ve SID sayısı.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Grup üyeliği için önbelleğe alınan bilgilerin geçerlilik dönemi.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Önbellekte saklanabilecek, bir grup üyesi olan en fazla ilgili kişi sayısı.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Grup üyesi olan ilgili kişilerin önbelleğe alınan bilgilerinin geçerlilik dönemi.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747586.Caution(WS.10).gif)Dikkat                                                                                                             |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Kayıt defterinde yanlış düzenlemeler yapmak sisteminize ciddi zararlar verebilir. Kayıt defterinde değişiklik yapmadan önce, bilgisayarınızdaki değerli verileri yedeklemeniz gerekir. |
  
| ![](images/Cc747586.note(WS.10).gif)Not                                                                                                                                                                                                                                                           |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** ve **ContactMembersofGroupCacheExpireMinutes** kayıt defteri girdileri, veritabanı sunucunuzdaki dizin hizmetleri veritabanında depolanan yerel Active Directory önbelleği için önbellek sona erme süresini de denetler. |
