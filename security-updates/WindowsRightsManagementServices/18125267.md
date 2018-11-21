---
TOCTitle: RMS Active Directory Önbelleği
Title: RMS Active Directory Önbelleği
ms:assetid: 'c721a2eb-2fe9-4346-b426-3cc169b97265'
ms:contentKeyID: 18125267
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747662(v=WS.10)'
---

RMS Active Directory Önbelleği
==============================

Her RMS kök sertifika sunucusu veya kümesi ve lisans sunucusu, Active Directory genel kataloğu grup üyeliği sorgularının sonuçlarını içeren bir yerel Active Directory önbelleği içerir. Her sunucudaki önbelleğin yanı sıra, her küme için, dizin hizmetleri veritabanında depolanan bir paylaşılan önbellek de bulunur. Bu önbelleklerin amacı, genel kataloga gönderilen sorgu sayısını ve lisans isteklerini yanıtlama süresini azaltmaktır.

Kullanıcı kullanım lisansı isteğinde bulunduğunda, yanıt veren sunucunun, kullanıcıya yayımlama lisansında gerekli hakların verilip verilmediğini değerlendirmesi gerekir. En basit senaryoda, lisans isteğinde bulunan kullanıcının adı yayımlama lisansında açık olarak belirtilir. Ancak çoğu senaryoda yazar, hakları bireysel kullanıcılardan çok bir gruba verir.

Yayımlama lisansında istekte bulunan kullanıcının adı açıkça belirtilmez ve bunun yerine ilgili haklar bir gruba verilirse; kullanıcının hakların verildiği grubun üyesi olup olmadığının belirlemek üzere sunucunun, kullanıcının grup üyeliklerini değerlendirmesi gerekir. Bunu yapmak için sunucu genel kataloğa bir LDAP sorgusu gönderir.

RMS sunucuları tüm grup üyeliği sorgusu sonuçlarını hem yerel Active Directory önbelleğine hem de küme dizini hizmetleri veritabanına kaydeder. Sunucular daha sonra genel kataloga göndermeleri gereken sorguların sayısını azaltan bu önbelleklerden grup üyeliği bilgilerini elde edebilirler. Varsayılan olarak, en yakın sunucu sorgulanır; ancak sorgulanacak genel katalog sunucularını belirtmek için GC kayıt defteri anahtarını yapılandırabilirsiniz. Bu ayar hakkında daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Bağlantı Havuzu Kayıt Defteri Ayarlarını Değiştirme" konusuna bakın.

Kullanıcının grup üyeliklerini değerlendirmek için sunucu, önbellekte kullanıcının grup üyelik bilgilerinin zaten bulunup bulunmadığını görmek için önce önbelleğini denetler. Yoksa, bunun ardından sunucu kümenin dizin hizmetleri veritabanını denetler. Grup üyelik bilgileri bu veritabanında depolanmıyorsa, sunucu genel katalogu sorgular.

Kullanıcılar ve gruplar için aşağıdaki Active Directory öznitelikleri önbelleğe kaydedilir:

-   mail
-   ProxyAddresses (yalnızca SMTP e-posta adresleri)
-   objectSID
-   sidHistory
-   memberOf (kullanıcı veya grubun üyesi olduğu grupların GUID'leri)

Yerel Active Directory önbelleğindeki girdiler zaman damgalıdır. Kayıt defteri ayarları önbelleğe kaydedilebilen toplam girdi sayısının yanı sıra önbellekte bulunan girdilerin geçerlilik dönemini belirtir. Bu ayarlar sunucularınızın performansını etkileyebilir. Daha fazla bilgi için, bu belge grubundaki "RMS Sunucusunu Çalıştırma" bölümünde bulunan "Active Directory Önbellek Ayarlarını Değiştirme" konusuna bakın.
