
## İçindekiler
1. [Git Versiyon Kontrol Sistemi](#git-versiyon-kontrol)
   - [Git Versiyon Kontrol Sistemi'nin Tercih Edilme Sebebi](#git-versiyon-kontrol)
2. [Temel Git Komutları](#git-komutlari)
3. [Branch ve Commit Mesaj Formatı](#branch-commit-format)
4. [Uzaktaki Reporisitories'e Pull Request Yapmak](#pull-request)

---
<br>
<br>
<br>



<h3 id="git-versiyon-kontrol"></h3>

# Git Versiyon Kontrol Sistemi

---

Git Versiyon Kontrol Sistemi, bir proje üzerinde birden çok kişinin çalışmasına ve her birinin kendi versiyonunu oluşturmasına, daha sonra değişiklik yapılmak istendiğinde istenilen versiyona dönülüp oradan değişiklik yapılmasına olanak veren bir kontrol sistemidir. Proje üzerinde yapılan bir değişikliğin sadece ilgili kısmını değil, projenin tamamını bir bütün halinde saklar, böylelikle projenin son halinin her geliştirici tarafından bir bütün halinde görülmesine olanak sağlar. Yerel ve uzak bilgisayarlar olmak üzere 2 ortam söz konusudur. 


## Git Versiyon Kontrol Sistemi’nin Tercih Edilme Sebebi

Lokal bir geliştirme ortamında Versiyon Kontrol kullanılmadan geliştirilen yazılımın diskte meydana gelecek bir sorun sonucu kaybedilme ihtimaline karşın, Versiyon Kontrol Sistemi’nin geliştirme aşamalarının tamamı farklı versiyonlar olarak kaydedilir ve olası bir soruna karşı her biri için ayrı ayrı yedekleme gerektirmeden istenildiği zaman istenilen versiyona dönülebilecek şekilde kaydedilir.

Grup çalışmasına olanak sağlaması ise diğer bir kullanılma sebebidir. Bir proje üzerinde çalışan birden fazla kişinin aynı kaynak kod üzerinde yaptıkları farklı değişiklikler tüm geliştiriciler tarafından görülebilir ve her aşama versiyonlandığı için istenilen aşamadan değişiklik yapılmaya devam edilebilir. Harici disk kullanılması gibi vakit kaybına sebep olacak yöntemlere gerek kalmaksızın her geliştirici kendi istediği değişiklikleri yapabilir, diğer geliştiriciler de bu değişiklikleri görebilir ve üzerine ekleyerek devam edebilir. 

### Yerel Versiyon Kontrol Sistemleri

Çoğu insanın versiyon kontrol metodu, ilgili dosyaları başka bir yere kopyalamaktır (Muhtemelen daha zeki olanları, klasör isimlendirmesinde zaman damgası kullanıyordur). Bu yaklaşım basit olduğundan çok yaygındır fakat aynı zamanda inanılmaz derecede hataya açık bir yaklaşımdır. Hangi dizinde bulunduğunuzu unutmak, yanlışlıkla yanlış dosya üzerine yazmak veya istemediğiniz dosyaların üzerine yazmak gibi ihtimallerin gerçekleşmesi çok olasıdır.

![gitlocalcomputer](https://user-images.githubusercontent.com/73849259/156150825-73dc33bf-b6d6-436e-a82a-3c61bafd0f11.png)


### Merkezî Versiyon Kontrol Sistemleri

İnsanların karşılaştığı bir diğer büyük problemse diğer sistemlerdeki geliştiricilerle iş birliği yapmak zorunda kalmalarıydı. Bu problemin çözümü olarak Merkezî Versiyon Kontrol Sistemleri (MVKS) geliştirildi. Bu sistemler (CVS, Subversion ve Perforce gibi) bütün sürümlendirilmiş dosyaları barındıran tek bir sunucuya ve o sunucudaki dosyaları merkezî bir yerden sürekli denetleyen istemcilere sahipti. Uzun yıllar boyunca bu sistem, versiyon kontrol sistemleri için standart oldu.

![gitcenteral](https://user-images.githubusercontent.com/73849259/156150875-2e80aaa2-6246-4e03-85e0-316974c50aaa.png)


### Dağıtık Versiyon Kontrol Sistemleri

İşte tam da burada devreye Dağıtık Versiyon Kontrol Sistemleri (DVKS) giriyor. Bir DVKS’de (Git, Mercurial, Bazaar ya da Darcs gibi) istemciler sadece dosyaların son anlık görünümünü denetlemezler, daha çok depoyu deponun tam tarihiyle birlikte yansıtırlar. Dolayısıyla eğer herhangi bir sunucu devre dışı kalırsa, birbiriyle o sunucu aracılığıyla iş birliği yapan sistemlerdeki herhangi bir istemci deposu sunucuyu yenilemek için geri yüklenebilir. Her klon, en nihayetinde tüm verilerin tam bir yedeğidir aslında.

![gitdagitik](https://user-images.githubusercontent.com/73849259/156150958-a2fd591b-b28b-4471-8203-256b9dff7f2e.png)


<h3 id="git-komutlari"></h3>

## Temel Git Komutları

#### git config
Bu komut ile kullanıcı adı ve e-posta adresi yapılandırılır ve sonraki tüm projelerde bu kullanıcı adı ve e-posta adresi kullanılır. 
> `git config --global user.name kullanici_adi`
> `git config --global user.email email@itu.edu.tr`



<br>

#### git init
Bu komut kullanılarak bulunulan dizin boş bir git repository’si haline getirilir ve .git isimli bir dizin oluşturulur.
> `git init`


<br>

#### git clone
Bu komut var olan bir Git repository’sinin kopyalanması için kullanılır. Git clone komutu ile öncelikle yerel bir repository işaret edilerek bu repository’nin bir kopyası, yeni bir dizine kopyalanır. Orijinal repository lokalde olabileceği gibi uzak bir cihazda yer alıyor da olabilir.
> `git clone URL`


<br>

#### git add 
Bu komut kullanılarak işaret edilen dosya veya tüm proje, çalışılan dizine eklenir. 
> `git add`

<br>

#### git commit 
Bu komut kullanılarak çalışılan dizinde bulunan dosyalar paketlenerek .git klasörü içindeki head isimli kısıma eklenir. Daha sonra gelen pencerede bir commit mesajı girilir.
git commit 

>`git commit`

<br>


#### git status 
Bu komut kullanılarak üzerinde çalışılan Repository’nin o anki durumu görüntülenir. Üzerinde değişiklik yapılan dosyalar, yeni eklenmiş dosyalar ve commit komutu uygulanmamış dosyalar konsol üzerinde listelenir.
>`git status`

<br>


#### git checkout –b
Bu komut kullanılarak yeni bir branch oluşturulur ve o branch üzerine geçilir.
>`git checkout -b yeni_branch`

<br>


#### git checkout
Bu komut kullanılarak üzerinde çalışılan branch’dan bir başka branch’a geçilir.
>`git checkout`

<br>


#### git branch
Bu komut kullanılarak repository’deki tüm branch’lar listelenir ve üzerinde olunan branch görüntülenir.
>`git branch`

<br>


#### git branch –d
Bu komut kullanılarak işaret edilen branch silinir.

`git branch -d diger_branch`

<br>


#### git pull
Bu komut kullanılarak uzak bir repository’deki değişiklikler üzerinde çalışılan dizine getirilir ve bu dizin ile birleştirilir.

>`git pull` 

<br>


#### git merge
Bu komut kullanılarak farklı bir branch, üzerinde çalışılan branch ile birleştirilir.

>`git merge diger_branch`

<br>


#### git diff
Bu komut temel dosya ile olan farklılıkları gösterir.Bu komut, git diff **<"kaynak branch">** **<"hedef branch">** şeklinde kulanıldığında işaret edilen iki branch arasındaki farklar görüntülenir.

>`git diff` 

<br>



#### git log
Bu komut kullanılarak proje üzerindeki kayıt geçmişi en son kayıt en üstte olacak şekilde ters kronolojik sıra ile görüntülenir. Her kayıt, o kaydı alan kişinin adı, adresi, kayıt tarihi ve kayıt mesajı ile birlikte görüntülenir.

> `git log` 

<br>

#### git log --oneline
Bu komut kullanılarak sadece commit ID’lerinin ilk 7 karakteri ve hemen yanında commit mesajı olacak şekilde kayıt geçmişi daha temiz bir şekilde görüntülenir ve proje üzerinde yapılmış değişiklikler hakkında daha kolay bilgi edinilir.

> `git log --oneline`

<br>


#### git rebase -i
Bir proje üzerinde uzun süre çalışılıp çok fazla değişiklik commit edildiğinde commit tarihçesi çok uzun ve karmaşık görünür. Oysa ki yapılan değişiklikler tek commit mesajı ile de açıklanabilir ve böylece projeyi inceleyen kişiler proje üzerinde yapılan değişiklikleri kısa ve öz biçimde görebilirler. Bir proje üzerinde alınan birden fazla commit, git log komutu ile görüntülenmek istendiğinde kayıt alan kişilerin ismi, adresi, kayıt tarihi ve commit mesajı ile birlikte aşağıdaki gibi görünecektir.  Tüm bu değişiklikleri tek bir commit mesajı ile belirtmek ve kayıt tarihçesini daha anlaşılır kılmak için git rebase -i HEAD komutu ile işleme başlanır. Bu komutta HEAD kelimesi branch’in en uç noktasını temsil eder ve onun yanına eklenecek sayı ile kaç commit kadar geriye gidileceği belirtilir.

> `git rebase -i` 

<br>
<br>

<h3 id="branch-commit-format"></h3>

### Branch ve Commit Mesaj Formatı
<br>

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

<h3 id="pull-request"></h3>

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


<h3 id="rebase-conflict"></h3>

### Rebase ve Conflict Nedir?

#### Rebase 

Git’de merge ve rebase komutları benzer işlevleri yerine getirmek için kullanılıyor. Her iki komut da bir daldaki değişiklikleri başka bir dala birleştirmek için kullanılır. Ancak bu iki komut arasında proje tarihçesinin oluşturulması ile ilgili ciddi bir farklılık vardır.

Merge komutu ile A dalındaki değişiklikler B dalı ile birleştirildiğinde B dalının commit tarihçesinde merge işleminden kaynaklanan ve merge commit adı verilen otomatik oluşturulmuş bir commit yer alır. Bu commit A ve B dallarının tarihçelerini birbiri ile ilişkilendirir.

**rebase** komutu kullandığımızda ise ile A dalındaki her bir commit B dalına sanki commit işlemi B dalında yapılmış gibi yeniden yazılır. Bu sayede B dalının commit tarihçesi sanki tüm değişiklikler bu dalda olmuş gibi düz ve kesintisiz görünür.

##### Rebase'i ne zaman kullanmalıyız?

Rebase komutu yerel ve kısa süreliğine (örneğin bir hata giderme veya deneysel bir çalışma için oluşturulan) geçerli dallar için kullanılmalı. Paylaşılan depolarda rebase komutunu kullanmamanızı tavsiye ediyorum, çünkü rebase sonrasında projenizin ana dallarında değişikliklerin nereden kaynaklandığına dair bir bilgi veya ipucu göremezsiniz. Bu durum takım çalışmasını olumsuz yönde etkiler.

#### Conflict

Merhabalar, geçenki dersimizde git ile iki dalı birleştirmeyi, git merge komutunu görmüştük. Bu dersimizde ise merge işleminden kaynaklanan conflict yani çakışmaları görüp bu çakışmanın nasıl çözüleceğini göreceğiz.

Bir versiyon kontrol sistemi kullandığınızda yaşayacağınız en büyük problem çakışmalardır. Bu çakışmalar yaptığınız geliştirmeye bağlı olarak bazen basitçe çözebilir bazen de saatlerce zamanınızı alabilir. Hatta ekip içinde tatsızlıklara bile sebep olabilir.

### Rebase Nasıl Yapılır ?


1. Master branch üzerinden pull yapılır.
2. Master branch üzerinden **git checkout -b branch_ismi** komutu ile yeni bir branch oluşturulur.
3. Oluşturulan branch üzerinde geliştirmeler ya da iyileştirmeler yapılır. 
4. Yapılan değişiklerin ardından **git add .** komutu ile Repositories'e dosyaları ekleriz.
5. Yapılan değişiklikleri **git commit -m "Yapılan değişiklikler** komutu ile veri tabanına işlenir.
6. **git push origin branch_ismi** komutu ile pull request için yollanır.
7. **Github** üzerinden pull request açmadan önce, açılan branch üzerinden **git rebase master** komutu yapılır. Bu sayede **merge** komutunu kullanmadan ve commit işlemlerinin sırası bozulmadan birleştirme yapılır. 
8. Eğer **rebase** komutundan sonra hata almadıysanız, **Github** üzerinden PR açabilirsiniz.

#### Rebase Yaparken Conflict Hatası Alırsanız Ne Yapmalısınız?

Ekran çıktımızda bu hatayı aldıysak,

```
Auto-merging story.txt
CONFLICT (content): Merge conflict in story.txt
Automatic merge failed; fix conflicts and then commit the result.
```
Değişiklik yaptığımız dosyaya baktığımızda **<<<<<<< HEAD** yazan bir satır görürüz. Yine aynı şekilde paragrafın sonunda **=======** bir satır daha var. **HEAD** burada bulunduğumuz branch'in yani masterın son commitini ifade eder. Çakışmayı (Conflict)düzeltelim,

1. Hatanın ardadından yapılmış değişikliklerden hangilerinin doğru olduğunu siz belirleyeceksiniz. Yanlış olduğunu düşündüğünüz satırları sileceksiniz. 
2. **git add .** komutu ile  Repo'ya ekleriz.
3. **git commit -m "Conflict Giderildi"** komutunu kullnarak istenilen veriye işleme işlemi gerçekleştirilir.
4. **git push origin branch_ismi** komutu ile tekrardan yollanır.
5. PR açılabilirsiniz.







