---
TOCTitle: İptal Listelerini Dağıtma
Title: İptal Listelerini Dağıtma
ms:assetid: 'e331338b-66d4-45e4-8d3f-acccf2302ac4'
ms:contentKeyID: 18125347
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747702(v=WS.10)'
---

İptal Listelerini Dağıtma
=========================

İptali uygulamak için iptal listelerini dağıtmanız gerekir. İptal listeleri; iptal edilmiş içerik, uygulama, kullanıcı veya diğer asıl öğeleri belirtir. Hem kuruluşun iptal listelerini hem de Microsoft'tan alınan iptal listelerini dağıtabilirsiniz.

Kuruluş İptal Listelerini Dağıtma
---------------------------------

Hak ilkesi şablonunu bir iptal listesiyle kullanmak için, iptal listesini kuruluştaki istemci bilgisayarların kullanımına sunmanız gerekir. İptal listeleri oluşturma hakkında daha fazla bilgi için bu konuda daha önce geçen "İptal Uygulama" bölümüne bakın.

Bir kuruluş iptal listesini aşağıdaki adımları kullanarak dağıtabilirsiniz:

1.  İptal listesi dosyasını herkesin erişilebildiği bir Web sunucusuna kopyalayın. Kullanıcılar korumalı içeriği kuruluş dışından kullanabilecekleri için, belirtilen konuma hem ağ içinden hem de ağ dışından erişilebilmelidir.
    İptal listesi dosyasını istemci bilgisayarlara dağıtmak biraz zaman alabilir. Bu durum, kullanıcının bir iptal listesini gerektiren belge açmak istediğinde istemci bilgisayarlarda iptal listesini bulamamasına yol açabilir. İstemci bilgisayarda iptal listesi yoksa, RMS etkin uygulama bu listeyi kullanım lisansında belirtilen konumdan yükleyebilir.
    En iyisi, iptal listesini her gün otomatik olarak imzalayıp Web sitesine kopyalayan bir komut dosyası oluşturmanızdır. Bu, kullanıcıların sahip oldukları listenin eskiliğinden dolayı içeriği kullanamamalarını önlemenize yardımcı olur. Örnek komut dosyası için bu konuda daha önce geçen "İptal Listesi İmzalama Aracını Kullanma" bölümüne bakın.
2.  Hak ilkesi şablonunda kuruluş iptal listesi için sıfırdan büyük bir yenileme aralığı belirtin. Bu, iptal listesinin isteğe bağlı olmamasını sağlar. Listeyi sık sık güncelleştirmeyecekseniz (örneğin, yalnızca güvenlik ihlali gibi bir durumda güncelleştirecekseniz), yenileme koşulunu uzun bir aralık olarak belirleyebilir ve iptal listesini istemci bilgisayarlara gerektikçe komut dosyası veya ilke ayarları ile gönderilecek duruma getirebilirsiniz. Yenileme aralığı belirleme hakkında daha fazla bilgi için bu konuda daha önce geçen "İptal İlkelerini Tanımlama" bölümüne bakın. Hak ilkesi şablonları yapılandırma hakkında daha fazla bilgi için bu konuda daha sonra yer alan "Hak İlkesi Şablonlarını Oluşturma ve Değiştirme" bölümüne bakın.
3.  Hak ilkesi şablonunda iptal listesinin ulaşılabileceği bir URL belirtin.
4.  İsteğinize göre, iptal listesini Grup İlkesi veya Systems Management Server (SMS) gibi otomatik bir yöntem kullanarak istemci bilgisayarlara dağıtın.

Microsoft'un İptal Listelerini Dağıtma
--------------------------------------

Rights Management Services istemcisinin Microsoft'tan alınan bir iptal listesini kullanması için listeyi istemci bilgisayarlarda dağıtmanız gerekir. Bu konuda Microsoft'tan alınan bir iptal listesinin nasıl dağıtılacağı aşağıdaki senaryolarla açıklanmaktadır:

-   Kuruluşunuz kendi iptal listesini ve Microsoft'tan alınan iptal listesini dağıtmak istiyor:
-   Kuruluşunuz yalnızca Microsoft'tan alınan iptal listesini dağıtmak istiyor.

Microsoft bir iptal listesi yayımladığında bu dosyayı aşağıdaki konumlardan karşıdan yükleyebilirsiniz:

-   RMS sunucular iptal listesini Windows Güncelleme kullanarak karşıdan yükleyebilir.
-   Alternatif olarak, Microsoft iptal listesi RMS sunucunuz Internet'e bağlı değilse Microsoft Yükleme Merkezi konumundan da karşıdan yüklenebilir.

