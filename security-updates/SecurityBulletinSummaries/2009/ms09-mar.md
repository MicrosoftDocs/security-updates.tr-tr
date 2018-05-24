---
TOCTitle: 'MS09-MAR'
Title: Microsoft Güvenlik Bülteni Mart 2009 Özeti
ms:assetid: 'ms09-mar'
ms:contentKeyID: 61235819
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms09-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Mart 2009 Özeti
==========================================

Yayım Tarihi: 10 Mart 2009 Salı | Güncelleştirme Tarihi: 11 Mart 2009 Çarşamba

**Sürüm:** 1.1

Bu bülten özetinde Mart 2009'da yayımlanan güvenlik bültenleri listelenir.

Mart 2009 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 5 Mart 2009'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 11 Mart 2009 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Mart Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395124). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

Microsoft, müşterilerin aylık güvenlik güncelleştirmeleriyle aynı gün yayımlanan güvenlikle ilgili olmayan yüksek öncelikli güncelleştirmelerle aylık güvenlik güncelleştirmelerinin önceliklerini belirlemelerine yardımcı olan bilgiler de sağlar. **Diğer Bilgiler** bölümüne bakın.

### Bülten Bilgileri

Yürütmeyle İlgili Özetler
-------------------------

<span></span>
Aşağıdaki tabloda, bu ayın güvenlik bültenleri önem derecesine göre özetlenmektedir.

Etkilenen yazılımlar ile ilgili ayrıntılar için **Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları** adlı sonraki bölüme bakın.

 
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bülten Kimliği</th>
<th style="border:1px solid black;" >Bülten Başlığı ve Yürütmeyle İlgili Özet</th>
<th style="border:1px solid black;" >En Yüksek Önem Derecesi ve Güvenlik Açığının Etkisi</th>
<th style="border:1px solid black;" >Yeniden Başlatma Gereksinimi</th>
<th style="border:1px solid black;" >Etkilenen Yazılımlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132503">MS09-006</a></td>
<td style="border:1px solid black;"><strong>Windows Çekirdeğindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958690)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows çekirdeğindeki özel olarak bildirilen birkaç güvenlik açığını giderir. Bunların arasında en önemlisi olan güvenlik açığı, bir kullanıcı etkilenen bir sistemdeki özel hazırlanmış bir EMF veya WMF resim dosyasını görüntülerse uzaktan kod yürütülmesine izin verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139854">MS09-007</a></td>
<td style="border:1px solid black;"><strong>SChannel'deki Güvenlik Açığı Kimlik Sahtekarlığına Neden Olabilir (960225)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Windows'daki Güvenli Kanal (SChannel) güvenlik paketindeki özel olarak bildirilen bir güvenlik açığını giderir. Güvenlik açığı, bir saldırgan kimlik doğrulama için son kullanıcı tarafından kullanılan sertifikaya erişim sağlarsa kimlik sahtekarlığına olanak verebilir. Müşteriler yalnızca kimlik doğrulaması için kullanılan ortak anahtar bileşeni başka yollarla saldırganın eline geçmişse bu güvenlik açığından etkilenir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Sızdırma</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139821">MS09-008</a></td>
<td style="border:1px solid black;"><strong>DNS ve WINS Sunucusundaki Güvenlik Açıkları Kimlik Sahtekarlığına Neden Olabilir (962238)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Windows DNS sunucusundaki ve Windows WINS sunucusundaki özel ve genel olarak bildirilen ikişer güvenlik açığını giderir. Bu güvenlik açıkları bir uzak saldırganın Internet üzerindeki sistemlere gönderilen trafiği kendi sistemlerine yönlendirmesine olanak verebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Sızdırma</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Yararlanma Dizini  
-----------------
  
<span></span>
Aşağıdaki tabloda, bu ay bildirilen güvenlik açıklarının her biri için yararlanılabilirlik değerlendirmesi sağlanmaktadır. Güvenlik açıkları, bülten numarasına ve CVE numarasına göre listelenmektedir.
  
**Bu tabloyu nasıl kullanacağım?**  
  
