---
TOCTitle: RMS Sistemine Genel Bakış
Title: RMS Sistemine Genel Bakış
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18125269
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747671(v=WS.10)'
---

RMS Sistemine Genel Bakış
=========================

Bu konuda, RMS Web hizmetleri ve RMS istemcisi teknolojilerinin bir RMS sisteminde nasıl birlikte çalıştığı hakkında bilgiler sağlanmıştır.

Aşağıdaki tabloda RMS dağıtımında yer alan sunucu türleri listelenmiş ve bunları işlevleri açıklanmıştır. Ayrıntılı dağıtım bilgileri için, bu belge grubundaki "RMS Sistemini Dağıtma" konusuna bakın.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Sunucu ve Küme</th>
<th style="border:1px solid black;" >İşlev</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kök sertifikası</td>
<td style="border:1px solid black;">Aşağıdaki RMS hizmetlerini çalıştırır:
<ul>
<li><strong>Alt kayıt</strong>. Lisans sunucularının alt kaydını yapar.<br />
<br />
</li>
<li><strong>Etkinleştirme proxy hizmeti</strong>. Kasalara ve RMS makine sertifikalarına yönelik istemci istekleri için Internet proxy hizmeti olarak çalışır.<br />
<br />
</li>
<li><strong>Sertifika</strong>. Hak hesabı sertifikalarını verir.<br />
<br />
</li>
<li><strong>Yayımlama</strong>. Yayımlama lisansları verir.<br />
<br />
</li>
<li><strong>Lisans</strong>. Kullanım lisansları verir.<br />
<br />
</li>
</ul>
Her dağıtımın en az bir kök sertifika sunucusu veya kümesini içermesi gerekir. Her Active Directory ormanında yalnızca bir kök sertifika kümesi olabilir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lisans (isteğe bağlı)</td>
<td style="border:1px solid black;">Aşağıdaki RMS hizmetlerini çalıştırır:
<ul>
<li><strong>Yayımlama</strong>. Yayımlama lisansları verir.<br />
<br />
</li>
<li><strong>Lisans</strong>. Kullanım lisansları verir.<br />
<br />
</li>
</ul>
Lisans sunucuları genellikle kuruluşun farklı bölümlerini desteklemek veya kök sertifika kümesinden gelen lisans istekleri yükünü azaltmak için dağıtılır. Lisans sunucuları isteğe bağlıdır.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server gibi veritabanı sunucusu</td>
<td style="border:1px solid black;"><ul>
<li>RMS yapılandırması, günlük ve dizin hizmetleri veritabanlarını çalıştırır.<br />
<br />
</li>
<li>Kök sertifika kümesinin yapılandırma veritabanındaki hak hesabı sertifikalarını depolar.<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Etki alanı denetleyicisi ve genel katalog</td>
<td style="border:1px solid black;"><ul>
<li>Kullanıcı kimlik doğrulaması ve dizin hizmetleri sağlar.<br />
<br />
</li>
<li>Kök sertifika kümesinin hizmet bulma konumunu depolar.<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

RMS, sistem için ortak güven kökü sağlamak amacıyla Microsoft tarafından barındırılan Kayıt ve Etkinleştirme hizmetlerini kullanır. Daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS Güven Hiyerarşisi](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)" bölümüne bakın.

Aşağıdaki çizimde RMS sistemindeki farklı bileşenler ve bunların sistemdeki rolleri gösterilmektedir. Oklar, farklı bileşenler arasında geçirilen istekleri ve yanıtları gösterir.

![](/security-updates/images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Her bir bileşen hakkında daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS Yazılım Bileşenleri](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca)" bölümüne bakın.
