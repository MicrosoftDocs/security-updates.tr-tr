---
TOCTitle: Erişim Gereksinimlerini Belirleme
Title: Erişim Gereksinimlerini Belirleme
ms:assetid: 'eb2ce9a5-0430-4811-bd40-4a94a84426a8'
ms:contentKeyID: 18125312
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747790(v=WS.10)'
---

Erişim Gereksinimlerini Belirleme
=================================

Planlama aşamasının bu kısmında, RMS uygulamanızın kapsamını tanımlamanız gerekir. RMS sisteminizin güvenliğini değerlendirirken, katılımcılara yönelik kapsamı sınırlayabileceğiniz yöntemleri dikkate almalı ve RMS ile korudukları verilerin aynı zamanda geleneksel bilgi güvenliği yöntemleri kullanılarak da korunduğundan emin olmalısınız. Ayrıca, yönetim ve yapılandırma işlemleri için RMS sunucusuna erişimin, yalnızca güvenilen yöneticilerle sınırlandırıldığından da emin olmalısınız. RMS ile kullanabileceğiniz erişim güvenliği yöntemleri, aşağıda belirtilenleri içerir:

-   **Erişim denetim listeleri (ACL)**. Her RMS Web hizmeti ve Yönetim Web sitesi, ACL'lerle korunabilir. Kullanıcıların RMS sertifika ve lisans hizmetlerine bağlanabilme özelliklerini kısıtlamak için erişim denetim listeleri kullanarak, bu işlemleri yalnızca RMS hizmetini kullanma yetkisi olan kullanıcıların yaptığından emin olabilirsiniz. Bu, yalnızca belirli grupların korumalı içerik oluşturabilmesini istiyorsanız veya korumalı içerik için yalnızca belirli grupların lisans almasını sağlamak istiyorsanız kullanışlıdır.
-   **İstemci kimliğini doğrulama**. Kullanıcı kullanım lisansı veya sertifika almaya çalıştığında, akıllı kart kullanılmasının istenmesini veya başka bir istemci kimliği doğrulama işleminin oluşmasını sağlayabilirsiniz. Bu, yetkisiz bir kullanıcın, yetkili kullanıcının oturumunu kullanarak içeriği açma olasılığını azaltmanıza yardımcı olabilir.
-   **Güvenli Yuva Katmanı**. Ek bir koruma katmanı sağlamak için RMS istemcileri ve RMS sunucusu arasında bir SSL bağlantısı olması da gerekebilir. SSL'yi etkinleştirmeniz ve tüm RMS Web hizmetleri dosyalarında 128 bit şifreleme istemeniz önerilir. Bu dosyaların dosya adı uzantısı .asmx şeklindedir ve Licensing, Certification ve Admin sanal dizinlerinde bulunurlar. **RMS Yönetimi** Web sayfalarını uzaktaki bilgisayarda bulunan tarayıcıdan açmak istiyorsanız, SSL'yi etkinleştirmelisiniz. Ancak, SSL etkinleştirilse bile, **Genel Yönetim** sayfasını uzaktaki bilgisayardan açamazsınız.
    Sunucularda SSL yapılandırma hakkında bilgi için IIS Yardımı'na bakın.

Bazı kuruluşlarda, diğer bölümlerden yalıtılmış ve güvenli hale getirilmiş, bölümlere yönelik bir lisans sistemi gereksinimi vardır. Böyle bir senaryoda, bilgi hakları yönetim ilkeleri oluşturma yöntemi olarak RMS sunucusu kullanılabilir. Kuruluşunuzda çok önemli bilgileri denetleyen bir bölüm ve birim varsa, bu bölüm veya birime ait bilgilerin lisans ve yayım işlemlerini, kuruluşun diğer bölümlerinden ayrı olarak yönetmek üzere ayrı bir lisans sunucusu veya lisans kümesi kurmayı düşünebilirsiniz. Lisans sunucusuna, her lisans sunucusuna yönelik sertifika ve diğer hizmetleri sağlayan kök sertifika sunucusuyla (veya kümesiyle) alt kayıt işlemi yaptırılır. Ancak, lisans sunucuları kendi lisanslama ve yayımlama hizmetlerini sağlar.

Kullanıcı hesapları, ACL'ler ve fiziksel güvenlik, dağıtımınızın en önemli bileşenleridir. RMS'yi üretim ortamına uygulamadan önce, en iyi güvenlik yöntemlerini değerlendirip uyguladığınızdan ve en uygun güvenlik modelini kullandığınızdan emin olun.
