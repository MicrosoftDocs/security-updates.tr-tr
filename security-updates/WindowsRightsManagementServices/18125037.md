---
TOCTitle: Performansı En İyi Duruma Getirme
Title: Performansı En İyi Duruma Getirme
ms:assetid: '24dc9ca4-652b-41a6-9a99-95fdeca9120b'
ms:contentKeyID: 18125037
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720220(v=WS.10)'
---

Performansı En İyi Duruma Getirme
=================================

Bu bölümdeki başlıklarda RMS dağıtımınızın performansını en iyi duruma getirme hakkında bilgi verilmektedir.

Dizin Hizmetleri Performansını En İyi Duruma Getirme
----------------------------------------------------

RMS'de bulunan dizin hizmetleri performans sayaçlarını izleyebilirsiniz. Gerekiyorsa, Active Directory önbelleğinin özniteliklerini denetleyen kayıt defteri ayarlarını değiştirerek performansı en iyi duruma getirebilirsiniz.

Kayıt defteri ayarları Active Directory önbelleğinin aşağıdaki özniteliklerini denetler:

-   Önbelleğe alınabilecek en fazla sorumlu sayısı
-   Sorumlular için önbelleğe alınan bilgilerin geçerlilik dönemi
-   Önbelleğe alınabilecek en fazla grup sayısı
-   Gruplar için önbelleğe alınan bilgilerin geçerlilik dönemi
-   En fazla grup üyeliği girişi sayısı
-   Gruplar için önbelleğe alınan bilgilerin geçerlilik dönemi

Genellikle, önbelleğe alınan bilgiler için belirlenen geçerlilik dönemi ne kadar uzunsa veya önbellekte ne kadar çok giriş varsa, Windows RMS, dizin hizmetleri bilgilerini almayı gerektiren istekleri o kadar hızlı yanıtlayabilir. Bilgiler Active Directory önbelleğinde saklanırsa, arama yapmak için Active Directory'ye gidip gelmek gerekmez. Bu, isteği yanıtlama süresini kısaltır.

Active Directory önbelleğinde daha fazla bilgi saklamanın bedeli, daha fazla sistem belleği kaynaklarının gerekmesidir. Kayıt defteri ayarlarını yapılandırırken göz önünde bulundurulması gereken diğer bir konu, bir öğe için belirlenen geçerlilik dönemi uzadıkça Active Directory önbelleğinden dönen sonuçlardan bazılarının geçersiz olma olasılığının artmasıdır. Bu, bilgilerin Active Directory'de değiştirilmesi, fakat bu değişikliklerin Active Directory önbelleğine yansıtılmaması durumunda ortaya çıkabilir. Active Directory'de sık değişiklik yapılıyorsa, önbelleğe alınan bilgiler için bu sıklığı yansıtan daha kısa bir geçerlilik süresi belirlemeniz gerekebilir.

