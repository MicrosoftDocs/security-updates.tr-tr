---
TOCTitle: 'RMS SSS: Sertifikaları, Anahtarları ve Şifreleme'
Title: 'RMS SSS: Sertifikaları, Anahtarları ve Şifreleme'
ms:assetid: 'ad8cc088-1dea-44c2-be68-9091129f0f12'
ms:contentKeyID: 18125239
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747725(v=WS.10)'
---

RMS SSS: Sertifikaları, Anahtarları ve Şifreleme
================================================

RMS Sertifikaları, Anahtarları ve Şifrelemesi Hakkında SSS
----------------------------------------------------------

-   [RMS'de hangi şifreleme algoritmaları kullanılır?](#bkmk_10)
-   [RMS, FIPS sertifikalı şifreleme kullanır mı?](#bkmk_11)
-   [Tek tek kullanıcılar yerine bir dağıtım listesine izin hakkı veren yayımlama lisansları veya şablonlarda, kullanma lisansları, üyeleri dinamik olarak değerlendirmek için farklı mı kullanılır?](#bkmk_12)
-   [RMS bilgi noktasından kullanıldığında, geçici hak hesabı sertifikası (RAC) verilir. Geçici RAC'nin standart RAC'den farkı nedir? RMS'nin bilgi noktasından kullanıldığı nasıl algılanır?](#bkmk_13)
-   [Geçici RAC ne zaman kullanılır?](#bkmk_14)
-   [RMS, X.509v3 Sertifikaları verir mi?](#bkmk_15)
-   [XrML sertifikaları nerede depolanır?](#bkmk_16)
-   [Makine özel/ortak anahtar çifti nerede depolanır?](#bkmk_17)
-   [İstemci özel/ortak anahtar çifti nerede depolanır?](#bkmk_18)
-   [AES simetrik bir algoritmadır. Anahtarlar sunucu ve kullanıcı arasında nasıl güvenli aktarılır?](#bkmk_19)

<span id="BKMK_10"></span>
#### RMS'de hangi şifreleme algoritmaları kullanılır?

RMS, RMS sunucusu için 2048 bit RSA anahtarları ve kullanıcı ve makine anahtar çifti için 1024 bit RSA anahtarları kullanır.

<span id="BKMK_11"></span>
#### RMS, FIPS sertifikalı şifreleme kullanır mı?

RMS Service Pack 1 ve daha ilerisinde, RMS istemci uygulaması tarafından oluşturulan kasalar, istemci Windows XP veya Windows Server 2003 çalıştıran bir bilgisayarda yüklüyse FIPS sertifikalı AES şifrelemesi kullanır. Ancak, RMS istemcisi Windows 2000 çalıştıran bir bilgisayarda yüklüyse, FIPS sertifikalı AES kitaplığı yüklenmediğinden bu kasalar FIPS uyumlu değildir.

<span id="BKMK_12"></span>
#### Tek tek kullanıcılar yerine bir dağıtım listesine izin hakkı veren yayımlama lisansları veya şablonlarda, kullanma lisansları, üyeleri dinamik olarak değerlendirmek için farklı mı kullanılır?

Kullanım lisansları her zaman tek tek kullanıcılara verilir. Yayımlama lisansı veya şablonu bir grup adınaysa, RMS, kullanım lisansı verildiği sırada grup üyeliğini değerlendirir. Lisansı isteyen kullanıcı adlandırılmış bir grubun üyesiyse, kullanım lisansı kullanıcının kimliğine verilir.

<span id="BKMK_13"></span>
#### RMS bilgi noktasından kullanıldığında, geçici hak hesabı sertifikası (RAC) verilir. Geçici RAC'nin standart RAC'den farkı nedir? RMS'nin bilgi noktasından kullanıldığı nasıl algılanır?

RMS etkin uygulamanın, RMS istemcisinin kullanıcı için geçici veya standart RAC istemesi gerektiğini belirlemesi gerekir. Bu duruma yönelik bir algılama yöntemi yoktur. Microsoft Office 2003, kullanıcının uygun RAC'yi seçmesine olanak veren RMS etkin uygulamalara örnek olarak verilebilir.

Geçici RAC ve standart RAC arasındaki en temel fark, kullanıcı güvenlik tanımlayıcısının ve geçerlilik süresi belirtiminin bulunmasıdır. Geçici RAC'lerde kullanıcı SID'si bulunmaz ve geçerlilik süreleri dakika olarak belirtilir. Geçici RAC için varsayılan geçerlilik süresi 15 dakikadır. Bunun yanı sıra standart RAC'lerde kullanıcı SID'si bulunur ve geçerlilik süreleri gün olarak belirtilir. Standart RAC için varsayılan geçerlilik süresi 365 gündür.

<span id="BKMK_14"></span>
#### Geçici RAC ne zaman kullanılır?

Geçici RAC, kullanıcının, aşağıdaki ölçüte uyan bilgisayarlarda RMS korumalı içerik kullanmasını sağlamak üzere tasarlanmıştır:

-   RAC'nin alınmış olduğu RMS yüklemesinin bulunduğu ormanın üyesi olmayan bir bilgisayar.
-   Kullanıcı hesabının bulunduğu ormanın üyesi olmayan bir bilgisayar.
-   Kullanıcının aynı makineyi bir daha kullanıp kullanmayacağından emin olmadığı durum.

Bu ölçüte uyan bilgisayarlar, havaalanı terminallerinde, kütüphanelerde ve Internet kafelerde bulunabilir.

<span id="BKMK_15"></span>
#### RMS, X.509v3 Sertifikaları verir mi?

Hayır. RMS, X.509v3 sertifikalarının kapsamı dışında olan, kullanıcıları ve ilke ifadesini temsil etmeyi amaçlayan XrML sertifikaları verir.

<span id="BKMK_16"></span>
#### XrML sertifikaları nerede depolanır?

RMS sistemi, istemci bilgisayardaki XrML'ye kaydedilen, aşağıdaki sertifika ve lisansları kullanır.

-   Makine Sertifikası
    Dosya adı: CERT-Machine.drm dosyası
    Konum: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM\\
-   Hak hesabı sertifikası
    Dosya adı öneki: GIC
    Konum: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM
-   İstemci lisans sertifikası
    Dosya adı öneki: CLC
    Konum: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM
-   Kullanım lisansı
    Dosya adı öneki: EUL
    Konum: %USERPROFILE%\\Local Settings\\Application Data\\Microsoft\\DRM

| ![](/security-updates/images/Cc747725.note(WS.10).gif)Not                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Kullanıcı hesabında tek bir Makine Sertifikası, GIC dosyası ve CLC dosyası vardır, ancak erişilen içeriğin her bölümü için birden çok EUL dosyası bulunur. |

| ![](/security-updates/images/Cc747725.note(WS.10).gif)Not                                       |
|------------------------------------------------------------------------------------------------------------|
| RMS istemci Windows Vista® ile tümleşikse, konumu şöyledir: %USERPROFILE%\\AppData\\Local\\Microsoft\\DRM. |

<span id="BKMK_17"></span>
#### Makine özel/ortak anahtar çifti nerede depolanır?

Makine özel anahtarı, kullanıcının oturum açma kimlik bilgileri ve makine yapılandırmasıyla ilişkili şifreleme anahtarları tarafından güvenli bir şekilde korunarak depolanır.

<span id="BKMK_18"></span>
#### İstemci özel/ortak anahtar çifti nerede depolanır?

Kullanıcı hesabına ilişkin anahtar çifti, hak hesabı sertifikasında depolanır.

<span id="BKMK_19"></span>
#### AES simetrik bir algoritmadır. Anahtarlar sunucu ve kullanıcı arasında nasıl güvenli aktarılır?

Simetrik ve ortak/özel anahtarların her ikisi de sistemde kullanılır. İçerik bir simetrik anahtarla şifrelenir, ancak sistemdeki diğer anahtarlar (kullanıcı, makine ve sunucu) RSA ortak/özel anahtarlarıdır. Simetrik içerik anahtarı, yayımlama lisansındaki RMS sunucusu RSA ortak anahtarı veya kullanım lisansındaki kullanıcının RSA ortak anahtarı ile çeşitli lisanslarda her zaman şifrelenir.
