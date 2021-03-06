---
TOCTitle: 'MS09-APR'
Title: Microsoft Güvenlik Bülteni Nisan 2009 Özeti
ms:assetid: 'ms09-apr'
ms:contentKeyID: 61235812
ms:mtpsurl: 'https://technet.microsoft.com/tr-TR/library/ms09-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Güvenlik Bülteni Nisan 2009 Özeti
===========================================

Yayım Tarihi: 14 Nisan 2009 Salı | Güncelleştirme Tarihi: 16 Nisan 2009 Perşembe

**Sürüm:** 1.1

Bu bülten özetinde Nisan 2009'da yayımlanan güvenlik bültenleri listelenir.

Nisan 2009 bültenlerinin yayımlanmasıyla birlikte, bu bülten özeti, 9 Nisan 2009'da özgün olarak yayımlanan bülten öncelikli bildiriminin yerini alır. Bülten öncelikli bildirim hizmeti hakkında daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Öncelikli Bildirimi](http://technet.microsoft.com/security/bulletin/advance).

Microsoft güvenlik bültenleri her yayımlandığında otomatik bildirimlerin nasıl alınacağı hakkında bilgi için, [Microsoft Teknik Güvenlik Bildirimleri](http://go.microsoft.com/fwlink/?linkid=21163)'ne bakın.

Microsoft, bu bültenlerle ilgili müşteri soruları için 15 Nisan 2009 günü saat 11:00'de (Pasifik Saati, ABD ve Kanada) bir Web yayını gerçekleştirecektir. [Nisan Güvenlik Bülteni Web Yayını için şimdi kaydolun](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395126). Bu tarihten sonra, Web yayını isteğe bağlı olarak kullanılabilecektir. Daha fazla bilgi için, bkz: [Microsoft Güvenlik Bülteni Özetleri ve Web Yayınları](http://technet.microsoft.com/security/bulletin/summary).

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139849">MS09-010</a></td>
<td style="border:1px solid black;"><strong>WordPad ve Office Metin Dönüştürücüleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960477)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft WordPad ve Microsoft Office metin dönüştürücülerinde genel ve özel olarak bildirilen ikişer güvenlik açığını giderir. Güvenlik açıkları, özel hazırlanmış bir dosya WordPad'de veya Microsoft Office Word'de açılırsa uzaktan kod yürütülmesine izin verebilir. Güvenilmeyen kaynaklardan gelen Microsoft Office, RTF, Write veya WordPerfect dosyalarını WordPad'in veya Microsoft Office Word'ün etkilenen sürümlerini kullanarak açmayın.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139852">MS09-013</a></td>
<td style="border:1px solid black;"><strong>Windows HTTP Hizmetleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960803)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows HTTP Hizmetleri'ndeki (WinHTTP) genel olarak bildirilen bir ve özel olarak bildirilen iki güvenlik açığını giderir. En ciddi güvenlik açığı uzaktan kod yürütülmesine olanak verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139107">MS09-011</a></td>
<td style="border:1px solid black;"><strong>Microsoft DirectShow'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (961373)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Microsoft DirectX'teki özel olarak bildirilen bir güvenlik açığını giderir. Bu güvenlik açığı, bir kullanıcı özel hazırlanmış bir MJPEG dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu açığı başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146659">MS09-014</a></td>
<td style="border:1px solid black;"><strong>Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)</strong><br />
<br />
Bu güvenlik güncelleştirmesi Internet Explorer'daki özel olarak bildirilen dört ve genel olarak duyurulan iki güvenlik açığını giderir. Bu güvenlik açıkları, bir kullanıcı özel hazırlanmış bir Web sayfasını Internet Explorer kullanarak görüntülerse veya HTTP protokolünü kullanarak saldırganın sunucusuna bağlanırsa uzaktan kod yürütülmesine olanak verebilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=143568">MS09-009</a></td>
<td style="border:1px solid black;"><strong>Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine Neden Olabilir (968557)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Office Excel'de özel olarak bildirilen ve genel olarak duyurulan birer güvenlik açığını giderir. Bu güvenlik açıkları, kullanıcı özel hazırlanmış bir Excel dosyasını açarsa uzaktan kod yürütülmesine izin verebilir. Bu açıkları başarıyla kullanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir. Saldırgan, program yükleyebilir; verileri görüntüleyebilir, değiştirebilir veya silebilir; tüm kullanıcı haklarına sahip olan yeni hesaplar oluşturabilir. Hesapları, sistemde az sayıda kullanıcı hakkıyla yapılandırılmış olan kullanıcılar, yönetici haklarıyla çalışan kullanıcılardan daha az etkilenebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Kritik</a><br />
Uzaktan Kod Yürütme</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirebilir</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132587">MS09-012</a></td>
<td style="border:1px solid black;"><strong>Windows'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (959454)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Windows'daki genel olarak duyurulan dört güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırganın sistemde oturum açmasına ve daha sonra özel hazırlanmış bir uygulamayı çalıştırmasına izin verilirse ayrıcalık yükselmesine neden olabilir. Saldırganın bu güvenlik açığından yararlanabilmesi için yerel makinede kod çalıştırabilmesi gerekir. Bu güvenlik açıklarından herhangi birinden başarıyla yararlanan bir saldırgan, etkilenen sistemin tüm denetimini ele geçirebilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Ayrıcalık Yükselmesi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141639">MS09-016</a></td>
<td style="border:1px solid black;"><strong>Microsoft ISA Server ve Forefront Threat Management Gateway'deki (Medium Business Edition) Güvenlik Açıkları Hizmet Reddine Neden Olabilir (961759)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, Microsoft Internet Security and Acceleration (ISA) Server ve Microsoft Forefront Threat Management Gateway (TMG) Medium Business Edition'da (MBE) özel olarak bildirilen ve genel olarak duyurulan birer güvenlik açığını giderir. Bu güvenlik açıkları, bir saldırgan etkilenen sisteme özel hazırlanmış ağ paketleri gönderirse hizmet reddine veya bir kullanıcı, saldırgan tarafından denetlenen içeriğe sahip olan kötü amaçlı bir URL'yi tıklatırsa ya da Web sitesini ziyaret ederse bilginin açığa çıkmasına neden olabilir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Önemli</a><br />
Hizmet Reddi</td>
<td style="border:1px solid black;">Yeniden başlatma gerektirir</td>
<td style="border:1px solid black;">Microsoft Forefront Edge Security</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=146803">MS09-015</a></td>
<td style="border:1px solid black;"><strong>SearchPath İşlevindeki Karma Tehdit Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (959426)</strong><br />
<br />
Bu güvenlik güncelleştirmesi, bir kullanıcı özel hazırlanmış bir dosyayı belirli bir konuma karşıdan yükleyip daha sonra dosyayı belirli koşullarda yükleyebilecek bir uygulamayı açarsa Windows SearchPath işlevinde ayrıcalık yükselmesine neden olabileceği genel olarak duyurulan bir güvenlik açığını giderir.</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=21140">Orta</a><br />
Ayrıcalık Yükselmesi</td>
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
  
