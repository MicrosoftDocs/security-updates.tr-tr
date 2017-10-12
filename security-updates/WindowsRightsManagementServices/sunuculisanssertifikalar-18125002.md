---
TOCTitle: Sunucu Lisans Sertifikaları
Title: Sunucu Lisans Sertifikaları
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18125002
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720184(v=WS.10)'
---

Sunucu Lisans Sertifikaları
===========================

Sunucu lisans sertifikası, RMS sunucusuna sertifika ve lisans verme hakkı verir. RMS dağıtımınızın ilk kök sertifika sunucusu sağlandığında, Microsoft Kayıt Hizmeti'nden bir sunucu lisans sertifikası alır. Bu işlem kayıt olarak adlandırılır. Bu sertifika kök sertifika sunucusunun ortak anahtarını içerir ve Kayıt Hizmeti'nin özel anahtarıyla imzalanır. Kök sertifika kümesine eklenen diğer sunucular bu sertifikayı paylaşır.

Sağlama işlemi sırasında, kümedeki ilk lisans sunucusu, alt kayıt olarak adlandırılan işlem sırasında RMS kök sertifika sunucusundan veya kümesinden bir sunucu lisans sertifikası alır. Bu sertifika lisans sunucusunun ortak anahtarını içerir ve kök sertifika sunucusu veya kümesinin özel anahtarıyla imzalanır. Lisans kümesine eklenen diğer sunucular bu sertifikayı paylaşır.

Aşağıdaki tabloda sunucu lisans sertifikaları tarafından sunuculara verilen haklar listelenmektedir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Şunları verme hakkı sağlar</th>
<th style="border:1px solid black;" >Kök sertifika sunucusuna verilen sunucu lisans sertifikası</th>
<th style="border:1px solid black;" >Lisans sunucusuna verilen sunucu lisans sertifikası</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Hak hesabı sertifikaları</td>
<td style="border:1px solid black;">Evet</td>
<td style="border:1px solid black;">Hayır</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Yayımlama lisansları</td>
<td style="border:1px solid black;">Evet</td>
<td style="border:1px solid black;">Evet</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Kullanım lisansları</td>
<td style="border:1px solid black;">Evet</td>
<td style="border:1px solid black;">Evet</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alt sunucu lisans sertifikaları</td>
<td style="border:1px solid black;">Evet</td>
<td style="border:1px solid black;">Hayır</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">İstemci lisans sertifikaları</td>
<td style="border:1px solid black;">Evet</td>
<td style="border:1px solid black;">Evet</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720184.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| RMS ayrı lisans sunucuları veya kümeleri gerektirmez, ancak kök sertifika kümesinden lisans isteği yükünü almak için ayrı lisans sunucuları ve kümeleri kullanılabilir. Yöneticiler, güvenli içerik yayımlama üzerinde doğrudan denetiminin olmasını isteyen iç kuruluşların gereksinimlerini karşılamak için lisans sunucuları kurmak da isteyebilirler. Örneğin, kök sertifika sunucusu veya kümesinin hak ilkesi şablonlarında uygulanan genel şirket ilkeleri, belirli bir bölümün gereksinim duyduğu bazı hakları belirtmeyebilir. Bu durumda, ilgili bölüm kendi hak ilkesi şablonlarını depolamak ve lisans isteklerini işlemek için ayrı bir lisans sunucusu veya kümesi dağıtabilir. |