İptal listesi paketini bir RMS sunucusuna karşıdan yüklerseniz, paket %systemdrive%\\Program Files\\Windows Rights Management Services Revocation List klasörüne kaydedilir. İptal listesi paketini başka türde bir bilgisayara karşıdan yüklüyorsanız, yükleme konumunu seçebilirsiniz. Paket, istemci lisans deposundaki tüm istemci iptal listelerini yüklemek üzere çalıştırabileceğiniz CRL\_Update.exe yürütülebilir dosyasını ve bir Web sitesine veya ortak paylaşılan klasöre kopyalayabileceğiniz bir iptal listesi dosyası olan Msrl.xml dosyasını içerir.

**Hem kuruluşunuzun iptal listesini hem de Microsoft'tan alınan iptal listesini dağıtmak için**
1.  Kuruluşunuzun iptal listesini dağıtmak için bu konuda daha önce geçen "[İptal Listelerini Dağıtma](https://technet.microsoft.com/e331338b-66d4-45e4-8d3f-acccf2302ac4)" bölümündeki yönergeleri izleyin.

2.  Microsoft iptal listesi paketini karşıdan yükleyin ve Grup İlkesi veya Systems Management Server (SMS) gibi bir yöntem kullanarak kuruluşunuzdaki tüm istemci bilgisayarlara dağıtın. Bunun yerine, Microsoft iptal listesindeki girişleri kuruluş iptal listesine kopyalayıp, yalnızca bu kuruluş iptal listesini dağıtabilirsiniz.

| ![](/security-updates/images/Cc747702.Caution(WS.10).gif)Dikkat                                                                                                                                                                                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft, RMS'nin yayınladığı tüm sertifikaların ve lisansların güven zincirinde bir asıl öğedir. Bu nedenle, kuruluş iptal listesini gerektiren hak ilkesi şablonuna göre kullanım lisansı alınan tüm bağlantı isteklerinde Microsoft'un yayınladığı iptal listesi etkili olur. Ayrıca, Microsoft iptal listesi istemci bilgisayara kaydedilir. |

**Yalnızca Microsoft iptal listesi dağıtmak için**
1.  Microsoft iptal listesi paketini karşıdan yükleyin.

2.  İptali gerektirmek için varolan hak ilkesi şablonlarını değiştirin; hak ilkesi şablonu yoksa, iptal gerektiren bir hak ilkesi şablonu oluşturun. İptal koşulunu belirtirken Microsoft ortak anahtarını kullanın.

3.  Yenileme aralığını 50.000 gibi büyük bir sayı yapın. Bu büyük sayı, Microsoft'un yayınladığı iptal listesinin geçerliliğinin hiç sona ermemesini sağlar. Bu nedenle, dağıttığınız kullanım lisansları, Microsoft iptal listesi kullanılabilir olmadığında yeni sürüm iptal listesi gerektirmez.

4.  İptal listesi dosyasını herkesin erişilebildiği bir Web sunucusuna kopyalayın. Kullanıcılar korumalı içeriği kuruluş dışından kullanabilecekleri için, belirtilen konuma hem ağ içinden hem de ağ dışından erişilebilmelidir.

5.  İptal listesi dosyasının istemci bilgisayarlara dağıtımı zaman alabileceği için iptal listesini kullanıma sunmanız gerekir. Bu yüzden, kullanıcı iptal gerektiren bir yayımlama lisansına sahip bir belgeyi açmak istediğinde iptal listesinin bilgisayarda yerel olarak bulunmama olasılığı vardır. İstemci bilgisayarda iptal listesi yoksa, RMS etkin uygulama belirtilen konumdan iptal listesini yükleyebilir.

6.  Hak ilkesi şablonunda iptal listesinin ulaşılabileceği bir URL belirtin. Hak ilkesi şablonları yapılandırma hakkında daha fazla bilgi için bu konuda daha sonra yer alan "[Hak İlkesi Şablonlarını Oluşturma ve Değiştirme](https://technet.microsoft.com/6014176f-ef71-4d29-b3e3-da129c18563d)" bölümüne bakın.

7.  İsteğinize göre, iptal listesini Grup İlkesi veya SMS gibi bir yöntem kullanarak istemci bilgisayarlara dağıtın. Böylece kullanıcılar ağa bağlı olmasalar bile, iptal listeleri gerektiren RMS korumalı içeriği açabilirler.