| Bülten Kimliği                                            | Bülten Başlığı                                                                                                                                      | CVE Kimliği                                                                          | Yararlanma Dizini Değerlendirmesi                                                                                 | Önemli Notlar                                                                                                                                                                                                                                                                                                        |  
|-----------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine Neden Olabilir (968557)                                                     | [CVE-2009-0100](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0100)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-009](http://go.microsoft.com/fwlink/?linkid=143568) | Microsoft Office Excel'deki Güvenlik Açıkları Uzaktan Kod Yürütülmesine Neden Olabilir (968557)                                                     | [CVE-2009-0238](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0238)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | WordPad ve Office Metin Dönüştürücüleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960477)                                   | [CVE-2008-4841](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4841)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | WordPad ve Office Metin Dönüştürücüleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960477)                                   | [CVE-2009-0087](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0087)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Bu, birden çok kod yolu nedeniyle karmaşık bir güvenlik açığıdır. Çoğu yararlanma kodu tutarlı olmayan sonuçlar doğuracaktır. Varsayılan azaltıcı etkenler, bu vektöre karşı koruma sağlar.                                                                                                                          |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | WordPad ve Office Metin Dönüştürücüleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960477)                                   | [CVE-2009-0088](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0088)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Bu güvenlik açığından yararlanılabilir, ancak yalnızca daha eski sürümleri ve yaygın olarak kullanılmayan eski dosya biçimini etkiler. 2007 Microsoft Office sistemi ve Microsoft Office 2003 Service Pack 3 gibi daha yeni sürümler etkilenmez.                                                                     |  
| [MS09-010](http://go.microsoft.com/fwlink/?linkid=139849) | WordPad ve Office Metin Dönüştürücüleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960477)                                   | [CVE-2009-0235](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0235)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Bu bellek bozulması güvenlik açığından kolaylıkla yararlanılabilir.                                                                                                                                                                                                                                                  |  
| [MS09-011](http://go.microsoft.com/fwlink/?linkid=139107) | Microsoft DirectShow'daki Güvenlik Açığı Uzaktan Kod Yürütülmesine İzin Verebilir (961373)                                                          | [CVE-2009-0084](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0084)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Windows'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (959454)                                                                       | [CVE-2008-1436](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-1436)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Windows'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (959454)                                                                       | [CVE-2009-0078](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0078)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Windows'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (959454)                                                                       | [CVE-2009-0079](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0079)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-012](http://go.microsoft.com/fwlink/?linkid=132587) | Windows'daki Güvenlik Açıkları Ayrıcalık Yükselmesine İzin Verebilir (959454)                                                                       | [CVE-2009-0080](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0080)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | **Bu güvenlik açığından Internet ekosisteminde yararlanılmaktadır.**                                                                                                                                                                                                                                                 |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Windows HTTP Hizmetleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960803)                                                   | [CVE-2009-0086](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0086)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Bu teknolojinin yaygın olarak kullanılmasından dolayı birden çok saldırı vektörü ve fırsatı nedeniyle, bu, kolayca denetlenebilen bir bellek güvenlik açığıdır.                                                                                                                                                      |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Windows HTTP Hizmetleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960803)                                                   | [CVE-2009-0089](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0089)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-013](http://go.microsoft.com/fwlink/?linkid=139852) | Windows HTTP Hizmetleri'ndeki Güvenlik Açıkları Uzaktan Kod Yürütülmesine İzin Verebilir (960803)                                                   | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Yararlanma kodu genel kullanıma sunulmuştur.                                                                                                                                                                                                                                                                         |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Saldırı ayrıntıları genel kullanıma sunulmuştur, ancak bu sorun için bilinen bir saldırı vektörü henüz bulunmamaktadır. Bu güvenlik açığından başarıyla yararlanılabilmesi için, saldırganın ve kullanıcının belirli dosyaları masaüstüne kaydetmek de dahil bir dizi karmaşık adımı gerçekleştirmesi gerekmektedir. |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2009-0550](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0550)\*\* | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | Yararlanma kodu genel kullanıma sunulmuştur.                                                                                                                                                                                                                                                                         |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2009-0551](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0551)     | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2009-0552](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0552)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Internet Explorer 7 için azaltıcı etkenler, kod yürütülmesini engellemektedir. Internet Explorer 6 ve önceki sürümlerinde tüm güvenlik güncelleştirmeleri bulunmuyorsa, bu güvenlik açığından yararlanma olasılığı daha yüksektir.                                                                                   |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2009-0553](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0553)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-014](http://go.microsoft.com/fwlink/?linkid=146659) | Internet Explorer için Toplu Güvenlik Güncelleştirmesi (963027)                                                                                     | [CVE-2009-0554](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0554)     | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarlı     | (Yok)                                                                                                                                                                                                                                                                                                                |  
| [MS09-015](http://go.microsoft.com/fwlink/?linkid=146803) | SearchPath İşlevindeki Karma Tehdit Güvenlik Açığı Ayrıcalık Yükselmesine İzin Verebilir (959426)                                                   | [CVE-2008-2540](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2540)\*   | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - Yararlanma kodu büyük olasılıkla tutarsız    | Saldırı ayrıntıları genel kullanıma sunulmuştur, ancak bu sorun için bilinen bir saldırı vektörü henüz bulunmamaktadır. Bu güvenlik açığından başarıyla yararlanılabilmesi için, saldırganın ve kullanıcının belirli dosyaları masaüstüne kaydetmek de dahil bir dizi karmaşık adımı gerçekleştirmesi gerekmektedir. |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Microsoft ISA Server ve Forefront Threat Management Gateway'deki (Medium Business Edition) Güvenlik Açıkları Hizmet Reddine Neden Olabilir (961759) | [CVE-2009-0077](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0077)     | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Hizmet Tabanlı Hizmet Reddi olasılığı oldukça yüksektir. Ancak kod yürütülmesi mümkün değildir.                                                                                                                                                                                                                      |  
| [MS09-016](http://go.microsoft.com/fwlink/?linkid=141639) | Microsoft ISA Server ve Forefront Threat Management Gateway'deki (Medium Business Edition) Güvenlik Açıkları Hizmet Reddine Neden Olabilir (961759) | [CVE-2009-0237](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-0237)          | [**3**](http://technet.microsoft.com/en-us/security/cc998259.aspx) - İşlevsel bir yararlanma kodu olasılığı düşük | Bilginin açığa çıkması söz konusudur. Kod yürütülmesi olasılığı oldukça düşüktür.                                                                                                                                                                                                                                    |
  
\*Aynı CVE numarasının atandığı bu iki güvenlik açığı, iki ayrı güvenlik güncelleştirmesiyle giderilir. Daha fazla bilgi için ilgili bültenlere başvurun.
  
\*\*Aynı CVE numarasının atandığı bu iki güvenlik açığı, iki ayrı güvenlik güncelleştirmesiyle giderilir. Daha fazla bilgi için ilgili bültenlere başvurun.
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="7">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
(Önem derecesi yok)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=552d322a-5282-42c7-9c1e-1d8c494a7318)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=39d5468e-5733-4c3e-9e75-3adac8ac8cb9)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 8.1](http://www.microsoft.com/downloads/details.aspx?familyid=0ec5b7c7-13d3-467a-b24e-3cc6fb47adf6)  
(Kritik)  
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=8b98ed5c-a3ab-45a7-a61e-349eae304bc6)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=7799fd05-5b26-449f-8a14-50227c9164d1)  
(Kritik)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=87f0c380-5c31-4099-a6a9-c12f9d69b03b)  
(Kritik)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=52b756e7-636f-4d9e-8a17-dbf467bfbe4d)  
(KB952004)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=c4e408d7-6716-4a12-ad3a-8029667f5c84)  
(Önem derecesi yok)
</td>
</tr>
<tr>
<th colspan="7">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 ve Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=50a8519a-503e-43dd-a78a-c1bc764fd213)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=35af4151-1858-4c9a-85e4-9ff45feca1a4)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=feb5d821-f210-40e8-b1aa-2ca3170df8df)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=052c29fc-e8df-402c-9ab1-1079bc738e1b)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=55d6729a-9f96-4da4-b564-676c0a0c9390)  
(Kritik)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=90fe715e-8190-43e9-9c43-df5be564d923)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=73d2324f-be59-4b0c-b1ac-9876a13c2c03)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 ve Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3de0684d-605c-489b-bdc7-08bce9b2d4f6)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=49b16f0f-f6c3-4ca8-8041-392f4f7b5bbb)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=f1be8b7c-4874-4342-99b3-76ff725fbb9a)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=84c62211-2e82-4ccc-9f9b-26462b026d86)  
(Kritik)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=191c2f20-89ae-4e1c-bdd4-24b4abfe6b6c)  
(Kritik)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a794c32a-9a0c-47d9-9c57-ff5d4a8e4944)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b2f12ae5-0e46-47e1-ac5b-93550d030189)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition ve Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b743a7fe-7bf4-420d-a72e-39471e5659fa)  
(Orta)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
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
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2233a4d2-7c8a-4c89-b020-100d9afb43c8)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=42509f5a-d0f9-444a-9445-5eabdb555011)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=c1b4cd76-1dd6-43fa-bb9a-20c428985bfd)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f73a3669-c17f-4b18-8456-96cb7d52ed86)  
(Önemli)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=6a45dbd0-0520-4d9b-b76e-3f5109dd310d)  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=25adec10-db8c-4cac-bf74-2c784678150a)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=42aba890-8b76-4c5a-8fb6-609797d19831)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 ve Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=992bb0cd-fbc7-4a7c-9088-f7f9d9a3ead0)  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=323f4211-5add-4e02-bce1-e5a1b489982c)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7373ea32-bc2e-49f1-8b9f-4eeda5acc74c)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=f0e1e1db-94a5-451c-ab11-6b431fa065f1)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=03a9d581-2bd5-4151-9826-17b96e16f606)  
(Önemli)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=60ccc1d6-ea31-420c-b630-d7878a8dc527)  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b014c399-f404-4cb2-8f9d-864df382efeb)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a0609f65-82d9-4d82-9f48-f3266e8de123)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition ve Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=f0a58e8c-7d63-4d7d-ba95-b3787cf408f0)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=e840b9cb-f1f4-482a-aa07-eb6b42b477c4)  
(KB923561)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=05e33cc5-cff6-4c71-be71-285f66a95e01)  
(Kritik)
</td>
<td style="border:1px solid black;">
[DirectX 9.0](http://www.microsoft.com/downloads/details.aspx?familyid=8f36c215-fa8a-40c2-b680-6b1fece03b8d)\*\*\*  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=53d13c07-80b0-4f05-b372-a2dac17e6157)  
(Önemli)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0abaa2fb-7c4f-4149-993d-1575888bfc84)  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=6ada372b-ba17-433e-b022-d2c57b35af8a)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=fda8837c-e5d2-4489-9b44-4c24a1102e77)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2003 SP1 ve Itanium tabanlı sistemler için Windows Server 2003 SP2](http://www.microsoft.com/downloads/details.aspx?familyid=00c6479d-f81f-445d-b8e4-7b71d77d540a)  
(Orta)
</td>
</tr>
<tr>
<th colspan="7">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista ve Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f071d770-3b6b-4040-9911-d4de8cde4c68)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d743849d-f3b5-4114-adef-ade2716d55ac)  
(Kritik)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=f111b99a-e555-4f29-8d1f-e9ec03d5cf1f)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d0ea1598-45cb-4c79-8945-caae98969675)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista ve Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=2b672d45-f33b-4edc-9f22-2f2c8c726a8b)  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7ceef2d0-f316-48d1-aecc-d74f91cc5e1f)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=d191c8dc-a965-4a6a-b6d8-1470505eb55f)  
(Kritik)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=fa153bdc-6b48-4df2-9e5e-abacd6da782c)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6dd82f4b-bb33-41ec-90a7-9ef91329b240)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition ve Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7576e7d5-5bb1-4a53-b568-1ee0500ce721)  
(Orta)
</td>
</tr>
<tr>
<th colspan="7">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-013**](http://go.microsoft.com/fwlink/?linkid=139852)
</td>
<td style="border:1px solid black;">
[**MS09-011**](http://go.microsoft.com/fwlink/?linkid=139107)
</td>
<td style="border:1px solid black;">
[**MS09-014**](http://go.microsoft.com/fwlink/?linkid=146659)
</td>
<td style="border:1px solid black;">
[**MS09-012**](http://go.microsoft.com/fwlink/?linkid=132587)
</td>
<td style="border:1px solid black;">
[**MS09-015**](http://go.microsoft.com/fwlink/?linkid=146803)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
<td style="border:1px solid black;">
[**Orta**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
32-Bit Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=4c36548f-c8c9-4318-91e2-9e0501339548)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e2c6313c-3ba9-4f7c-b259-b4582a390146)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=9e3c7b52-65a7-42fb-beb5-1b374934737f)\*  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=d58702af-bbf8-4f1b-ae72-ced9ef23d581)\*  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[32-bit sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=6b73cf5e-66fe-4b7d-95fc-91a1c262c1e5)\*  
(Orta)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
x64 Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=1c3f0997-a8a9-4340-ae0c-2c4d6792c65c)\*  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=ebbade9d-704c-440b-8796-6d64225ac01a)\*\*  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=eebb4d4d-29d2-4247-8cbb-63a3b17585ec)\*  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=20bf4e9b-909b-4bc3-ae43-322d74a4f1c3)\*  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[x64 tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=7e60847c-b341-4c38-bc25-2e3cf2d4ae14)\*  
(Orta)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Itanium Tabanlı Sistemler için Windows Server 2008
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=0885b3b0-b78e-4980-902d-dff3886bcaac)  
(Kritik)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1b04aa6f-b787-4122-bf82-0d150618fe7a)  
(Önemli)
</td>
<td style="border:1px solid black;">
MSDTC İşlem Aracı güncelleştirmesi:  
[Itanium Tabanlı Sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=cc383c24-b0f6-47c1-9e89-6a378b09e82f)  
(KB952004)  
(Önemli)  
Windows Hizmet Yalıtımı güncelleştirmesi:  
[Itanium Tabanlı Sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=bcc2b18f-67db-4109-a9f4-764f985423ee)  
(KB956572)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Itanium tabanlı sistemler için Windows Server 2008](http://www.microsoft.com/downloads/details.aspx?familyid=de1c2b4b-af47-4b9a-8363-720e5527573c)  
(Orta)
</td>
</tr>
</table>
 
**Windows Server 2008 için Notlar**

**\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenir.** Windows Server 2008'in desteklenen sürümleri için, bu güncelleştirme, Windows Server 2008'in Sunucu Çekirdeği yükleme seçeneği kullanılarak yüklenmiş olup olmadığına bakılmaksızın aynı önem derecesiyle uygulanır. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**\*\*Windows Server 2008 sunucu çekirdeği yüklemesi etkilenmez.** Windows Server 2008'i Sunucu Çekirdeği yükleme seçeneğiyle yüklediyseniz, bu güncelleştirme tarafından giderilen güvenlik açıkları Windows Server 2008'in desteklenen sürümlerini etkilemez. Bu yükleme seçeneği hakkında daha fazla bilgi için, bkz: [Sunucu Çekirdeği](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Sunucu Çekirdeği yükleme seçeneği Windows Server 2008'in belirli sürümlerinde kullanılamaz; bkz: [Sunucu Çekirdeği Yükleme Seçeneklerini Karşılaştırma](http://www.microsoft.com/windowsserver2008/en/us/compare-core-installation.aspx).

**MS09-010 için Not**

Diğer güncelleştirme dosyaları için **Microsoft Office Paketleri ve Yazılımları** adlı bölüme de bakın. Bu bülten hem Windows İşletim Sistemi ve Bileşenleri hem de Microsoft Office Paketleri ve Yazılımları içindir.

**MS09-011 için Not**

\*\*\*DirectX 9.0 güncelleştirmesi DirectX 9.0a, DirectX 9.0b ve DirectX 9.0c için de uygulanır.

#### Microsoft Office Paketleri ve Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3">
Microsoft Office Paketleri, Sistemleri ve Bileşenleri
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
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
[**Kritik**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=95876927-e612-414c-bdec-3632a3100415)  
(KB921606)  
(Kritik)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=3dc8b670-25a5-4f46-b7de-12bc693b628a)  
(KB959964)  
(Kritik)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=e1db55c6-78fb-498d-89a5-9ad54d971546)  
(KB933399)  
(Önemli)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=9a52bf4b-05f6-4b73-94b9-28ed7e20f86c)  
(KB959988)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d9dbfa63-c0cb-4c84-9b8a-6e52568045b0)  
(KB959995)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
2007 Microsoft Office Sistemi Service Pack 1
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=50d8630b-1365-4007-81a0-18c0d6d4b86e)\*  
(KB959997)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="3">
Mac için Microsoft Office
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Mac için Microsoft Office 2004
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2004](http://www.microsoft.com/downloads/details.aspx?familyid=52271140-89be-4b9c-baa2-cea09097d703)  
(KB968695)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Mac için Microsoft Office 2008
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Mac için Microsoft Office 2008](http://www.microsoft.com/downloads/details.aspx?familyid=f6e407eb-11a5-433f-8006-4b822953ca98)  
(KB968694)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="3">
Diğer Office Yazılımları
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-010**](http://go.microsoft.com/fwlink/?linkid=139849)
</td>
<td style="border:1px solid black;">
[**MS09-009**](http://go.microsoft.com/fwlink/?linkid=143568)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
Yok
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=c72e6087-b48f-4d2d-8366-01d9f5ff6b6c)  
(KB959993)  
(Önemli)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?familyid=58b3929c-5373-47a4-aa97-66d179758792)  
(KB960000)  
(Önemli)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
<td style="border:1px solid black;">
[Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=05f7c517-e551-4dcd-b24a-5d548f2d09cf)  
(KB960003)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Dönüştürücü Paketi
</td>
<td style="border:1px solid black;">
[Microsoft Office Dönüştürücü Paketi](http://www.microsoft.com/downloads/details.aspx?familyid=d763fae3-b2af-47f9-a554-ec786766b3c3)  
(KB960476)  
(Önemli)
</td>
<td style="border:1px solid black;">
Uygulanamaz
</td>
</tr>
</table>
 
**MS09-010 için Not**

Diğer güncelleştirme dosyaları için **Windows İşletim Sistemi ve Bileşenleri** bölümüne de bakın. Bu bülten hem Windows İşletim Sistemi ve Bileşenleri hem de Microsoft Server Yazılımı içindir.

**MS09-009 için Not**

\*Microsoft Office Excel 2007 Service Pack 1 için, müşterilerin bu bültende açıklanan güvenlik açıklarına karşı korunmak üzere Word, Excel ve PowerPoint 2007 Dosya Biçimleri için Microsoft Office Uyumluluk Paketi Service Pack 1'e yönelik güvenlik güncelleştirmesini de yüklemeleri gerekmektedir.

#### Microsoft Sunucu ve Güvenlik Yazılımları

 
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2">
Microsoft Forefront
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Threat Management Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Threat Management Gateway Medium Business Edition](http://www.microsoft.com/downloads/details.aspx?familyid=6abf9fb4-42d0-4c67-935f-8dc67850148b)\*  
(KB968075)  
(Önemli)
</td>
</tr>
<tr>
<th colspan="2">
Internet Security and Acceleration Server
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bülten Tanımlayıcısı**
</td>
<td style="border:1px solid black;">
[**MS09-016**](http://go.microsoft.com/fwlink/?linkid=141639)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Toplam Önem Derecesi**
</td>
<td style="border:1px solid black;">
[**Önemli**](http://go.microsoft.com/fwlink/?linkid=21140)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2004 Standard Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=adf623fa-2d74-4f2a-9835-4b8debdb0e1b)\*\*  
(KB960995)  
(Önemli)  
[Microsoft Internet Security and Acceleration Server 2004 Enterprise Edition Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=d1d55ab6-3de5-4811-9693-8d43f49f5fe8)  
(KB960995)  
(Önemli)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Internet Security and Acceleration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Internet Security and Acceleration Server 2006](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Önemli)  
[Microsoft Internet Security and Acceleration Server 2006 Supportability Update](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Önemli)  
[Microsoft Internet Security and Acceleration Server 2006 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=eda30bcc-0582-4f60-a4c5-ea5000b7c770)  
(KB968078)  
(Önemli)
</td>
</tr>
</table>
 
**MS09-016 için Not**

\*Microsoft Forefront Threat Management Gateway Medium Business Edition tek başına bir ürün olarak ve Windows Essential Business Server 2008'in bir bileşeni olarak edinilebilir.

\*\*Microsoft ISA Server 2004 Standard Edition tek başına bir ürün olarak edinilebilir. Microsoft ISA Server 2004 Standard Edition, Windows Small Business Server 2003 Enterprise Edition Service Pack 1'in Windows Small Business Server 2003 R2 Enterprise Edition'ın bir bileşeni olarak da edinilebilir.

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
-   [Microsoft Windows Dışındaki Microsoft Ürünleri için Yeni, Yeniden Düzenlenen ve Yayımlanan Güncelleştirmeler](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

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

-   Fortinet bünyesindeki [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) için çalışan Haifei Li, MS09-009'da açıklanan sorunu bildirdiği için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) için çalışan Sean Larsson ve Jun Mao, MS09-010'da açıklanan sorunu bildirdikleri için
-   Fortinet bünyesindeki [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) ile birlikte çalışan bir araştırmacı, MS09-010'da açıklanan sorunu bildirdikleri için
-   [VeriSign iDefense Labs](http://labs.idefense.com/) ile birlikte çalışan bir araştırmacı, MS09-010'da açıklanan sorunu bildirdikleri için
-   [Kryptos Logic](http://www.kryptoslogic.com/) için çalışan Piotr Bania, MS09-011'de açıklanan sorunu bildirdiği için
-   [Argeniss](http://www.argeniss.com/) için çalışan Cesar Cerrudo, MS09-012'de açıklanan sorunu bildirdiği için
-   [iSIGHT Partners Labs](http://www.isightpartners.com/) için çalışan Greg MacManus, MS09-013'te açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan Wan-Teh Chang ve Cem Paya, MS09-013'te açıklanan sorunu bildirdikleri için
-   [Aviv Raff](http://aviv.raffon.net/), MS09-014'te açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan Michal Zalewski, MS09-014'te açıklanan sorunu bildirdiği için
-   [iSIGHT Partners Labs](http://www.isightpartners.com/) için çalışan Ivan Fratric, MS09-014'te açıklanan sorunu bildirdiği için
-   [Google Inc.](http://www.google.com/) için çalışan Skylined, MS09-014'te açıklanan sorunu bildirdiği için
-   [VenusTech](http://www.venustech.com.cn/) için çalışan ADLab, MS09-014'te açıklanan sorunu bildirdiği için
-   [Aviv Raff](http://aviv.raffon.net/), MS09-015'te açıklanan sorunu bildirdiği için
-   New York Eyaleti Bilişim Müdürü / Teknoloji Bürosu, MS09-016'da açıklanan sorunu bildirdiği için

#### Destek

-   Listelenen etkilenen yazılımlar, hangi sürümlerinin etkilendiğini belirlemek amacıyla sınanmıştır. Diğer sürümler destek ömrünü tamamlamıştır. Yazılım sürümünüzün destek ömrünü belirlemek için [Microsoft Destek Ömrü](http://go.microsoft.com/fwlink/?linkid=21742) Web sitesini ziyaret edin.
-   ABD ve Kanada'daki müşterilerimiz, [Güvenlik Desteği](http://go.microsoft.com/fwlink/?linkid=21131)'nden veya 1-866-PCSAFETY numaralı telefondan teknik destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Kullanılabilir destek seçenekleri hakkında daha fazla bilgi için, bkz: [Microsoft Yardım ve Destek](http://support.microsoft.com/).
-   Uluslararası müşterilerimiz, yerel Microsoft temsilcilerinden destek alabilir. Güvenlik güncelleştirmeleriyle ilgili olan destek görüşmelerinden ücret alınmaz. Destek sorunlarıyla ilgili olarak Microsoft'a başvurma konusunda daha fazla bilgi için [Uluslararası Destek ve Yardım](http://go.microsoft.com/fwlink/?linkid=21155) Web sitesini ziyaret edin.

#### Sorumluluğun Kaldırılması

Microsoft Bilgi Bankası'nda sağlanan bilgiler hiçbir garanti olmadan "olduğu gibi" sağlanır. Microsoft, ticari olarak satılabilirlik ve belirli bir amaca uygunluk da dahil olmak üzere doğrudan ya da dolaylı hiçbir garanti vermemektedir. Microsoft Corporation veya tedarikçileri, bu gibi zararlar olabileceği Microsoft Corporation veya tedarikçilerine önceden bildirilmiş olsa dahi, doğrudan, dolaylı, arızi, neticede oluşan, gelir kaybına neden olan ya da özel hiçbir hasar için sorumlu tutulamaz. Bazı eyaletlerde, neticede oluşan ya da kaza sonucu oluşan hasarların kapsam dışında tutulmasına ya da sınırlanmasına izin verilmediği için bu kısıtlamalar uygulanmayabilir.

#### Düzenlemeler

-   V1.0 (14 Nisan 2009): Bülten Özeti yayımlandı.
-   V1.1 (16 Nisan 2009): Yararlanma Dizini güncelleştirildi: MS09-014 ve MS09-015'te CVE-2009-0089 anahtar notları kaldırıldı ve CVE-2008-2540 anahtar notları değiştirildi.

*Built at 2014-04-18T01:50:00Z-07:00*
