---
TOCTitle: RMS Hizmet Hesabı Parolasını Değiştirme
Title: RMS Hizmet Hesabı Parolasını Değiştirme
ms:assetid: '435c9cef-b622-48b3-9d4d-4bf5cac7d52d'
ms:contentKeyID: 18125067
ms:mtpsurl: 'https://technet.microsoft.com/tr-tr/library/Cc720273(v=WS.10)'
---

RMS Hizmet Hesabı Parolasını Değiştirme
=======================================

RMS hizmet hesabı parolasının kullanım süresi, RMS sunucuları için belirttiğiniz parola ilkesine bağlı olarak dönemsel olarak sona erebilir. Parolanın geçerliliği sona ererse RMS işlevlerini yerine getirmeyi bırakacaktır. Bundan ötürü, parolayı kullanım tarihi süresi dolmadan değiştirmeniz gerekir.

**Tek RMS Hizmet Hesabı Kullanma**

Bir RMS hizmet hesabını kullandığınızda parolayı aşağıda belirtildiği şekilde her RMS sunucusunda değiştirebilirsiniz:

1.  Sunucu kümede bulunuyorsa, sunucuyu döngünün dışına çıkarın.
2.  RMS hizmet hesabının kimlik bilgilerini kullanarak sunucuda oturum açın.
3.  RMS hizmet hesabı parolasını değiştirin.
    Aynı RMS hizmet hesabını kullanan diğer sunucular, parola değiştirildikten sonra bu sunucular tarafından saklanan kimlik bilgileri geçersiz olacağı için hizmet dışı sorunu yaşayacaktır.
4.  Sunucu oturumunu kapatın.
5.  RMS yönetici kimlik bilgilerini kullanarak sunucuda yeniden oturum açın.
6.  Sunucu üzerindeki kullanıcı kimliğini yeniden yapılandırmak için **Genel Yönetim** sayfasında, **RMS Hizmet Hesabını Değiştir**'i tıklatın ve ardından **RMS Hizmet Hesabını Değiştir** sayfasında etki alanını, kullanıcı adını ve parolayı belirtin.
7.  IIS'yi yeniden başlatın.
8.  Uygunsa sunucuyu yeniden döngüye yerleştirin.
9.  Kümede bulunan her sunucu için 6. adımdan 8. adıma kadar tekrar edin.

Bu, RMS hizmet hesabı parolasını değiştirmek için izlenebilecek en basit yoldur, ancak bir sunucuda RMS hizmet hesabını değiştirdiğinizde Active Directory yeni parola ile güncelleştirileceği için RMS'nin belirli bir süre kullanım dışı kalmasına yol açabilir. IIS, uygulama havuzlarını periyodik olarak yeniden başlatır ve siz RMS hizmet hesabı parolasını değiştirip IIS'yi bu sunucu üzerinde yeniden başlatmadan, eski kimlik bilgileriyle çalışan bu uygulama havuzları başlatılamaz. RMS, uygulama havuzları yeniden çalışmaya başlayana kadar işlevlerini yerine getiremez.

**İki RMS Hizmet Hesabı Kullanma**

Bu yöntemde, farklı süre sonu ilkeleri veya tarihleri olan iki RMS hizmet hesabı oluşturun. Normal işlemler sırasında RMS ilk hesabın altında çalışır. İlk hesap için hizmet hesabı parolasını değiştirmeye hazır olduğunuzda, her RMS sunucusunda aşağıdaki adımları uygulayın:

1.  Sunucu kümede bulunuyorsa, sunucuyu döngünün dışına çıkarın.
2.  İkinci RMS hizmet hesabını RMS'yi çalıştıracak hesap olarak belirtin. Hesap değiştirmeyle ilgili yönergeler için bu konuda daha sonra yer alan "[RMS Hizmet Hesabını Değiştirme](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)" bölümüne bakın.
3.  IIS'yi yeniden başlatın.
4.  Uygunsa sunucuyu yeniden döngüye yerleştirin.

Tüm RMS sunucuları ikinci RMS hizmet hesabını kullanmaya başladıktan sonra, ilk RMS hizmet hesabındaki parolayı, RMS sisteminin çalışmasını etkilemeden değiştirebilirsiniz. Bu şekilde, RMS'de kesinti oluşmasını engelleyerek, iki hesap arasında geçiş yapabilirsiniz.
