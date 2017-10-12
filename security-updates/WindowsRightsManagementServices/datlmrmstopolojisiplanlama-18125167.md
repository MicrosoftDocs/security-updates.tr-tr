---
TOCTitle: Dağıtılmış RMS Topolojisi Planlama
Title: Dağıtılmış RMS Topolojisi Planlama
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18125167
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747657(v=WS.10)'
---

Dağıtılmış RMS Topolojisi Planlama
==================================

Bazı durumlarda, kök sertifika kümesinin üyesi olmayan bir veya daha çok lisans sunucusu dağıtmanız gerekebilir. Genelde bunu, yayımlama ve kullanım lisansları üzerinde doğrudan denetimleri olması gereken, güvenlik gereksinimleri bölüm düzeyinde denetimi zorunlu kılan hukuk bölümü gibi bölümleri desteklemek için yaparsınız. Kök sertifika kümesi, lisans sunucuları için hesap sertifikası hizmeti sağlar. Kök sertifika sunucusu ve bir veya birkaç lisans sunucusu yüklemesinin birleşimine dağıtılmış topoloji denir.

Kök sertifika sunucuları gibi, lisans sunucuları da küme içinde dağıtılabilir. Ayrıca lisans kümesi, kök sertifika kümesine benzer şekilde kendi yük dengeleme hizmetini kullanır. Her lisans sunucusu veya lisans kümesi, söz konusu sunucu veya küme için yapılandırma ve günlük veritabanları sağlamak amacıyla ayrı bir SQL Server örneği kullanır.

RMS yüklemesini, kök yüklemesinden yalnızca sertifika hizmetlerini çalıştıracak ve tüm lisans hizmetini bir veya birkaç lisans sunucusu veya kümesinden çalıştıracak biçimde kurabilirsiniz, ancak bu standart yapılandırma değildir. Genellikle, performans ve artıklık gereksinimlerini karşılamak için ayrı lisans sunucuları dağıtmak yerine kök sertifika kümesindeki fiziksel sunucu sayısını artırırsınız (lisans için bölüm düzeyinde desteğe gereksiniminiz yoksa). Aşağıdaki şekilde bu dağıtım gösterilmektedir.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

Dağıtılmış topoloji oluşturmak, bu topoloji yapısı gereği daha karmaşık olduğundan kuruluşunuzun yönetim maliyetlerini artırabilir. Kuruluşunuzda birden çok küme ve orman varsa, RMS istemci bilgisayarlarının lisans isteklerini doğru RMS sunucusundan almalarını sağlamak için bu RMS istemci bilgisayarlarındaki kayıt defterinde değişiklik yapmanız gerekebilir. Ayrıca, etki alanları arasında güven sorunları yaşanabilir. Bu, RMS korumalı içeriğin kullanılmasını sağlamak için etki alanlarınızda ek yapılandırma yapmanızı gerektirir.

Dağıtılmış Topolojisinde Hizmet Bağlantı Noktaları
--------------------------------------------------

RMS sunucusu sağladığınızda, hizmet bağlantı noktasındaki (SCP) Active Directory ormanına bir küme URL'si eklenir. Kök sertifika kümesi ve ormanda sağladığınız her lisans kümesi için bir SCP vardır. SCP'nin, lisans kümesi sağlamadan önce kök sertifika kümesine kaydettirilmesi gerekir. Lisans kümesini sağladığınızda, alt kayıt işlemi, ağınızdaki kök sertifika kümesini bulmak için bu URL'yi kullanır ve bir sunucu lisans sertifikası alır.

Tek bir kök sertifika sunucusu yerine kök sertifika kümesi dağıtırsanız, kümedeki her sunucunun paylaşılan URL'nin ardında sanal olarak adreslenebilmesi gerekir.

Sanal adreslemenin, hepsinin bir kez denendiği DNS, Ağ Yük Dengeleme hizmeti veya donanım çözümleri gibi çeşitli uygulamaları vardır. Sanal adresleme sunucular arasında yük dengelemesi sağlar ve ayrıca lisans ve yayımlama için herhangi bir sunucuya bağımlılığı da ortadan kaldırır.

RMS, lisans alma URL'si için ve son kullanıcı bilgisayarlarının Active Directory'de veya kayıt defterinde RMS kümesini ararken kullandığı yayımlanan değer için paylaşılan bir URL kullanır. Hiçbir son kullanıcı bilgisayarı kümedeki tek bir sunucuya doğrudan erişim gerektirmez.
