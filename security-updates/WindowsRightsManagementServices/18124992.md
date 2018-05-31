---
TOCTitle: 'RMS''nin Uzaktan Yönetimini Etkinleştirmek için'
Title: 'RMS''nin Uzaktan Yönetimini Etkinleştirmek için'
ms:assetid: '00f17054-5f5d-47e2-89c1-7a593b930bb3'
ms:contentKeyID: 18124992
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720181(v=WS.10)'
---

RMS'nin Uzaktan Yönetimini Etkinleştirmek için
==============================================

RMS'nin uzaktan yönetimi için Internet Explorer 6.0'ın ya da daha üst sürümünün bilgisayarda yüklü olması gerekir.

RMS'nin Uzaktan Yönetimini Etkinleştirme
----------------------------------------

#### RMS'nin Uzaktan Yönetimini Etkinleştirmek için

1.  Uzaktan yönetebilmeyi istediğiniz sunucuya oturum açın.

2.  **Yönetimsel Araçlar**'dan, **Internet Information Services (IIS) Yöneticisi** ek bileşenini açın.

3.  RMS'yi hazırladığınız Web sitesini temsil eden öğeyi genişletin.

4.  **\_wmcs** klasörünü sağ tıklatın ve **Özellikler**'i tıklatın. **Dizin Güvenliği** sekmesinde, **Güvenli iletişim** altında, **Düzenle**'yi tıklatın, **Güvenli kanal kullanılmasını iste**'yi ve sonra **Tamam**'ı tıklatın. Bu, Güvenli Yuva Katmanı (SSL) korumasını RMS Web hizmetlerine uygular. IIS'yi kullanarak Web sitelerini yönetme hakkında daha fazla bilgi için, IIS Yardımı'na başvurun.

    | ![](/security-updates/images/Cc720181.Important(WS.10).gif)Önemli                                                                                                                                                                                                               |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Daha fazla güvenlik sağlamak ve RMS yönetimi Web sayfalarına uzaktan HTTP erişimini etkinleştirmek için, RMS Web hizmetlerini SSL ile güvenli hale getirebilirsiniz. RMS Web hizmetleri için SSL'yi etkinleştirmek istiyorsanız geçerli bir SSL Web sunucusu sertifikası alın ve yükleyin. |

5.  **Admin** klasörünü sağ tıklatın ve sonra **Özellikler**'i tıklatın. **Dizin Güvenliği** sekmesinde, **IP adresi ve etki alanı adı sınırlamaları** altında, **Düzenle**'yi tıklatın ve sonra **IP adresi erişimi sınırlamaları** altında, tüm bilgisayarların bu Web sitesine bağlantı istemesini sağlamak için **Erişim verildi**'yi tıklatın.
