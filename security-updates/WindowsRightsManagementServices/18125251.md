---
TOCTitle: Passport Tabanlı Hak Hesabı Sertifikalarına Güvenmek için
Title: Passport Tabanlı Hak Hesabı Sertifikalarına Güvenmek için
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18125251
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747655(v=WS.10)'
---

Passport Tabanlı Hak Hesabı Sertifikalarına Güvenmek için
=========================================================

Microsoft, kullanıcı için hak hesabı sertifikası oluşturmak üzere Microsoft .NET Passport kimlik bilgilerini kullanan bir hesap sertifikası hizmeti sağlar. Bu hizmet için hak hesabı sertifikaları olan kullanıcıların kullanım lisanslarını RMS kümenizden edinebilmelerini isterseniz, Microsoft'un hesap sertifikası hizmetinden kullanıcı kimlik bilgilerini kabul eden güvenilen bir kullanıcı etki alanı kurmalısınız.

Bu özelliği kullanmak için, Internet Information Services'ı, RMS lisans hizmetine anonim erişime izin verecek biçimde yapılandırmalısınız. Lisans hizmeti varsayılan olarak Tümleşik Windows kimlik doğrulaması kullanacak biçimde yapılandırıldığı için, bu adım dış kullanıcılar açısından önemlidir. Anonim erişim ayarlanmazsa, Passport tabanlı Hak Hesabı Sertifikaları (RAC) olan dış kullanıcılar lisanslarını edinemez.

Passport Tabanlı Hak Hesabı Sertifikalarına Güvenme
---------------------------------------------------

#### RMS lisans hizmetine anonim erişimi etkinleştirmek için

1.  **Internet Information Services (IIS) Yöneticisi** ek bileşenini açın ve RMS'yi barındıran sunucuyu genişletin.

2.  Konsol ağacında, **Web siteleri** öğesini ve sonra da RMS'yi yapılandırmış olduğunuz Web sitesini genişletin. Bu, varsayılan olarak **Varsayılan Web sitesi** öğesidir.

3.  Konsol ağacında, **\_wmcs** Web sitesini genişletin ve **licensing** sanal dizinini seçin.

4.  **Licensing** sanal dizinini sağ tıklatın ve **Özellikler**'i seçin.

5.  **Lisans Özellikleri** iletişim kutusunda, **Dizin Güvenliği** sekmesini tıklatın.

6.  **Kimlik doğrulaması ve erişim denetimi** alanında, **Düzen**'i tıklatın.

7.  **Anonim Erişime İzin Ver** onay kutusunu seçin.

#### Passport Tabanlı Hak Hesabı Sertifikalarına Güvenmek için

1.  **Genel Yönetim** sayfasını açın ve sonra hak hesabı sertifikasını dışlamak istediğiniz Web sitesinin yanındaki **RMS'yi bu Web sitesinde yönet**'i tıklatın.

2.  **Yönetim bağlantıları** alanında, **Güven ilkeleri**'ni tıklatın.

3.  **Güvenilen kullanıcı etki alanları** alanında, **Passport RAC'lerine güven**'i tıklatın. **Güvenilen kullanıcı etki alanı** listesinde Microsoft RM Sertifika Hizmeti görüntülenir.

4.  İsteğe bağlı olarak, kullanıcıları e-posta adreslerine göre dışlayabilirsiniz. Bunu yapmak için, **Dışlanan kimlikler**'i tıklatın ve sonra güvenmediğiniz kullanıcının e-posta adresini yazın.
