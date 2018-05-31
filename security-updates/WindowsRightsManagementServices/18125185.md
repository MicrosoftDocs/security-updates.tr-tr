---
TOCTitle: RMS için Active Directory Desteği
Title: RMS için Active Directory Desteği
ms:assetid: '9589127d-19b3-44f1-b7a1-01992e78218a'
ms:contentKeyID: 18125185
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747604(v=WS.10)'
---

RMS için Active Directory Desteği
=================================

RMS, Active Directory'yi aşağıdaki amaçlar için kullanır:

-   **Kullanıcı kimliğini doğrulama.** Active Directory, RMS kullanıcılarının kimliğini doğrulamak için kullanılan dizin hizmetlerini sağlar. Kimlik doğrulaması ve RMS hakkında daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS Güvenlik Modeli](https://technet.microsoft.com/665db831-366d-4dca-9bb3-cc2912481fe1)" bölümüne bakın.
-   **Grup üyeliğini ve kullanıcı hesap kimliklerini çözümleme.** Yayımlama lisansı tek tek kullanıcı hesapları yerine gruplara yönelik haklar verdiğinde, Active Directory, RMS'nin RMS korumalı içeriğe kullanım lisansları vermek için kullandığı grup üyelikleri hakkında bilgiler sağlar. Active Directory'ye yönelik LDAP sorgusu sayısını azaltmak için, RMS yerel önbellekten alınan bilgileri merkezi bir dizin hizmetleri veritabanının yanı sıra bir yerel önbelleğe de kaydeder. Daha fazla bilgi için, bu konuda daha önce yer alan "[RMS Active Directory Önbelleği](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)" ve "[RMS Dizin Hizmetleri Veritabanı](https://technet.microsoft.com/6f6b8586-5d17-4a40-94a3-4dc738195301)" bölümlerine bakın.
-   **RMS hizmet bulma konumunu depolama.** Hizmet isteklerinin (örneğin kullanım lisansı, yayım lisansı veya bir lisans sunucusunun alt kaydı için), isteğe izin veren Web hizmetinin yürütülebilir modülünün URL'sine gönderilmesi gerekir. Tüm hizmet istekleri, hizmet isteğine uygun URL'yi sağlayan sunucu Web hizmetinin (Server.asmx) URL'sine yönelik bir Active Directory sorgusuyla başlar. Daha fazla bilgi için, bu konuda daha sonra yer alan "[RMS Hizmeti Yayımlama ve Bulma](https://technet.microsoft.com/336c0d55-fd7f-4aa9-b3e6-bfd6565b1086)" bölümüne bakın.
