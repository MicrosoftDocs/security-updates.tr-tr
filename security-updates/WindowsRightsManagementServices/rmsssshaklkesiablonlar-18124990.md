---
TOCTitle: 'RMS SSS: Hak İlkesi Şablonları'
Title: 'RMS SSS: Hak İlkesi Şablonları'
ms:assetid: '01515f08-9844-4c1a-9ab5-a5a60a901b50'
ms:contentKeyID: 18124990
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720175(v=WS.10)'
---

RMS SSS: Hak İlkesi Şablonları
==============================

RMS Şablonları Hakkında SSS
---------------------------

-   [Kuruluşta en düşük düzeyde bir hak kümesi kullanılmasını sağlamak için, kuruluşta oluşturulan tüm içeriğe yönelik varsayılan bir RMS şablonu uygulayabilir miyim?](#bkmk_57)
-   [RMS ilke şablonları nerede bulunur?](#bkmk_58)
-   [Şablonlar oluşturulduğunda, kullanıcı diğer adları ve dağıtım listeleri (DL) bu şablonlara bağlanır. Birden çok bölümü olan bir kuruluş, temel hakları aynı olan şablonlar sağlayıp, bu hakları içeriğe bağlı olarak farklı gruplara nasıl verebilir?](#bkmk_59)
-   [Haklar statik bir belgeye uygulanır mı? Dosya gönderildikten sonra hakların değiştirilmesi gerekirse, yayımlama lisansı RMS "ilke" sunucusunda değil de dosyaya katıştırılmış durumdaysa, bu değişiklik yapılabilir mi?](#bkmk_60)

<span id="BKMK_57"></span>
#### Kuruluşta en düşük düzeyde bir hak kümesi kullanılmasını sağlamak için, kuruluşta oluşturulan tüm içeriğe yönelik varsayılan bir RMS şablonu uygulayabilir miyim?

Evet. Rights Management Services SDK kullanılarak, gerekli şablonun uygulanmasını sağlayabilecek özel bir uygulama geliştirilebilir. Ancak, Office 2003 veya daha ileri sürümdeki Bilgi Hakları Yönetimi uygulaması, içeriğe şablon uygulanmasını desteklemez.

<span id="BKMK_58"></span>
#### RMS ilke şablonları nerede bulunur?

Şablonun konumu, RMS etkin uygulama tarafından belirlenir. Office 2003 veya daha ileri sürümde, kayıt defterinde, bir kullanıcı ayarı olarak aşağıdaki konumda bulunur:

**HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\11.0\\Common\\DRM\\AdminTemplatePath**

-veya-

Microsoft Office 2007 için **HKEY\_CURRENT\_USER\\Software\\Microsoft\\Office\\12,0\\Common\\DRM\\AdminTemplatePath**.

| ![](images/Cc720175.note(WS.10).gif)Not                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Girdi istemcideki yerel bir klasörü gösteriyorsa, şablon dosyalarının istemciye kopyalanması gerekir. Girdi bir ağ paylaşımı klasörünü gösteriyorsa, kullanıcı çevrimdışıyken erişilemez. |

<span id="BKMK_59"></span>
#### Şablonlar oluşturulduğunda, kullanıcı diğer adları ve dağıtım listeleri (DL) bu şablonlara bağlanır. Birden çok bölümü olan bir kuruluş, temel hakları aynı olan şablonlar sağlayıp, bu hakları içeriğe bağlı olarak farklı gruplara nasıl verebilir?

Bu senaryoya yönelik iki çözüm vardır:

-   Çalışma biriminizdeki tüm çalışanlar için lisanslanmış “Şirkete Özel” adında tek bir şablon oluşturun ve sonra bu şablonu e-postada kullanıp e-postayı belirli kişilere gönderin. Bunun yararı, her çalışma birimi için e-posta olarak gönderilecek yalnızca bir tek şablon gerektirmesi ve bu e-postayı gönderdiğiniz kullanıcılarla sınırlanabilmesidir. Olumsuz yönü ise, postanın gönderildiği grup dışındaki herhangi bir kişinin bu postayı okuyabilmesidir.
-   Diğer bir yöntem, her dağıtım listesi için bir tane olacak şekilde birden çok şablon oluşturmaktır. Bu yöntem daha hassas bir denetim sağlasa da, BT bölümünün birden çok şablonla uğraşması gerektirir.

<span id="BKMK_60"></span>
#### Haklar statik bir belgeye uygulanır mı? Dosya gönderildikten sonra hakların değiştirilmesi gerekirse, yayımlama lisansı RMS "ilke" sunucusunda değil de dosyaya katıştırılmış durumdaysa, bu değişiklik yapılabilir mi?

Evet, RMS ilke şablonu kullanıldığında bu mümkündür: İçerik RMS ilke şablonu kullanılarak yayımlandığında, ilkenin tanımı sunucuda kalır ve içerik yayımlandıktan sonra yönetici tarafından değiştirilebilir. Kullanıcı içerik için lisans istediğinde, lisans, geçerli ilkenin sunucudaki tanımını temel alarak hakları verir. Kullanıcıya kullanım lisansı verildikten sonra haklar değiştirilirse, kullanıcı, kullanım lisansının verildiği zaman geçerli olan hakları kullanmaya devam eder. İçerik yayımlandıktan sonra yeni bir hak ilkesi şablonu uygulamanızı sağlamak için, şablonunuza yönelik bir süre sonu ilkesi ayarlayın ve ardından **İçerik kullanım lisansları: n gün**. Buradaki n yerine, kullanıcının kaç gün sonra yeni kullanım lisansı istemesi gerektiğini belirten sayıyı girin.
