---
TOCTitle: Kök Sertifika Sunucusunu Yüklemeye Hazırlanma
Title: Kök Sertifika Sunucusunu Yüklemeye Hazırlanma
ms:assetid: 'ed51605e-8b17-4155-8d83-f6777f499b7b'
ms:contentKeyID: 18125327
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747726(v=WS.10)'
---

Kök Sertifika Sunucusunu Yüklemeye Hazırlanma
=============================================

Sınama yüklemesi örneğinde, yalnızca tek bir kök sertifika sunucusu vardır. İsterseniz, kök sertifika kümesinin bir parçası veya ayrı bir lisans sunucusu kümesi olarak ek sunucular kurabilirsiniz. Bu tür sunucuların tümü için altyapı kurulumu aynıdır, bu yüzden sunucuların her birinde bu konuda sağlanan yordamı uygulamanız gerekir.

Etki alanı denetleyicisi yüklendikten, veritabanı sunucuları kurulduktan (önceki bölümde anlatıldığı gibi) ve aşağıdaki tabloda yer alan adımlar tamamlandıktan sonra, RMS'yi yüklemeye hazır olursunuz.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Altyapı Bileşeni</th>
<th style="border:1px solid black;" >Sunucuyu RMS Yüklemesine Hazırlamak için</th>
<th style="border:1px solid black;" >Üretim Ortamında Dağıtım Notları</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">İşletim sistemi</td>
<td style="border:1px solid black;">RMS donanım gereksinimlerini karşılayan, ancak henüz ağa bağlı olmayan bir bilgisayara, Windows Server 2003 işletim sistemini yükleyin ve bölüm için NTFS dosya sistemini kullanın.</td>
<td style="border:1px solid black;">Her zaman en son hizmet paketini ve düzeltme eklerini yüklemeniz özellikle önerilir. NTFS olarak biçimlendirilmiş bölümleri kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet bağlantısı
(isteğe bağlı)</td>
<td style="border:1px solid black;">Internet bağlantısı sağlayan, ancak üretim ortamından ayrılmış bir ağa yönelik Ethernet bağlantısı oluşturun. Sağlama işleminde RMS sunucusunu kaydettirmek için çevrimiçi kayıt işlemini kullanacaksanız, sunucunuzun Internet bağlantısı olması gerekir.</td>
<td style="border:1px solid black;">Çevrimiçi kayıt kullanıyorsanız, Internet bağlantısında uygun güvenlik duvarının olduğundan emin olun.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IP adresi</td>
<td style="border:1px solid black;">Bu bilgisayara statik bir IP adresi atayın.</td>
<td style="border:1px solid black;">Sunucular için her zaman statik IP adresleri kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bu bilgisayarı etki alanına ekleyin.</td>
<td style="border:1px solid black;">Bilgisayara yerel yönetici olarak oturum açın. <strong>Başlat</strong>'ı tıklatın, <strong>Bilgisayarım</strong>'ı sağ tıklatın, <strong>Özellikler</strong>'i tıklatın, <strong>Bilgisayar Adı</strong> sekmesini tıklatın ve sonra <strong>Değiştir</strong>'i tıklatın.</td>
<td style="border:1px solid black;">Tüm sunucular için aynı etki alanını kullanın.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;">Bilgisayar adını olduğu gibi bırakın, <strong>Etki Alanı</strong>'nı tıklatın ve sonra etki alanı adını yazın, örneğin Contoso.com yazın ve sonra <strong>Tamam</strong>'ı tıklatın. Etki alanına katılmanızı sağlayan kullanıcı kimlik bilgilerini girin, <strong>Tamam</strong>'ı tıklatın ve sonra istendiğinde bilgisayarı yeniden başlatın. Bilgisayar yeniden başlatılıp oturum açma kimlik bilgileri istendiğinde, uygun etki alanını, kullanıcı adını ve parolayı sağlayın.</td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kullanıcı ve oturum açma</td>
<td style="border:1px solid black;"><strong>Bilgisayarım</strong>'ı tıklatın, <strong>Yönet</strong>'i tıklatın, <strong>Yerel Kullanıcılar ve Gruplar</strong>'ı genişletin, <strong>Gruplar</strong>'ı tıklatın ve sonra <strong>Administrators</strong>'ı çift tıklatın.
<strong>Ekle</strong>'yi tıklatın, eklenecek kullanıcı hesabının adını (Demir@contoso.com gibi) belirtin ve sonra <strong>Tamam</strong>'ı tıklatın. Kullanıcı hesabına Yönetici ayrıcalıkları verin. Kimlik bilgileri istendiğinde, ilgili kimlik bilgilerini girin, örneğin Contoso\Administrator.
Bilgisayara Yönetici ayrıcalıklarına sahip bir etki alanı kullanıcısı olarak oturum açın.</td>
<td style="border:1px solid black;">Bu bilgisayara bileşen eklemek için yönetici hakları gereklidir. Bazı yükleme adımları yerel yönetici hesabı kullanılarak tamamlanamaz. Bu sunucuda, yönetici olan en az bir etki alanı kullanıcısına sahip olmalısınız. Ayrıca, SQL Server yeni veritabanı oluşturmak için Sistem Yöneticisi hakları gerektirir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internet bağlantısı
(isteğe bağlı)</td>
<td style="border:1px solid black;">Internet erişimini doğrulamak için bir Internet tarayıcısı kullanarak http://uddi.microsoft.com/ adresine gidin. Windows Server 2003 çalıştıran bilgisayarlarda, etki alanı denetleyicisini eklemek için Lmhosts ve Hosts dosyalarının değiştirilmesi gerekebilir.</td>
<td style="border:1px solid black;">Internet erişimini doğrulamak için http://uddi.microsoft.com adresine gidin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Etkinleştirmesi</td>
<td style="border:1px solid black;">Internet bağlantısı kullanarak Windows'u Microsoft ile etkinleştirmek için Etkinleştirme Sihirbazı'nı kullanabilir veya Windows'u telefonla etkinleştirebilirsiniz. Windows Server 2003 ürün etkinleştirmesi hakkında daha fazla bilgi için bkz. Windows Server 2003 Yardım ve Destek Merkezi.</td>
<td style="border:1px solid black;">Windows Server 2003 yüklemeden sonra 14 gün içinde etkinleştirilmelidir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Yazılım güncelleştirmeleri</td>
<td style="border:1px solid black;">Bu bilgisayara yüklü yazılımlar için en son yazılım güncelleştirmelerini yüklediğinizden emin olun.</td>
<td style="border:1px solid black;">En son yazılım güncelleştirmelerini yükleyin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet Explorer'ı Yapılandırma</td>
<td style="border:1px solid black;">RMS yönetim için Web arabirimi kullanır. Bazı varsayılan güvenlik ayarları sayfaların düzgün işlenmesini önleyebilir. RMS Yönetimi Web sitesindeki bazı sayfalarda bazı yapılandırma seçenekleri için açılır pencereler kullanılır.</td>
<td style="border:1px solid black;"> </td>
</tr>
</tbody>
</table>
  
Her iki sunucuda da yukarıdaki adımları tamamladığınızda, RMS'yi sunuculara yüklemeye ve sağlamaya hazır olursunuz.
