---
TOCTitle: 'RMS Yönetim Paketi''ni Almak ve Kullanmak için'
Title: 'RMS Yönetim Paketi''ni Almak ve Kullanmak için'
ms:assetid: 'd9a73ef0-2f81-48c2-97cc-deb7bf477389'
ms:contentKeyID: 18125283
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747688(v=WS.10)'
---

RMS Yönetim Paketi'ni Almak ve Kullanmak için
=============================================

RMS Yönetim Paketi'ni Alma ve Kullanma
--------------------------------------

#### RMS Yönetim Paketi'ni Almak ve Kullanmak için

1.  RMS Management Pack'i (RMS\_MOMPack.akm) %ProgramFiles%\\Windows Rights Management Services\\Tools klasöründen Microsoft Operations Manager (MOM) sunucusuna kopyalayın.

2.  MOM Yönetici konsolunu açın ve sonra aşağıdaki adımları izleyerek RMS Yönetim Paketi'ni alın.

    1.  MOM Yönetici konsolunun konsol ağacında, **Kurallar** öğesini genişletin ve sonra **Kural Gruplarını İşliyor** öğesini sağ tıklatın.
    2.  Kısayol menüsünde **Yönetim Paketi Al**'ı tıklatın. **Yönetim Paketi Al** iletişim kutusu ekranda görüntülenir.
    3.  **Gözat**'ı tıklatın ve sonra RMS\_MOMPack.akm'yi seçin.

3.  Birleştirme ve değiştirme seçeneklerini belirleyin. Birleştirme ve değiştirme seçenekleri hakkında daha fazla bilgi için Microsoft Web sitesindeki (http://www.microsoft.com/) "Yönetim Paketlerini Verme ve Alma" konusuna bakın.

    **Değiştir**'i tıklatın. Değiştir seçeneği, alınan yönetim paketinin varolan işleme kuralı gruplarının üzerine yazmaya neden olur; hiçbir kullanıcı açıklaması korunmaz. Bu yönetim paketini varolan bir yönetim paketiyle birleştirmek istiyorsanız, bunu bir sınama ortamında yapmalı ve sonra yönetim paketini üretim ortamında dağıtırken **Değiştir** seçeneğini kullanmalısınız.

4.  Yönetim paketini almak için **Al**'ı tıklatın.

5.  **MOM Yöneticisi** konsolunda **Yapılandırma** öğesini seçin, sonra **Aracı Yöneticileri** klasörünü tıklatın.

6.  RMS Yönetim Paketi'ni aldığınız sunucunun adını sağ tıklatın ve sonra **Yönetilen Bilgisayarları Şimdi Tara**'yı seçin.
