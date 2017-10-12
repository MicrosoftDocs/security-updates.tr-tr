---
TOCTitle: RMS Dizin Hizmetleri Veritabanı
Title: RMS Dizin Hizmetleri Veritabanı
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18125143
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747617(v=WS.10)'
---

RMS Dizin Hizmetleri Veritabanı
===============================

Veritabanı sunucusu kullanıcılar, tanıtıcılar (e-posta adresleri gibi), güvenlik kimliği (SID), grup üyeliği ve diğer tanıtıcılar hakkındaki bilgileri içeren dizin hizmeti veritabanını barındırır. Bu bilgiler RMS Lisans hizmeti tarafından Active Directory genel kataloğuna yöneltilen LDAP sorgularından alınır. Bu işlem ve amacı hakkında daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS Active Directory Önbelleği](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)" bölümüne bakın.

RMS hizmet grubu, dizin hizmetleri veritabanında bulunan saklı yordamlar üzerinde Yürütme izinlerine sahiptir.

Aşağıdaki tabloda dizin hizmetleri veritabanı tablolarında depolanan Active Directory öznitelikleri listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Tablo</th>
<th style="border:1px solid black;" >Öznitelik</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: grubun diğer adı<br />
<br />
</li>
<li>GroupID: bu grubun benzersiz kimliği<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: bu grubun Active Directory ayırt edici adı<br />
<br />
</li>
<li>GroupID: bu grubun benzersiz kimliği<br />
<br />
</li>
<li>Expiration: bu grup için, depolanan bilgilerin süresinin dolacağı tarih ve saat<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: bu grubun benzersiz kimliği<br />
<br />
</li>
<li>ParentID: bu grubun üyesi olduğu grubun benzersiz kimliği<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: sorumlunun diğer adı<br />
<br />
</li>
<li>PrincipalID: bu sorumlunun benzersiz kimliği<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: bu sorumlunun benzersiz kimliği<br />
<br />
</li>
<li>Expiration: bu sorumlu için depolanan bilgilerin süresinin dolacağı tarih ve saat<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Bu tablonun her satırı, sorumlunun benzersiz kimliği ile üyesi olduğu grubun benzersiz kimliğini içerir.
<ul>
<li>PrincipalID: bu sorumlunun benzersiz kimliği<br />
<br />
</li>
<li>ParentID: bu sorumlunun üyesi olduğu grubun benzersiz kimliği<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
