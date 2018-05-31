---
TOCTitle: 'Adım 4: Sunucuyu Eşitleme'
Title: 'Adım 4: Sunucuyu Eşitleme'
ms:assetid: 'a5514e46-a50b-46a6-9e5b-33c87c5b7cef'
ms:contentKeyID: 18155292
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc708523(v=WS.10)'
---

Adım 4: Sunucuyu Eşitleme
=========================

Ağ bağlantısını yapılandırdıktan sonra güncelleştirmeleri alabilirsiniz. Varsayılan olarak WSUS, tüm Microsoft ürünleri için Kritik ve Güvenlik Güncelleştirmeleri'ni karşıdan yüklemek üzere yapılandırılmıştır. Güncelleştirmeleri almak için WSUS sunucusunu *eşitlemelisiniz*.

Eşitleme, WSUS sunucusunun Microsoft Update sitesiyle iletişim kurmasını içerir. İletişim kurulduktan sonra WSUS, son eşitlemeden sonra kullanıma sunulan yeni güncelleştirmeler olup olmadığını belirler. WSUS sunucusunu ilk kez eşitlediğinizden tüm güncelleştirmeler kullanılabilir durumdadır ve yükleme için onayınıza hazırdır.

| ![](/security-updates/images/Cc708523.note(WS.10).gif)Not                                                                                                                                                                                                                       |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Bu inceleme, varsayılan ayarları kullanarak eşitlemeyi açıklar, ancak WSUS, eşitleme sırasında bant genişliğini en aza indirmenizi sağlayan seçenekler içerir. Daha fazla bilgi için “Microsoft Server Windows Update Services'ı Dağıtma” teknik incelemesine bakın (Belge İngilizce'dir). |

**WSUS sunucunuzu eşitlemek için**
1.  WSUS konsolu araç çubuğunda **Seçenekler**'i, sonra da **Eşitleme Seçenekleri**'ni tıklatın.

2.  **Görevler**'in altında **Şimdi eşitle**'yi tıklatın.

Eşitleme tamamlandıktan sonra güncelleştirmelerin listesini görmek için WSUS konsolu araç çubuğunda **Güncelleştirmeler**'i tıklatın.
