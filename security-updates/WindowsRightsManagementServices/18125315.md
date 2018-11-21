---
TOCTitle: Pilot RMS Dağıtımından Üretim Dağıtımına Geçiş
Title: Pilot RMS Dağıtımından Üretim Dağıtımına Geçiş
ms:assetid: 'ea151946-22fb-4cba-a3ef-fd7a4bf0d292'
ms:contentKeyID: 18125315
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747789(v=WS.10)'
---

Pilot RMS Dağıtımından Üretim Dağıtımına Geçiş
==============================================

Birçok kuruluş RMS teknolojisini kuruluş genelinde uygulamadan önce RMS'yi bir pilot dağıtımda sınamayı seçer. Pilot programda genellikle sınırlı sayıda kullanıcı vardır ve sunucu, bir BT grubunun yönetiminde olan bir veri merkezinin parçası olmak yerine yerel olarak atanmış bir yöneticinin gözetiminde olur. Pilot dağıtım tamamlandıktan sonra kuruluş, RMS'yi tüm istemciler için veri merkezinde uyguladığında, daha yüksek olası kullanıcı sayısını desteklemek için yeni RMS sunucuları dağıtılır.

Ancak, RMS korumalı içerik bunu oluşturmak için kullanılan RMS sunucusuna bağlıdır ve bu nedenle, bir sunucu kaldırıldığında veya değiştirildiğinde, pilot RMS sunucuları kullanılarak şifrelenen içeriğin üretim RMS sunucuları tarafından şifresinin çözülebilmesi ve lisanslanabilmesi için bazı adımlar atılmalıdır.

RMS'yi pilot program olarak dağıttıysanız ve RMS sunucusunu kuruluşunuzun üretim ortamına taşımak ve aynı zamanda pilot RMS sunucusu kullanılarak korunan içeriğin bütünlüğünü korumak istiyorsanız, sorunsuz geçiş ve gerektiğinde verileri kurtarmak için pilot programa geri dönebilme olanağı sağlayan bir geçiş planı oluşturmalısınız.