Bu tabloyu, yüklemeniz gerekebilecek her güvenlik güncelleştirmesi için, güvenlik bülteni yayımlandıktan sonraki 30 gün içinde yayımlanacak yararlanma kodunun işlevsel olma olasılığını öğrenmek amacıyla kullanın. Geliştirme önceliklerinizi belirlemek için, kendi yapılandırmanıza uygun olarak aşağıdaki değerlendirmelerin her birini incelemelisiniz. Bu derecelendirmelerin ne anlama geldiği ve nasıl belirlendiği konusunda daha fazla bilgi için [Microsoft Yararlanma Dizini](http://technet.microsoft.com/en-us/security/cc998259.aspx)'ne bakın.
  
| Bülten Kimliği                                            | Bülten Başlığı                                                                             | CVE Kimliği                                                                      | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                                                                                                                                                         |  
|-----------------------------------------------------------|--------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-006](http://go.microsoft.com/fwlink/?linkid=132503) | Windows Çekirdeğindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958690) | [CVE-2009-0081](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0081) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Tutarlı şekilde hizmet reddi olasılığı, güvenilir ve işlevsel şekilde kod yürütülmesinden daha yükseltir                                                                                              |  
| [MS09-006](http://go.microsoft.com/fwlink/?linkid=132503) | Windows Çekirdeğindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958690) | [CVE-2009-0082](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0082) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Tutarlı şekilde hizmet reddi olasılığı, güvenilir ve işlevsel şekilde kod yürütülmesinden daha yükseltir                                                                                              |  
| [MS09-006](http://go.microsoft.com/fwlink/?linkid=132503) | Windows Çekirdeğindeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (958690) | [CVE-2009-0083](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0083) | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Yerel tehdit yalnızca tutarlı şekilde hizmet reddi veya bilginin açığa çıkması durumunda söz konusudur ve bu olasılık, güvenilir ve işlevsel şekilde kod yürütülmesinden daha yükseltir               |  
| [MS09-007](http://go.microsoft.com/fwlink/?linkid=139854) | SChannel'deki Güvenlik Açığı Kimlik Sahtekarlığına Neden Olabilir (960225)                 | [CVE-2009-0085](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0085) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenilir şekilde yararlanma olasılığı için gereksinimler yüksek ve önemli müşteri senaryolarının sayısı düşüktür                                                                                     |  
| [MS09-008](http://go.microsoft.com/fwlink/?linkid=139821) | DNS ve WINS Sunucusundaki Güvenlik Açıkları Kimlik Sahtekarlığına Neden Olabilir (962238)  | [CVE-2009-0093](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0093) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenlik açığının kanıtı olabilecek kod örneği tutarlı şekilde sızdırılabilir, ancak kötü amaçlı kod yürütülmesine neden olabilecek işlevsel yararlanma kodu oluşturulması olasılığı oldukça düşüktür |  
| [MS09-008](http://go.microsoft.com/fwlink/?linkid=139821) | DNS ve WINS Sunucusundaki Güvenlik Açıkları Kimlik Sahtekarlığına Neden Olabilir (962238)  | [CVE-2009-0094](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0094) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenlik açığının kanıtı olabilecek kod örneği tutarlı şekilde sızdırılabilir, ancak kötü amaçlı kod yürütülmesine neden olabilecek işlevsel yararlanma kodu oluşturulması olasılığı oldukça düşüktür |  
| [MS09-008](http://go.microsoft.com/fwlink/?linkid=139821) | DNS ve WINS Sunucusundaki Güvenlik Açıkları Kimlik Sahtekarlığına Neden Olabilir (962238)  | [CVE-2009-0233](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0233) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenlik açığının kanıtı olabilecek kod örneği tutarlı şekilde sızdırılabilir, ancak kötü amaçlı kod yürütülmesine neden olabilecek işlevsel yararlanma kodu oluşturulması olasılığı oldukça düşüktür |  
| [MS09-008](http://go.microsoft.com/fwlink/?linkid=139821) | DNS ve WINS Sunucusundaki Güvenlik Açıkları Kimlik Sahtekarlığına Neden Olabilir (962238)  | [CVE-2009-0234](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0234) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Güvenlik açığının kanıtı olabilecek kod örneği tutarlı şekilde sızdırılabilir, ancak kötü amaçlı kod yürütülmesine neden olabilecek işlevsel yararlanma kodu oluşturulması olasılığı oldukça düşüktür |
  
Etkilenen Yazılımlar ve Karşıdan Yükleme Konumları  
--------------------------------------------------
  
<span></span>
Aşağıdaki tablolarda, bültenler başlıca yazılım kategorilerine ve önem derecelerine göre listelenmektedir.
  
**Bu tabloları nasıl kullanabilirim?**  
  
Bu tabloları, yüklemeniz gerekebilecek güvenlik güncelleştirmelerini öğrenmek için kullanın. Listelenen her bir yazılım programını veya bileşeni inceleyip, yüklemenizle ilişkili güvenlik güncelleştirmeleri olup olmadığına bakmalısınız. Listelenen bir yazılım programı veya bileşen varsa, kullanılabilir yazılım güncelleştirmesinin bağlantısı sunulur ve ayrıca yazılım güncelleştirmesinin önem derecesi listelenir.
  
**Not** Tek bir güvenlik açığı için birkaç güvenlik güncelleştirmesi yüklemeniz gerekebilir. Listelenen her bülten tanımlayıcısı için sütunun tamamını inceleyip, sisteminize yüklemiş olduğunuz programlara veya bileşenlere bağlı olarak, yüklemeniz gereken güncelleştirmeleri doğrulayın.
  
#### Windows İşletim Sistemi ve Bileşenleri

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://go.microsoft.com/fwlink/?linkid=139821)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=98bb7d40-89a0-470a-8eb7-06f15072a635)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=bf7065bc-c183-4a78-8d46-72fe7385c07c)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Server Service Pack 4 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=110354f7-5ece-4c4d-b563-3adba6ac0116)  
(961063)  
(Önemli)  
[Microsoft Windows 2000 Server Service Pack 4 üzerinde WINS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=4319abb3-1ea2-466a-a815-c0b3b86b4462)  
(961064)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="4">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://go.microsoft.com/fwlink/?linkid=139821)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e09641ba-6cbe-4095-82b5-703d3a7dc33b)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=942d87f6-3cb1-4d36-a70a-70d9c34488f3)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d0d704c6-48c2-4907-b6c3-2455d7cf21c8)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6d02306e-9e2e-4ae8-bd21-8a2c1a229472)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://go.microsoft.com/fwlink/?linkid=139821)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f5cfb8da-e7cc-4183-8631-507c2a406500)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0b3f6fdd-276e-4267-99d8-8f00d91ad6a2)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=6cc42c9e-c34e-4577-8b23-9e07e2369878)  
(961063)  
(Önemli)  
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2 üzerinde WINS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=049e5db5-7315-4188-99fd-4a54833e6bf2)  
(961064)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ecf75c70-8489-41ad-9759-3a07e13957be)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=ce98ff55-f565-469d-bbd2-32b681faf908)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=b1f81fd2-0099-4450-8543-0459561d22d0)  
(961063)  
(Önemli)  
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2 üzerinde WINS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=4a393c63-eff5-4c8c-9c3f-33ce45c32428)  
(961064)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=04be3d7e-7dda-4dca-887a-e7a8156ede1c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=5ca3c72c-cadb-4b0a-b3a3-fb81d0bfd7b3)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=d3ed7d9a-d652-4bd0-aecc-5a415bec6c59)  
(961063)  
(Önemli)  
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2 üzerinde WINS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=37e3a75e-0a5d-4df0-881f-cdb87efa4dcf)  
(961064)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="4">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://go.microsoft.com/fwlink/?linkid=139821)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=4b1aaaba-f355-4265-83c0-50b901856ced)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=21086a04-402a-4940-8358-7fa63508102b)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=0fcac480-d6db-4a94-8c7d-b7319282cf56)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=c75a2ea9-b42f-457b-be09-5c8fa0339388)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
<tr>
<th colspan="4">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-006**](http://go.microsoft.com/fwlink/?linkid=132503)
</td>
<td style="border:1px solid black;">
[**MS09-007**](http://go.microsoft.com/fwlink/?linkid=139854)
</td>
<td style="border:1px solid black;">
[**MS09-008**](http://go.microsoft.com/fwlink/?linkid=139821)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-Bit Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=38851df2-4fb5-4d28-9d15-181c260cf8cf)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=47b361ce-624b-466c-b5c5-8703f6532615)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=92e89882-d656-4b61-a05c-3afb44895f08)\*  
(961063)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=ec15acc4-3e0f-4414-9383-61c122ff1382)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=5c81ac45-60e6-4121-ab6b-d3b3179aacc4)\*  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008 üzerinde DNS sunucusu](http://www.microsoft.com/downloads/details.aspx?familyid=be068d06-5939-4ad8-8191-e85931ed610f)\*  
(961063)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=eead6f93-10fd-4492-8137-481d9876a5fe)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=bf8f5a86-1757-4f9b-b632-d4aa7005a9f8)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**Windows Server 2008 için Notlar**

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz. [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz. [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

Algılama ve Dağıtım Araçları ve Kılavuzu
----------------------------------------

<span></span>
**Güvenlik Merkezi**

Kuruluşunuzdaki sunuculara, masaüstü bilgisayarlara ve taşınabilir bilgisayarlara dağıtmanız gereken yazılımları ve güvenlik güncelleştirmelerini yönetin. Daha fazla bilgi için, bkz: [TechNet Update Management Center](http://go.microsoft.com/fwlink/?linkid=69903). [TechNet Security Center](http://go.microsoft.com/fwlink/?linkid=21171), Microsoft ürünlerinde güvenlik konusunda ek bilgi sağlar. Müşteriler, bu bilgilerin "En Son Güvenlik Güncelleştirmeleri" tıklatılarak da edinilebileceği [Evde Güvenlik](http://go.microsoft.com/fwlink/?linkid=85102) sitesini de ziyaret edebilir.

Güvenlik güncelleştirmeleri [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) ve [Office Update](http://go.microsoft.com/fwlink/?linkid=21135) sitesinden edinilebilir. Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden de edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.

Son olarak, güvenlik güncelleştirmeleri [Microsoft Update Kataloğu](http://go.microsoft.com/fwlink/?linkid=96155)'ndan karşıdan yüklenebilir. Microsoft Update Kataloğu, Windows Update ve Microsoft Update aracılığıyla sunulan güvenlik güncelleştirmeleri, sürücüler ve hizmet paketleri gibi içeriğin arama yapılabilen bir kataloğunu sunar. Güvenlik bülteni numarasını kullanarak arama yaptığınızda (“MS07-036” gibi), uygulanabilen tüm güncelleştirmeleri sepete ekleyebilir (bir güncelleştirmenin farklı dilleri de dahil) ve istediğiniz klasöre karşıdan yükleyebilirsiniz. Microsoft Update Kataloğu hakkında daha fazla bilgi için, bkz: [Microsoft Update Kataloğu Hakkında SSS](http://go.microsoft.com/fwlink/?linkid=97900).

**Algılama ve Dağıtım Kılavuzu**

Microsoft bu ayın güvenlik güncelleştirmeleri için algılama ve dağıtım kılavuzu sağlamıştır. Bu kılavuz, ayrıca BT uzmanlarının güvenlik güncelleştirmesini dağıtmak amacıyla Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Algılama Aracı, Microsoft Systems Management Server (SMS) ve Genişletilmiş Güvenlik Güncelleştirmesi Envanter Aracı (ESUIT) gibi çeşitli araçları nasıl kullanabileceklerini anlamalarına yardımcı olur. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Microsoft Baseline Security Analyzer (MBSA), yöneticilerin eksik güvenlik güncelleştirmeleri ve ayrıca sık rastlanan güvenlik yapılandırması hataları için yerel ve uzak sistemleri taramasına olanak sağlar. MBSA hakkında daha fazla bilgi için [Microsoft Baseline Security Analyzer](http://go.microsoft.com/fwlink/?linkid=21134) Web sitesini ziyaret edin.

**Windows Server Update Services**

Windows Server Update Services'ı (WSUS) kullanarak, yöneticiler en son kritik güncelleştirmeleri ve güvenlik güncelleştirmelerini Windows 2000 işletim sistemlerine ve sonrasına, Office XP'ye ve sonrasına, Exchange Server 2003'e, SQL Server 2000'e, Windows 2000 ve sonraki işletim sistemi sürümlerine hızla ve güvenle dağıtabilir.

Bu güvenlik güncelleştirmesini Windows Server Update Services kullanarak dağıtma hakkında daha fazla bilgi için, [Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=50120) Web sitesini ziyaret edin.

**Systems Management Server**

Microsoft Systems Management Server (SMS), güncelleştirmeleri yönetmek için yüksek düzeyde yapılandırılabilir bir kuruluş çözümü sunar. SMS kullanarak, yöneticiler güvenlik güncelleştirmelerine gereksinimi olan Windows tabanlı sistemleri belirleyebilir ve bu güncelleştirmeleri son kullanıcıların çalışmasını en az düzeyde etkileyerek kuruluş genelinde denetimli bir şekilde dağıtabilir. SMS'nin yeni sürümü olan System Center Configuration Manager 2007 artık kullanılabilir; ayrıca bkz. [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx). Yöneticilerin güvenlik güncelleştirmelerini dağıtmak için SMS 2003'ü nasıl kullanacakları hakkında daha fazla bilgi için, bkz. [SMS 2003 Güvenlik Düzeltme Eki Yönetimi](http://go.microsoft.com/fwlink/?linkid=22939). SMS 2.0 kullanıcıları, güvenlik güncelleştirmelerinin dağıtılmasına yardımcı olması için [Software Update Services Feature Pack](http://go.microsoft.com/fwlink/?linkid=33340)'i de kullanabilir. SMS hakkında daha fazla bilgi için, [Microsoft Systems Management Server](http://go.microsoft.com/fwlink/?linkid=21158) Web sitesini ziyaret edin.

**Not** SMS, güvenlik bülteni güncelleştirmesi algılama ve dağıtımı konusunda geniş destek sağlamak için, Microsoft Baseline Security Analyzer'ı ve Microsoft Office Algılama Aracı'nı kullanır. Bazı yazılım güncelleştirmeleri bu araçlar tarafından algılanmayabilir. Yöneticiler, bu durumlarda SMS'nin envanter becerilerini kullanarak güncelleştirmeleri belirli sistemlere hedefleyebilir. Bu yordam hakkında daha fazla bilgi için, bkz: [SMS Yazılım Dağıtma Özelliğini Kullanarak Yazılım Güncelleştirmelerini Dağıtma](http://go.microsoft.com/fwlink/?linkid=33341). Bazı güvenlik güncelleştirmeleri bilgisayarın yeniden başlatılmasının ardından yönetimsel haklar gerektirir. Yöneticiler, bu güncelleştirmeleri yüklemek için Elevated Rights Deployment Tool'u kullanabilir ([SMS 2003 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=33387) ve [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) içinde bulunur).

**Güncelleştirme Uyumluluğu Değerlendiricisi ve Uygulama Uyumluluğu Araç Takımı**

Güncelleştirmeler genelde uygulamalarınızın çalışması için gerekli olan aynı dosyalara ve kayıt defteri ayarlarına yazar. Bu durum da uyumsuzlukları tetikleyebilir ve güvenlik güncelleştirmelerinin dağıtılması için gereken zamanı artırabilir. [Uygulama Uyumluluğu Araç Takımı 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) ile birlikte gelen [Güncelleştirme Uyumluluğu Değerlendiricisi](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true) bileşenlerini kullanarak, Windows güncelleştirmelerinin yüklü uygulamalara göre sınanması ve doğrulanması sürecini hızlandırabilirsiniz.

Uygulama Uyumluluğu Araç Takımı (ACT), çalışma ortamınıza Microsoft Windows Vista'yı, bir Microsoft Güvenlik Güncelleştirmesi'ni ya da Windows Internet Explorer'ın yeni bir sürümünü dağıtmadan önce uygulama uyumluluğu sorunlarını değerlendirmek ve etkilerini azaltmak için kullanılabilecek gerekli araçları ve belgeleri içerir.

### Diğer Bilgiler

#### Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı

Microsoft, Windows Update, Microsoft Update, Windows Server Update Services ve Yükleme Merkezi'nde Microsoft Windows Kötü Amaçlı Yazılımları Temizleme Aracı'nın güncelleştirilmiş bir sürümünü yayımladı.

#### MU, WU ve WSUS'deki Güvenlikle İlgili Olmayan Yüksek Öncelikli Güncelleştirmeler

Windows Update ve Microsoft Update sitesindeki güvenlikle ilgili olmayan yayınlar hakkında bilgi için, bkz:

-   [Microsoft Bilgi Bankası makalesi 894199](http://support.microsoft.com/kb/894199): Yazılım Güncelleştirme Hizmetleri ve Windows Server Güncelleştirme Hizmetleri'nin tanımı içeriğe bağlı olarak değişir. Tüm Windows içeriğini içerir.
-   [Microsoft Windows Dışındaki Microsoft Ürünleri için Yeni, Yeniden Düzenlenen ve Yayımlanan Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Microsoft Etkin Koruma Programı (MAPP)

Microsoft müşterilerinin güvenlik korumalarını artırmak için, güvenlik açığı bilgilerini aylık güvenlik güncelleştirmesi yayın döngüsünden daha önce başlıca güvenlik yazılımı sağlayıcılarına sunmaktadır. Güvenlik yazılımı sağlayıcıları böylece bu güvenlik açığı bilgilerini kullanarak müşterilere virüsten koruma, ağ tabanlı davetsiz giriş algılama sistemleri veya ana bilgisayar tabanlı davetsiz giriş algılama sistemleri gibi güvenlik yazılımları ya da aygıtları aracılığıyla güncelleştirilmiş koruma sağlayabilirler. Güvenlik yazılımı sağlayıcıları tarafından hazırlanmış etkin korumaların bulunup bulunmadığını belirlemek üzere, [Microsoft Etkin Koruma Programı (MAPP) Ortakları](http://www.microsoft.com/security/msrc/mapp/partners.mspx) altında listelenen program ortaklarınca sağlanan etkin koruma Web sitelerini ziyaret edin.

#### Güvenlik Stratejileri ve Topluluğu

**Güncelleştirme Yönetim Stratejileri**

[Security Guidance for Update Management](http://go.microsoft.com/fwlink/?linkid=21168) Web sitesi, güvenlik güncelleştirmelerini uygulamayla ilgili Microsoft'un en iyi uygulama önerilerini sağlar.

**Diğer Güvenlik Güncelleştirmelerini Edinme**

Diğer güvenlik sorunlarıyla ilgili güncelleştirmeler aşağıdaki konumlardan edinilebilir:

-   Güvenlik güncelleştirmeleri [Microsoft Yükleme Merkezi](http://go.microsoft.com/fwlink/?linkid=21129)'nden edinilebilir. "güvenlik güncelleştirmesi" anahtar sözcüğünü aratarak kolayca bulabilirsiniz.
-   Tüketici platformlarına yönelik güncelleştirmeler [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) Web sitesinden edinilebilir.
-   Windows Update sitesinde bu ay için sunulan güvenlik güncelleştirmelerini, Yükleme Merkezi'nden Güvenlik ve Kritik Sürümler ISO CD'si Yansıması dosyaları olarak edinebilirsiniz. Daha fazla bilgi için, bkz: [Microsoft Bilgi Bankası makalesi 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Topluluğu**

Güvenliği geliştirmeyi ve BT altyapınızı en iyi duruma getirmeyi öğrenin; ayrıca [IT Pro Security Topluluğu](http://go.microsoft.com/fwlink/?linkid=21164)'nda güvenlik konularında diğer BT Uzmanlarının çalışmalarına katılın.

#### İlgili Kaynaklar

Microsoft, müşterilerimizi korumamıza yardım etmek için bizimle işbirliği yapan aşağıdaki kişi ve kuruluşlara [teşekkür eder](http://go.microsoft.com/fwlink/?linkid=21127):

-   Helmut Buhler (<http://home.arcor.de/clipboarder/>), MS09-006'da açıklanan sorunu bildirdiği için
-   [SkyRecon](http://www.skyrecon.com/) için çalışan Thomas Garnier, MS09-006'da açıklanan sorunu bildirdiği için
-   [Secretaria da Fazenda do Estado do Rio Grande do Sul](http://www.sefaz.rs.gov.br/), MS09-007'de açıklanan sorunu bildirdikleri için
-   [Cia de Processamento de Dados do Estado do Rio Grande do Sul](http://www.procergs.rs.gov.br/), MS09-007'de açıklanan sorunu bildirdikleri için
-   Kevin Day, MS09-008'de açıklanan iki sorun konusunda bizimle çalıştığı için
-   [Georgia Tech Information Security Center](http://www.gtisc.gatech.edu/) için çalışan Dave Dagon, MS09-008'de açıklanan iki sorun konusunda bizimle çalıştığı için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, 1-866-PCSAFETY numarasını arayarak [Microsoft Ürün Destek Hizmetleri](http://go.microsoft.com/fwlink/?linkid=21131)'nden teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz.
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (10 Mart 2009): Bülten özeti yayımlandı.
-   V1.1 (11 Mart 2009): MS09-008 için Bulucu bilgileri güncelleştirildi.

*Built at 2014-04-18T01:50:00Z-07:00*
