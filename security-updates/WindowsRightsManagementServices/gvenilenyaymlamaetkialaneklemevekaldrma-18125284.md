---
TOCTitle: Güvenilen Yayımlama Etki Alanı Ekleme ve Kaldırma
Title: Güvenilen Yayımlama Etki Alanı Ekleme ve Kaldırma
ms:assetid: 'd87b502d-5497-4ccd-badf-f6807d587cee'
ms:contentKeyID: 18125284
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747687(v=WS.10)'
---

Güvenilen Yayımlama Etki Alanı Ekleme ve Kaldırma
=================================================

RMS sunucusu varsayılan olarak yalnızca kendisinin veya kümesindeki başka bir sunucunun verdiği yayımlama lisanslarına karşı kullanım lisansları verebilir. Kuruluşunuzdaki, örneğin başka bir ormandaki bir alt kuruluştaki, ya da farklı başka bir kuruluştaki diğer bir kök sertifika sunucusunu kullanarak yayımladığınız bir içerik bulunuyorsa ve RMS sunucunuzda güvenilir yayımlama etki alanı yapılandırırsanız, RMS sunucunuz kullanıcılara bu içerikle ilgili kullanım lisansları verebilir. Güvenilir yayımlama etki alanı ekleyerek diğer sunucunun sunucu lisans sertifikasını alır ve RMS sunucunuz ile diğer kök sertifika sunucusu arasında bir güven ilişkisi oluşturursunuz. RMS sunucunuz için sınırsız olarak istediğiniz kadar güvenilir yayımlama etki alanı yapılandırabilirsiniz.

Herhangi bir anda, güvenilen yayımlama etki alanlarına ait sertifika listesinden sertifikasını kaldırarak eklediğiniz güvenilen etki alanını kaldırabilirsiniz.

Güvenilen bir yayımlama etki alanı eklemek için, sunucu lisans sertifikasını, özel anahtarı (özel anahtar bir donanım güvenlik modülünde değil de yazılımda depolanıyorsa) ve eklemek istediğiniz RMS sunucusu veya kümesinin tüm hak ilkesi şablonlarını almalısınız. Yöneticinin bu öğeleri, öncelikle güvenilecek sunucu veya kümeden parola korumalı bir dosyaya vermesi ve ardından şifresini çözmek için gerekli parolayı belirtmesi gerekir. Yöneticinin bu dosyayı bir paylaşım klasörüne yerleştirmesi ve parolayı size bildirmesi gerekir. Ardından dosya konumunu ve parolayı belirterek dosyayı alabilirsiniz. Dosyayı kaydetmek için **Yönetici** uygulama havuzunu çalıştıran hesabın, paylaşım klasörü için gerekli izinlere sahip olması gerekir.

Güvenilen yayımlama etki alanının nasıl oluşturulacağı hakkında adım adım yönergeler için, bu konuda daha sonra yer alan "[Güvenilen Yayımlama Etki Alanı Eklemek için](https://technet.microsoft.com/731416d8-ddf4-4d4a-9f1a-bbd1ea48fe3c)" bölümüne bakın.

Özel anahtar bir donanım güvenlik modülünde depolanıyorsa, donanım güvenlik modülü belgelerindeki yönergeleri izleyerek özel anahtarı güvenilen sunucudaki donanım güvenlik modülüne aktarmanız gerekir. Her sunucuda bulunan donanım güvenlik modülünün türüne ve donanım güvenlik modülü aygıtlarının yapılandırmasına bağlı olarak, özel anahtarı bir donanım güvenlik modülünden diğerine aktaramayabilirsiniz. Özel anahtarı, hedef donanım güvenlik modülünde bulunan verileri kaybetmeden aktarıp aktaramayacağınızı belirlemek için donanım güvenlik modülü belgelerini gözden geçirin. Özel anahtarı başarıyla aktaramazsanız, iki sunucu arasında güvenilen bir yayımlama etki alanı oluşturamazsınız.

| ![](images/Cc747687.note(WS.10).gif)Not                                                                                                                                                                                                                                                                                 |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS özel anahtarınızı korumak için bir donanım güvenlik modülü kullanıyorsanız ve yazılım tabanlı özel anahtar koruması kullanan bir RMS yüklemesinden sunucu lisans sahibi sertifikası alıyorsanız, sertifikayı alma girişiminde bulunmadan önce kümedeki her sunucunun Güvenlik ayarları sayfasında bir özel anahtar parolası belirtmeniz gerekir. |
