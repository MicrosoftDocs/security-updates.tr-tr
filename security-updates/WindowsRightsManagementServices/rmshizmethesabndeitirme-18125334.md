---
TOCTitle: RMS Hizmet Hesabını Değiştirme
Title: RMS Hizmet Hesabını Değiştirme
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18125334
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747736(v=WS.10)'
---

RMS Hizmet Hesabını Değiştirme
==============================

Yükleme sırasında, RMS yerel bilgisayarda RMS Service Group'u oluşturur ve ona RMS'nin çalışması için gereken kaynakların ilgili izinleri verir. RMS'yi bir sunucuda sağladığınızda, RMS hizmetini bir etki alanı hesabını kullanarak tanımlarsınız. RMS hizmet hesabı, RMS'yi yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. RMS Service Group üyesi haline getirilen bu hesaba, bu grupla ilişkili izinler verilir. RMS, rutin işlemler sırasında RMS hizmet hesabının altında çalışır.

İstediğiniz zaman RMS hizmet hesabını değiştirebilirsiniz. RMS hizmet hesabını değiştirdiğinizde, önceden belirtilen hesap otomatik olarak RMS Service Group'tan çıkarılır ve yeni hesap bu grubun bir üyesi haline getirilir.

| ![](/security-updates/images/Cc747736.Important(WS.10).gif)Önemli                                                                                                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Güvenlik nedeniyle RMS hizmet hesabı olarak kullanmak için özel bir kullanıcı hesabı oluşturmanız, bu hesabı yalnızca RMS hizmet hesabı olarak kullanmanız ve başka hiçbir amaç için kullanmamanız önerilir. Ayrıca, bu hesaba herhangi bir ek izin vermemelisiniz. |

| ![](/security-updates/images/Cc747736.note(WS.10).gif)Not                                       |
|------------------------------------------------------------------------------------------------------------|
| RMS hizmet hesabı, Service Pack 1 kurulu RMS yüklemek için kullandığınız etki alanı hesabıyla aynı olamaz. |