Dizin hizmetleri performans sayaçları, bu konuda daha sonra yer alan "[RMS: Dizin Hizmetleri Performans Sayaçları](https://technet.microsoft.com/37afea1d-f320-4040-96d8-57c0b45e6d46)” bölümünde açıklanmaktadır. Kullanım yönergeleri için bu konuda daha önce geçen "[Performans Sayaçlarını Kullanma](https://technet.microsoft.com/096c3b17-c082-46c4-939c-4373af0c9dec)" bölümüne bakın. İzlenecek sayaçlar, "isabet sayısı" ve "kaçırılan sayısı"dır. RMS her isabetsiz arama için bir Active Directory araması gerçekleştirmelidir.

Kayıt defteri ayarları ve bu ayarları değiştirme yönergeleri hakkında ayrıntılı bilgi için, bu konuda daha sonra yer alan "[Active Directory Önbellek Ayarlarını Değiştirme](https://technet.microsoft.com/8789a7a5-2065-4fae-9104-e0a70f1f2fb6)" bölümüne bakın.

Active Directory Bağlantı Havuzu Ayarlarını En İyi Duruma Getirme
-----------------------------------------------------------------

Sistem performansını artırmak için Active Directory Basit Dizin Erişimi Protokolü (LDAP) bağlantı havuzu ayarlarını denetleyen kayıt defteri anahtarları ekleyebilir ve bu anahtarları değiştirebilirsiniz. Kayıt defteri ayarlarını yapılandırma, bu konuda daha sonra yer alan "[Bağlantı Havuzu Kayıt Defteri Ayarlarını Değiştirme](https://technet.microsoft.com/c61d91db-a1ad-4ca5-a492-015da629afbc)" bölümünde açıklanmaktadır.

RMS, LDAP bağlantılarını en iyi duruma getirecek biçimde tasarlanmıştır. RMS her Active Directory genel kataloğu için bir bağlantı sağlar ve her bağlantı birden fazla iş parçacığına hizmet edebilir. Ayrıca, sağlamlık sunmak için isteklere hizmet edecek bir bağlantı havuzu yürütür. RMS, tek bir genel kataloğa aşırı yüklenmeyi önlemek için, sorgulanacak kataloglar listesindeki genel kataloglar arasında yükü dengeleyerek istekleri dağıtan bir algoritma kullanır. Ayrıca, LDAP hatalarını işler ve gerekirse istekleri farklı bir genel kataloğa yönlendirir.

RMS, Topoloji Bulma algoritması kullanarak sorgulanacak genel katalogların listesini oluşturur. RMS hizmetlerinin başlayabilmesi için Topoloji Bulma'nın bulması gereken kullanılabilir genel katalogların en az ve en fazla sayısını belirtebilirsiniz. Topoloji Bulma, ilk olarak geçerli işletmedeki genel katalogları bulur. Ek genel kataloglar gerekiyorsa, bu ek katalogları diğer sitelerde arar. RMS'nin istekleri kabul etmeyi kesmesinden önce kullanılmaz duruma gelebilecek en fazla bağlantı sayısını da belirtebilirsiniz. Sorgu listesindeki bir veya birkaç genel katalog daha sonra kullanılamaz duruma gelirse, Topoloji Bulma, sorgu listesine eklenecek yedek genel kataloglar aramaya başlar.

Alternatif olarak, RMS'nin kullanmasını istediğiniz genel katalogların listesini hazırlayabilirsiniz. Bu durumda, Topoloji Bulma sorgu listesine eklemek üzere genel katalog aramaz.

Ayrıca, RMS'nin genel kataloglar arasında yük dengelemeyi nasıl gerçekleştireceğini belirleyen ayarları da yapılandırabilirsiniz. Belirli bir isteği belirli bir genel kataloğa gönderip göndermemeye karar verirken, aşağıdaki hususların birbirlerine göre ne kadar önemli olduğunu belirtebilirsiniz:

-   **Hepsini bir kez deneme (WtRoundRobin)**. Bu parametre, sürekli çalışma mantığını kullanan yük dengelemenin göreli önemini belirtir. Varsayılan ağırlık ayarı, bunun sunucunun genel katalog seçiminde en az önem vereceği husus olduğu anlamına gelen 1'dir.
-   **Bağlantı sırasında iş parçacığı sayısı (WtThreadCount)**. Bu parametre bağlantı için ayrılan iş parçacığı sayısının göreli önemini belirtir. Varsayılan ağırlık ayarı 100'dür. Bu, seçilecek bağlantı için genel katalog iş parçacığı sayısının düşük olmasının, sürekli çalışma mantığı kullanılarak yapılan yük dengelemesinden 100 kez daha önemli olduğu anlamına gelir.
-   **Yavaş bağlantı (WtSlow)**. Bu parametre yavaş bağlantının göreli önemini belirtir. Varsayılan ağırlık ayarı 1000'dir. Bu, genel katalog için seçilecek bağlantının yavaş olmamasının, iş parçacığı sayısının düşük olmasından 10 kez daha önemli olduğunu gösterir.
