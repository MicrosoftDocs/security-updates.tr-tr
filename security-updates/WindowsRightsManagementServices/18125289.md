---
TOCTitle: Etkinleştirme Hizmetini Bulma
Title: Etkinleştirme Hizmetini Bulma
ms:assetid: 'e178d81b-b35c-4958-87ef-e077e2204b32'
ms:contentKeyID: 18125289
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747697(v=WS.10)'
---

Etkinleştirme Hizmetini Bulma
=============================

Etkinleştirme hizmeti RMS sürüm 1.0 istemcileri için kasalar ve RMS makine sertifikaları verir. RMS sürüm 1.0 ile geriye dönük uyumluluk için desteklenmektedir. RMS kök sertifika kümesi, kuruluş ağında çalışan istemci bilgisayarlardan gelen RMS makine etkinleştirme isteklerini etkinleştirme hizmetine ileten etkinleştirme proxy hizmetini sağlar.

RMS makine etkinleştirme isteğinde bulunmak için, RMS sürüm 1.0 istemcisi ilk olarak Active Directory'den etkinleştirme proxy hizmetinin bulunduğu kök sertifika sunucusunun Certification sanal dizinine ait URL'yi alır. Ardından yolu etkinleştirme proxy hizmetinin sonuna ekler.

Örneğin, kök sertifika sunucusu üzerindeki Certification sanal dizinine ait URL Active Directory'de aşağıdaki biçimde depolanır:

http://*sunucu\_adı*/\_wmcs/Certification

İstemci RMS makine etkinleştirme isteğinde bulunduğunda, etkinleştirme proxy hizmeti dosya adını URL'ye aşağıdaki gibi ekler:

http://*sunucu\_adı*/\_wmcs/Certification/Activation.asmx

Kuruluş ağının dışında çalışan istemciler, etkinleştirme hizmetini konumlandırmak için hizmet bulma amacıyla UDDI'yi kullanır. Daha fazla bilgi için, bu konuda daha önce yer alan "[Microsoft Tarafından Barındırılan Hizmetleri Yayımlama](https://technet.microsoft.com/7ee8cb4d-1b46-48be-8a4c-5ff6a458231a)" bölümüne bakın.

| ![](/security-updates/images/Cc747697.note(WS.10).gif)Not                           |
|------------------------------------------------------------------------------------------------|
| RMS sunucunuzda SSL'yi etkinleştirdiyseniz, bu URL'ler https:// bağlantı protokolünü kullanır. |
