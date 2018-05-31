---
TOCTitle: Sunucuları Hizmetten Çekme
Title: Sunucuları Hizmetten Çekme
ms:assetid: '52005e2e-9563-4ba0-906c-3cc76f9c378f'
ms:contentKeyID: 18125091
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc747568(v=WS.10)'
---

Sunucuları Hizmetten Çekme
==========================

Bir RMS sunucusunu, örneğin aşağıdaki durumlardan dolayı, hizmetten çekme gereksinimi duyduğunuz zamanlar olabilir:

-   Belirli sunucuların değiştirilmesiyle sonuçlanan donatım sorunları veya yükseltmeler.
-   Bazı sunucuların yetkilerinin alınmasıyla sonuçlanan lisans ve yayımlama trafiğinde azalma.
-   Bir kümenin bütünün yetkisinin alınmasıyla sonuçlanan, sunucuların belirli konumlardan kaldırılmasıyla ilgili yasal gereksimler.
-   Varlıkların aktarılmasıyla sonuçlanan, bir kuruluşun bölümlerinin veya diğer kısımlarının birleştirilmesi veya satışı.
-   Kuruluşun bütününün RMS kullanan başka bir kuruluşla birleştirilmesi ve her iki RMS yüklemesinin gereksiz hale gelmesi.

Bir sunucuyu hizmetten çekmeden önce, başta yapılandırma veritabanı olmak üzere sunucu tarafından kullanılan tüm RMS veritabanlarını yedeklemeniz gerekir. Veritabanlarını yedekleme hakkında daha fazla bilgi için bu belge grubunun "RMS Dağıtımı Planlama" bölümündeki "RMS Sistemini Yedekleme ve Geri Yükleme" konusuna bakın. .

Veritabanlarını yedekledikten sonra sunucuyu kaldırabilirsiniz. Bir RMS sunucusunu kaldırma gereksinimleri, sunucunun rolüne ve RMS yüklemesinin topolojisine bağlıdır:

-   **Kümeden bir sunucu kaldırma**. Hizmetten çekmek istediğiniz RMS sunucusu diğer RMS sunucularının hala etkin ve gerekli olduğu bir kümede bulunuyorsa, tek bir RMS sunucusunun kümeden kaldırılması kullanım dışı bırakmak istediğiniz sunucu üzerindeki RMS'yi ve hazırlığını kaldırmanızı, donanımı kümeden kaldırmanızı ve veritabanlarını arşivlemenizi gerektirir.
    | ![](/security-updates/images/Cc747568.note(WS.10).gif)Not                                                                                    |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------|
    | RMS'yi kaldırmadan önce yalnızca kök yükleme kümesindeki sunucuların hazırlığının kaldırılması gerekir. Bu işlem lisans sunucularında gerekli değildir. |

-   **Tek başına çalışan bir sunucuyu hizmetten çekme**. Hizmetten çekmek istediğiniz RMS sunucusu yeni bir sunucuyla değiştireceğiniz bağımsız bir Windows RMS sunucusuysa (başka bir deyişle, çok sunuculu bir kümenin parçası değilse), aşağıdaki adımları uygulayın: Varolan RMS sunucusunun hazırlığını ve kendisini kaldırın, bu sunucuyu ağdan çıkarın ve hemen ardından RMS'yi değiştirilen sunucuya yükleyin ve hazırlayın. Yeni RMS sunucusunu hizmetten çekilen RMS sunucusuyla aynı URL ve yapılandırma veritabanını kullanacak şekilde yapılandırın. Değiştirilen sunucu yüklenip hazırlanıncaya kadar kullanıcıların hizmetten çekilen sunucu tarafından yayımlanan içeriği kullanamayacaklarını unutmayın.
    | ![](/security-updates/images/Cc747568.Important(WS.10).gif)Önemli                                                                                                                                                                                 |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Değiştirdiğiniz RMS sunucusu bir donanım güvenlik modülü kullanıyorsa, RMS'yi yeni sunucu üzerine yükleyip hazırlamadan önce güvenlik uzayını yeni sunucuya aktarmanız gerekir. Yönergeler için donanım güvenlik modülüyle birlikte verilen belgelere bakın. |

-   **RMS yüklemesini varolan başka bir RMS yüklemesiyle değiştirme**. Bazı durumlarda, örneğin her iki şirketin de RMS'yi çalıştırdığı bir şirket birleşmesinde, RMS yüklemesini hizmetten çekme ve varolan başka bir RMS yüklemesiyle değiştirme gereksinimi duyabilirsiniz.

Bir sunucunun hazırlığını ve sunucuyu kaldırdığınızda, sunucu yapılandırma veritabanının ClusterServer tablosundan kaldırılır ve dizin hizmetleri veritabanı SQL Server'dan silinir. RMS'nin yapılandırmasını geri alma ve kaldırma hakkında yönergeler için, bu konuda daha sonra yer alan "[RMS Yapılandırmasını Geri Almak için](https://technet.microsoft.com/9fa63daa-5fb9-4afd-8371-b38248619857)" ve "[RMS'yi Kaldırmak için](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)" bölümlerine bakın.
