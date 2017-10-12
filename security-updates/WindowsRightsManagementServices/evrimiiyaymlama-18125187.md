---
TOCTitle: Çevrimiçi Yayımlama
Title: Çevrimiçi Yayımlama
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18125187
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747694(v=WS.10)'
---

Çevrimiçi Yayımlama
===================

Aşağıdaki diyagram çevrimiçi yayımlama işlemini açıklamaktadır.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

Çevrimiçi yayımlama işlemi aşağıdaki adımları içerir:

1.  İçerik yazarı bir belge oluşturur ve kullanıcıları belirtmek ve içeriğe yönelik haklar ve koşullar uygulamak için RMS etkin bir uygulama kullanır.
2.  RMS etkin uygulama bir simetrik içerik anahtarı oluşturur ve sertifika sunucusuna veya lisans sunucusuna yayımlama lisansı için istek gönderir. İstek içerik anahtarını ve kullanım ayarlarını içerir.
3.  Lisans sunucusu yayımlama lisansını oluşturur ve içerik anahtarını sunucu ortak anahtarıyla şifreledikten sonra yayımlama lisansını RMS etkin uygulamaya döndürür.
4.  Uygulama dosyayı içerik anahtarıyla şifreler ve yayımlama lisansını dosyaya bağlar.
5.  İçerik kullanıcısının bilgisayarındaki RMS etkin uygulama, belge için kullanım lisansı istemek üzere, kullanıcının hak hesabı sertifikasını içeren bir isteği (yayımlama lisansını veren) RMS sunucusuna gönderir.
6.  RMS sunucusu kullanıcının kimlik bilgilerini doğrular. Kullanıcı başarıyla doğrulanırsa, bir kullanım lisansı oluşturulur ve bu kullanım lisansı içerik kullanıcısının bilgisayarındaki RMS etkin uygulamaya döndürülür.
7.  RMS etkin uygulama belgeyi açar ve kullanım lisansında tanımlanan parametrelere göre kullanıcı hakları verir.
