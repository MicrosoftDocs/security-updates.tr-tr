---
TOCTitle: Hesap Sertifikası Hizmetini Bulma
Title: Hesap Sertifikası Hizmetini Bulma
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18125033
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720224(v=WS.10)'
---

Hesap Sertifikası Hizmetini Bulma
=================================

RMS Hesap Sertifikası hizmeti kullanıcılara hak hesabı sertifikaları verir. Her hak hesabı sertifikası (RAC) yalnızca belirli bir bilgisayar veya aygıt için geçerlidir ve sertifikayı isteyen kullanıcının geçerli bir makine sertifikasına sahip olmasını gerektirir.

Hesap sertifika hizmetini yalnızca kök sertifika sunucusu veya kümesi çalıştırır. Hesap sertifikası isteğinde bulunmak için, bir istemci ilk olarak hesap sertifikası hizmetinin bulunduğu kök sertifika sunucusunun Certification sanal dizinin URL'sini Active Directory'den alır. Ardından yolu hesap sertifikası hizmetinin sonuna ekler.

Örneğin, kök sertifika sunucusunun Sertifika URL'si Active Directory'de aşağıdaki biçimde depolanır:

http://*sunucu\_adı*/\_wmcs/Certification

İstemci, hak hesabı sertifikası isteğinde bulunduğunda, hesap sertifikası hizmeti dosya adını URL'ye aşağıdaki gibi ekler:

http://*sunucu\_adı*/\_wmcs/Certification/Certification.asmx

| ![](images/Cc720224.note(WS.10).gif)Not                           |
|------------------------------------------------------------------------------------------------|
| RMS sunucunuzda SSL'yi etkinleştirdiyseniz, bu URL'ler https:// bağlantı protokolünü kullanır. |
