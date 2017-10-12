---
TOCTitle: RMS Özel Anahtarını Değiştirme
Title: RMS Özel Anahtarını Değiştirme
ms:assetid: 'da32137e-394a-42b2-9552-ba20f4547c23'
ms:contentKeyID: 18125298
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747765(v=WS.10)'
---

RMS Özel Anahtarını Değiştirme
==============================

RMS, sağlama sırasında sunucu için RMS özel anahtarı oluşturur. RMS özel anahtarı şifrelidir ve yapılandırma veritabanında saklanır. Özel anahtarı yedeklemeniz ve güvenli bir yerde saklamanız tavsiye edilir. Ek olarak, RMS özel anahtarı RMS sunucusunun koruduğu tüm içerik şifreleme şemasında kullanılacağından dolayı, bu anahtarın güvenliğini sağlamak için donanımsal bir güvenlik modülü kullanma seçeneğini göz önüne alın. RMS özel anahtarından herhangi bir şekilde kuşkulanılıyorsa RMS yapılandırmasını geri almanız, RMS'yi tekrar yapılandırmanız ve yeni bir RMS özel anahtarı almanız gerekir.

İçeriği korumak için sunucu kullanılıyorsa, tüm içerik sahiplerine bilgi verilmeli ve RMS sunucusu yeni özel anahtarla birlikte kullanılarak içerik yeniden yayımlanmalıdır. Kuşkulu özel anahtar ile korunan içeriğin yeterince korunduğu düşünülemeyeceği tüm kopyaları yok edilmelidir.

| ![](images/Cc747765.Important(WS.10).gif)Önemli                                                                                                                                                                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Yeni bir özel anahtar almak için, sunucu, Microsoft Kayıt Hizmetine kaydettirilip kaydettirilmediğinden bağımsız olarak sağlama işlemini yinelemelidir. RMS sunucusunu tekrar kaydettirmeyi denediyseniz bir önceki RMS özel anahtarı kullanılacaktır |