Aşağıdaki adımlar geçiş planınızda bulunması gereken bazı öğelere örnek olarak verilmiştir; dağıtımınızın ek gereksinimleri olabilir.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Sunucu</th>
<th style="border:1px solid black;" >Adım</th>
<th style="border:1px solid black;" >Notlar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Pilot</td>
<td style="border:1px solid black;">RMS yapılandırma veritabanını yedekleyin.</td>
<td style="border:1px solid black;">Böylece, gerekirse pilot sunucuyu geri yükleyebilirsiniz.
Yapılandırma veritabanı RMS özel anahtarını içerir.
Özel anahtar parolasını bildiğinizden emin olun.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pilot</td>
<td style="border:1px solid black;">RMS özel anahtarını korumak için bir Donanım Güvenlik Modülü (HSM) kullandıysanız, HSM yapılandırmasını ilgili üreticinin yönergelerine uygun olarak yedekleyin.</td>
<td style="border:1px solid black;">HSM yeni sunucuda geri yüklenir.
Kullanılan HSM'yi yüklemek ve yapılandırmak için gerekli tüm bileşenlere sahip olduğunuzdan emin olun.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Pilot</td>
<td style="border:1px solid black;">Güvenilen Yayımlama Etki Alanı dosyasını verin.</td>
<td style="border:1px solid black;">Bu, başka bir RMS sunucusunun bu sunucu tarafından oluşturulan yayımlama lisanslarının şifresini çözmesine ve korunan içerik için kullanım lisansları vermesine olanak tanır.
Güvenilen yayımlama etki alanı sunucu lisans sertifikasını, RMS özel anahtarını ve bu sunucunun oluşturduğu tüm hak ilkesi şablonlarını içerir.
Güvenilen yayımlama etki alanı dosyası, dosyayı oluşturduğunuzda belirttiğiniz sağlam parolayla şifrelenen bir XML dosyasıdır. Güvenilen yayımlama etki alanı dosyasını almak için de bu parolaya sahip olmanız gerekir.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Pilot</td>
<td style="border:1px solid black;">Güvenilen Kullanıcı Etki Alanını verin.</td>
<td style="border:1px solid black;">Bu, hak hesabı sertifikaları (RAC) pilot RMS sunucusu tarafından verilen kullanıcılara başka bir RMS sunucusunun kullanım lisansları vermesine olanak tanır.
Güvenilen kullanıcı etki alanı, bu sunucunun sunucu lisans sertifikasını başka bir RMS sunucusuna alarak oluşturulur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">Yeni sunucuyu kök sertifika sunucusu olarak hazırlayın.</td>
<td style="border:1px solid black;">Veritabanı sunucusuna erişebildiğinden ve IIS ile Message Queuing'in yüklü olduğundan emin olun.
Olabiliyorsa, bu sunucu için aynı sunucu adını kullanın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">HSM kullanıyorsanız HSM'yi yükleyin ve pilot sunucuda oluşturduğunuz yedeği kullanarak yapılandırmasını geri yükleyin.</td>
<td style="border:1px solid black;">RMS özel anahtarının şifresini çözmek için gereken kimlik bilgilerini oluşturur.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">RMS'yi yükleyin.</td>
<td style="border:1px solid black;">RMS önkoşul oluşturan tüm hizmetlerin düzgün olarak yüklendiğini ve yapılandırıldığını doğrular.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">Yeni bir özel anahtar kullanarak RMS'yi sağlayın. Çevrimiçi kayıt kullanıyorsanız, sağlama işlemi sırasında Microsoft Kayıt Hizmeti'ne bağlanmak için Internet kullanılarak sunucunuz kaydedilir. Bu sunucuda Internet bağlantısı kuramıyorsanız, çevrimdışı kaydı kullanmanız gerekir.</td>
<td style="border:1px solid black;">Bu sunucunun adı pilot sunucu adından farklıysa, küme URL ayarını pilot sunucuyla aynı URL olacak şekilde değiştirebilirsiniz.
Bunu yapmazsanız, önceden varolan içeriğe sahip kullanıcıların kullanım lisansları almasına olanak tanımak için önceki küme URL'sinden yeni küme URL'sine yönelik bir URL yönlendirmesi oluşturmanız gerekir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">Çevrimdışı kaydı kullanıyorsanız, yeni RMS sunucusu için el ile kayıt işlemini tamamlayın. Daha fazla bilgi için bu belge grubundaki &quot;RMS Sunucusunu Çalıştırma&quot; bölümünde bulunan &quot;Kök Sertifika Sunucusunu El İle Kaydettirmek İçin&quot; konusuna bakın.</td>
<td style="border:1px solid black;">RMS sunucusu kaydedilene kadar kullanılamaz.
Ayrıca, sunucu kaydedilene kadar RMS yönetim sayfalarına erişilemez.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">3. adımda verdiğiniz güvenilen yayımlama etki alanı dosyasını alın.</td>
<td style="border:1px solid black;">Dosyayı başarıyla almak için RMS hizmet hesabının, dosyanın depolandığı konumda okuma izni olması gerekir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">Alınan her şablonu güvenilen yayımlama etki alanıyla yeniden imzalayın.</td>
<td style="border:1px solid black;">Şablonlar sunucu özel anahtarıyla imzalanır. Bu şablonun yeni bir özel anahtarı olduğundan, şablonların geçerli olması için yeniden imzalanması gerekir. Daha fazla bilgi için bu belge grubundaki &quot;RMS Sunucusunu Çalıştırma&quot; bölümünde bulunan &quot;Hak İlkesi Şablonunu Yeniden İmzalamak İçin&quot; konusuna bakın.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">Şablonları pilot dağıtımda yer alan istemci bilgisayarlara yeniden dağıtın.</td>
<td style="border:1px solid black;">Eski şablonların kaldırılması ve bu sunucu tarafından imzalanan şablonlarla değiştirilmesi gerekir.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Üretim</td>
<td style="border:1px solid black;">4. adımda verdiğiniz güvenilen kullanıcı etki alanı dosyasını alın.</td>
<td style="border:1px solid black;">Eski istemci lisans sertifikalarını ve RAC'leri kullanılmak üzere etkinleştirir.
Bu geçiş işleminde kullanıcı hesapları ormanlar arasında taşınıyorsa, hesapların eşleşen SMTP proxy'lerine sahip olması gerekir.</td>
</tr>
</tbody>
</table>
 

Üretim sunucusunu kurmayı tamamladığınızda, pilot kullanıcıların posta oluşturmaya devam edebildiğini ve önceden korunan postaları okuyabildiğini doğrulayın. Daha sonra, kuruluşunuzdaki kullanıcı sayısını desteklemek için gereksinim duyduğunuz sayıda RMS sunucusunu kümeye ekleyebilirsiniz.
