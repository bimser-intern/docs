# Stajyer Günlük Hareket Dokümanı

###### 08.03.2022 Ufuk Yetişkin

### Branch ve Commit Mesaj Formatı


#### Commit Mesajı

Pull request yapmak istediğimiz projenin dosyasında oluşturduğumuz commit mesajı ekip için çok önem arzeder. Commit mesajına bakarak yapılmış değişikliğin büyüklüğü ve ne tarz bir değişiklik olduğunu anlarız.


>`[feature/bugfix/hotfix] - [Work Item No] - [semver:major/minor/patch] - commit mesajı`


Bu format bizim commit mesajlarımız için örnek alabileceğimiz bir prototip olarak görebiliriz. 


**semver:major** 
Yapılan değişiklik bağımlılıklardan birisiyle çalışmayı etkiliyorsa majör versiyon artırılmalıdır. 
Örneğin; endpoint lere gönderilen parametrelerin değiştirilmesi veya clientdan save methodunda textbox ın değeri önceden “value” propertysinde gönderiliyorken artık “text” propertysinde gönderilmeye başlandıysa majör versiyon artırılmalıdır.
>`1.2.3 -> 2.0.0 `

**semver:minor**
Yeni eklenen özellikler minör versiyon artırılmasını gerektirir.
Örneğin; dashboarda eklenen dijital saat widgetı veya serverdaki yeni endpointden çekilen hava durumu widgetı minör versiyon artırmalıdır.
>`1.2.3 -> 1.3.0`

**semver:patch** 
Yapılan hata düzeltmeleri patch versiyon artırılmasını gerektirir.
Örneğin; dashboarddaki dijital saat 1dk geriden gelme sorunu düzeltildiyse patch versiyon artırılmalıdır.
>`1.2.3 -> 1.2.4`

**Örnek Commit Mesajı Oluşturma**

>`[feature] - [6] - [semver:minor] - Doküman içeriğinde düzenlemeler yapıldı.`



#### Branch Mesajı Oluşturma

Oluşturulmuş branchin ismi yapılan güncellemeye göre verilir. Örneğin yukarıda örnek bir commit mesajı paylaşıldı. Bu örnek commit mesajı baz alarak bu şekilde branch oluşturulabilir.

> `feature/6`


<br>
<br>
<br>

###### 09.03.2022 Ufuk Yetişkin

### Uzaktaki Repositories'e Pull Request Yapmak

Github hesabınız yoksa [Buraya](https://github.com/signup) tıklayarak kendi Github hesabınızı oluşturun.

Öncelikle katkıda bulunacağımız repositoriesin bulunduğu kaynağa gidiyoruz. Hangi branch üstünde çalışmak istiyorsak o branchi seçip daha sonra code butonuna basıyoruz ve orada bulunan URL'yi kopyalıyoruz. 

![Adsız1](https://user-images.githubusercontent.com/73849259/157441787-f1923ecd-11f9-4ec6-b918-8e8ee4e8ef45.png)


Bilgisayarımızda boş bir klasör oluşturuyoruz. Daha sonra **Windows Terminalini** açıyoruz. Oluşturduğumuz boş klasörün içerisine **cd klasor.adi** ile giriyoruz. Girdiğimiz boş dosyanın içerisine **git clone URL** komutlarını yazıyoruz. URL kısmına github repositoriesimizden aldığımız clone linkini yapıştırıyoruz. Oluşturduğumuz klasöre projemizi indiriyoruz. Daha sonra **cd .** ile projemizi test editörümüzde açıyoruz. Proje üstünde istediğimiz şekilde oynama yapabiliriz.

![Adsız2](https://user-images.githubusercontent.com/73849259/157441852-0c505b0c-6d9c-4216-8443-ccdf6f2f3e9b.png)

Kod editörü üzerinde sol alt tarafta gördüğümüz gibi branch ismi yazmaktadır. Bu branch ismine tıklıyoruz ve yeni açılan pencerede **Create new branch** yazısını seçerek kendi branchimizi oluştururuz. Branch ismi nasıl verileceği hakkındaki yazımız yukarıda bulunmaktadır. 

![Adsız3](https://user-images.githubusercontent.com/73849259/157441898-3e3afd29-4850-4dcc-b78b-6df6a4fa8436.png)

Yapmış olduğumuz değişikliklerden sonra  aşağıdaki adımları izleyerek yapılan değişiklikleri push ile göndeririz.

1. Source Control'e tıklayarak üstünde değişiklik yaptığımız dosyaları görürüz.
2. Yukarıda belirttiğimiz formata uygun commit mesajı oluştururuz ve *Enter* tuşu ile göndeririz.
3. **tik** işareti ile değişmiş olan dosyaları kaydeder ve commit ederiz.
4. **push** ile yapılan değişiklikleri göndeririz.  

![push](https://user-images.githubusercontent.com/73849259/157441957-1ad14355-415a-4d05-aad8-1874ee47b997.png)


###### 10.03.2022 Ufuk Yetişkin

