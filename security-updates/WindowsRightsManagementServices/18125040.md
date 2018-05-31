---
TOCTitle: Hak İlkesi Şablonlarında İptal İşlemi
Title: Hak İlkesi Şablonlarında İptal İşlemi
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18125040
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720226(v=WS.10)'
---

Hak İlkesi Şablonlarında İptal İşlemi
=====================================

İptal koşulları, hak ilkesi şablonlarında belirtilir. Bir hak ilkesi şablonuna yazdığınız iptal koşulu değerleri, şablona karşılık verilen yayımlama lisansındaki bir XrML REFRESH etiketine kaydedilir. Sunucunun verdiği kullanım lisansı REFRESH etiketini de içerir.

Aşağıda REFRESH etiketindeki parametrelerin listesi bulunmaktadır.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parametre</th>
<th style="border:1px solid black;" >Açıklama</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">İptal listesi kimliği.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">İptal listesinin alınabileceği URL veya UNC yolu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">İptal listesi yayıncısının ortak anahtarı. Bu ortak anahtar iptal listesini imzalamada kullanılan özel anahtara karşılık gelir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">Yenileme listesi ömrünün, gün olarak üst sınırı. Önbellekteki iptal listesi INTERVALTIME değeri tarafından izin verilenden daha eskiyse, RMS istemcisi en son iptal listesini ADDRESS parametresinde listelenen URL'den alır. Bu, güncel bir iptal listesinin kullanılmasını sağlar.</td>
</tr>
</tbody>
</table>
  
Hak ilkesi şablonları oluşturma konusunda daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Hak İlkesi Şablonları Oluşturma ve Değiştirme" konusuna bakın.
