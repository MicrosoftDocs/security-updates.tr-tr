---
TOCTitle: Sunucu Hizmetlerinin Sertifikasını Etkinleştirmek için
Title: Sunucu Hizmetlerinin Sertifikasını Etkinleştirmek için
ms:assetid: '0ed78c85-7acb-4e3b-a594-613f8ccb5b14'
ms:contentKeyID: 18125006
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720196(v=WS.10)'
---

Sunucu Hizmetlerinin Sertifikasını Etkinleştirmek için
======================================================

Bu yordamı gerçekleştirmek için, Administrators grubunun üyesi olan bir etki alanı kullanıcı hesabıyla Yönetim Web sitesinde yerel olarak oturum açmış olmalısınız. Etkili bir güvenlik uygulaması olarak, bu yordamı uygulamak için **Farklı çalıştır**'ı kullanmayı deneyin.

Bu yordam, sadece kök kümesinde uygulanabilir.

Bu yordamda, haklarla korunan içeriği kullanırken sunucu hizmetlerini temsil eden kullanıcı hesaplarını içeren bir kullanıcı grubu oluşturduğunuz varsayılır.

Sunucu Hizmetleri Sertifikasını Etkinleştirme
---------------------------------------------

#### Sunucu Hizmetleri Sertifikasını Etkinleştirmek için

1.  Yerel Administrators grubunun üyesi olarak bilgisayarda oturum açın.

2.  Bir dosya sistemi tarayıcısı açın ve &lt;sistem sürücüsü&gt;:\\Inetpub\\wwwroot\\\_wmcs\\Certification klasörüne gidin.

3.  Hizmet hesabı sertifikaları (RAC) almak üzere sunucu hizmetlerini etkinleştirmek için, ServerCertification.asmx dosyasını sağ tıklatın ve ardından **Özellikler**'i tıklatın.

4.  **Güvenlik** sekmesinde, **Ekle**'yi tıklatın ve bu kullanıcı kategorisi ve **RMS Service Group** için oluşturduğunuz grubu ekleyin.

5.  Grupların **İzinler** listelerinde **Okuma & Yürütme** izinleri için **İzin Ver** onay kutusunu seçin ve ardından **Tamam**'ı tıklatın.

6.  Adım 1 - 4, kümedeki her sunucu için yinelenmelidir.

| ![](/security-updates/images/Cc720196.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Microsoft Exchange Server 2007 için, her körü sunucusunun Active Directory bilgisayar nesnesini ServerCertification.asmx öğesinin İsteğe Bağlı Erişim Denetim Listesi'ne (DACL) eklemelisiniz. Microsoft Office SharePoint Server 2007 için de benzer şekilde, Office SharePoint Server 2007 sunucusunun Active Directory bilgisayar nesnesini bu DACL'ye eklemelisiniz. Bu DACL'ye bir güvenlik grubu eklemeniz ve uygun bilgisayar nesnelerini de ona eklemeniz önerilir. |
