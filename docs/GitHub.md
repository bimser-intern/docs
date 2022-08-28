İçindekiler

---

- [GitHub Nedir ve Neden GitHub?](#github-nedir-ve-neden-github)
- [Yeni Repository Oluşturma](#yeni-repository-oluşturma)
- [Repository Sayfası](#repository-sayfası)
- [Label Tipleri](#label-tipleri)
- [Yeni Issue Açma](#yeni-issue-açma)
- [Yeni Branch Açma](#yeni-branch-açma)
- [Branch'de Değişiklik Yapmak](#branchde-değişiklik-yapmak)
- [Açılan Branchdeki Değişikliği Mergeleme](#açılan-branchdeki-değişikliği-mergeleme)
- [Yeni Organizasyon Oluşturma](#yeni-organizasyon-oluşturma)
- [Sunum Dosyası](#sunum-dosyası)
   

<br /><br />

# GitHub Nedir ve Neden GitHub?

GitHub, sürüm kontrolü ve işbirliği için bir kod barındırma platformudur. Sizin ve diğer takım arkadaşlarınızın projeler üzerinde her yerden birlikte çalışmasına olanak tanır.

GitHub'ın kalbinde Git adı verilen açık kaynaklı bir sürüm kontrol sistemi (VCS) bulunur. Git, bilgisayarınızda yerel olarak gerçekleşen GitHub ile ilgili her şeyden sorumludur.

-  Kolay Proje Yönetimi
- Paketlerle Arttırılmış Güvenlik
- Etkili Ekip Yönetimi
- Geliştirilmiş Kod Yazma
- Artırılmış Kod Güvenliği
- Kolay Kod Barındırma

<br />

 # Yeni Repository Oluşturma

GitHub ana sayfanızda bu iki butondan birine tıkladığınızda repository oluşturma sayfasına yönlendirileceksiniz.

![Yeni Repository](https://user-images.githubusercontent.com/65497602/186836532-2b9c5dec-49ed-44d9-8c13-ad45601dd6ee.PNG)

![image](https://user-images.githubusercontent.com/65497602/186837515-68b43051-fea2-4aba-a60f-825b454106b4.png)

- Her Repository’nin unique bir ismi olması lazım yani hesabınızda iki tane aynı isimle repo bulunmaz.

- Description kısmında kısaca repositorynizden bahsedebilirsiniz.

- Repo’nun public mi private mı olduğuna burdan karar veriyoruz. Private olursa izin vermediğimiz kimse erişemez repoya. Publicde ise isteyen herkes kodumuzu görüp katkıda bulunabilir.

- Readme dosyası repomuzu ve projemizi uzunca tanıtmamız için var. Eklemek zounlu değil.

- .gitignore dosyası projemizin kök dizinine oluşturulan düz bir metin dosyasıdır. Local çalışma alanındaki takip edilmesini istemediğin, takım arkadaşların için gerekmeyen dosyaların varsa veya bu dosyaların boyutu reponuza atmanıza gerek olmayacak kadar büyük ölçekli ise kullanılıyor.

- Lisans seçimi reponuza gelen insanların projenizle neler yapıp yapmayacağına karar veriyor.

 # Repository Sayfası



Repository’mizi açtığımızda karşımıza bu ekran geliyor. Bu ekranda ki butonların amaçlarına bakalım.

![image](https://user-images.githubusercontent.com/65497602/186837845-2586255d-53b9-4260-a956-2c7989b8d35f.png)


- <ins>Issues:</ins> Yapılacak işleri, bugları, özellik isteklerini ve daha fazlasını izlemek için kullanılır. Çok issue oluşturacağımızı düşünürsek, bunları belirli etiketlere koyarsak ulaşmamız daha kolay olur. 


 ![image](https://user-images.githubusercontent.com/65497602/186838403-56978850-3a93-4b86-b19a-f8e94b54c185.png)

Her projede belirli etiketler vardır, ekstra olarak kendimiz Labels kısmından ekleme yapabiliriz

Arama butonu aşağıdaki gibiyken açık olan issueları getirmesi için koşullanıyor.

Milestone , issue’lar koymak için oluşturulan bir kap gibi düşünülebilir. Belirli özellikleri ya da proje fazlarını issue’larla ilişkilendirmek için yararlı bir yöntemdir. Örneğin; projenin versiyon 1.0'ı için şu issue’lar yapılacak, versiyon 2.0 için ise başka issue’lar gibi.


- <ins>Pull Request:</ins> GitHub'daki bir repodaki bir branch’e gönderdiğiniz değişiklikleri başkalarına bildirmenize olanak tanır. Bir pull request açıldıktan sonra, olası değişiklikleri ortak çalışanlarla tartışabilir, gözden geçirebilir ve değişiklikleriniz master branch’de birleştirilmeden önce takip commitlerinizi ekleyebilirsiniz.

- <ins>Actions:</ins> Derleme, test ve dağıtım işlem hattınızı otomatikleştirmenize olanak tanıyan bir sürekli entegrasyon ve sürekli teslim (CI/CD) platformudur. Deponuza yönelik her pull requesti oluşturan ve test eden iş akışları oluşturabilir veya birleştirilmiş pull requestleri üretime dağıtabilirsiniz.
Wikis: Projenizin yol haritasını çıkarmak, mevcut durumu göstermek ve yazılımı daha iyi belgelemek için havuzunuzda bir yer sağlar.

- <ins>Security:</ins> Topluluğunuzun, projeniz için güvenlik açıklarını nasıl güvenli bir şekilde rapor edeceğini anlamasına yardımcı olup yeni güvenlik politikaları oluşturmak için kullanılır.
  
- <ins>Commit:</ins> Küçük anlamlı değişiklik gruplarını commit olarak kaydedebilirsiniz. Onaylanan pull requestler commit olur.

- <ins>Insights:</ins> Git Insights, yazılım projeleriniz ve ekipleriniz hakkında size bilgi veren bir analiz aracıdır. Verileri 3. taraf hizmetlere göndermeden tüm commitlerinizi, pull requestlerinizi,sorunlarınızı toplayabilir ve analiz edebilirsiniz.
  
- <ins>Settings:</ins> Repository kurumu yapıldıktan sonra gerçekleştirilen her şeyi değiştirip, ayarlarıyla oynayacağınız ya da silebileceğiniz kısım.
  
- <ins>Branch:</ins> Dallar, deponuzun kapalı bir alanında özellikler geliştirmenize, hataları düzeltmenize veya yeni fikirleri güvenle denemenize olanak tanır. Her zaman mevcut bir şubeden bir şube oluşturursunuz. Tipik olarak, deponuzun varsayılan dalından yeni bir dal oluşturabilirsiniz.
  
- <ins>Fork:</ins> Yönettiğiniz bir reponun kopyasıdır. Çatallar, orijinal repoyu etkilemeden bir projede değişiklik yapmanızı sağlar. Çekme istekleriyle orijinal depodan güncellemeleri alabilir veya değişiklikleri gönderebilirsiniz.
  
- <ins>Gist:</ins> Snippet'leri veya veri alıntılarını başkalarıyla paylaşmak için kolay bir yöntemdir. Bir öz, bir kod dizisi, bir bash betiği veya başka bir küçük veri parçası olabilir. Bu bilgi parçaları GitHub tarafından bir depo olarak barındırılır.
  
- <ins>Organization:</ins> İşletmelerin ve açık kaynak projelerinin aynı anda birçok projede, gelişmiş güvenlik ve yönetim özellikleriyle işbirliği yapabileceği paylaşılan hesaplardır.


<br /><br />

# Label Tipleri 


<img style="float: right;" src="https://user-images.githubusercontent.com/65497602/186839779-bbf0b20f-9a2e-4287-8f33-29c9ddad6f21.PNG" width="110">

- Bug: Beklenmeyen bir sorunu veya istenmeyen davranışı gösterir.
  
- Documentation: Belgelerde iyileştirmeler veya eklemeler yapılması gerektiğini belirtir.
  
- Duplicate: Benzer sorunları, pull requestleri veya tartışmaları gösterir

- Enhancement: Yeni özellik veya istekleri gösterir.
  
- Help Wanted: Bir bakıcının bir sorun veya çekme isteği hakkında yardım istediğini belirtir

- Invalid: Bir bakıcının bir sorun veya çekme isteği hakkında yardım istediğini belirtir
  
- Question: Bir sorun, çekme isteği veya tartışmanın daha fazla bilgiye ihtiyacı olduğunu gösterir
  
- Wontfix: Bir sorun, çekme isteği veya tartışma üzerinde çalışmanın devam etmeyeceğini belirtir


<br /><br />


# Yeni Issue Açma


Issues kısmından New Issue’ya tıkladığımızda bu sayfa karşımıza çıkar ve burdan issue’yu submitleyebiliriz.

![image](https://user-images.githubusercontent.com/65497602/186843706-f9854c00-ce60-4cad-99a4-44546abe2ce9.png)

<br />
Açılan Tüm Issuelar’ı görmek için de filtreleri kaldırabiliriz.

<br />

![image](https://user-images.githubusercontent.com/65497602/186844254-d41417c0-9969-491f-b507-03a2897889b3.png)


<br/>

# Yeni Branch Açma


Repositorymizin ana sayfasına geldiğimizde işaretlediğim butona tıklayıp branchlerimizi görebiliyoruz.

![image](https://user-images.githubusercontent.com/65497602/186844780-4b34a765-f999-4b05-bbf8-879fa555fc60.png)

Butone tıkladıktan sonra karşımıza çıkan ekranda ise yeşil butona tıklayıp yeni branchimizi açabiliyoruz.


![image](https://user-images.githubusercontent.com/65497602/186844881-b1aa08f4-4d85-4a06-a02e-d43cc4c0cb73.png)

<br/><br/>

# Branch'de Değişiklik Yapmak


Alt branchimize gelip kırmızı kutucuktaki düzenle seçeneğine tıklayıp değişiklik yapabiliyoruz.

Daha sonra ise bu değişikliği ya bir alt branche kaydırıp ya da direk bu branche commitleyebiliyoruz. Bu zaten alt branchimiz olduğu için direk commitleyebiliriz. 

![image](https://user-images.githubusercontent.com/65497602/186845051-39985ec8-d81d-42c6-9336-2afe36271c90.png)

![image](https://user-images.githubusercontent.com/65497602/186845335-0c409dca-9b5e-4193-a400-143716ffd344.png)

<br/><br/>

# Açılan Branchdeki Değişikliği Mergeleme 


Alt branchdeki iş tamamlandığında pull request ile bir üstteki branchle mergelenir. Depoya anında erişime sahip olan herkes birleştirme işlemini tamamlayabilir. 

Yeni bir pull requestle bu branchin mergelenmesi için istek göndeririz. Yetkili kişi bunu onaylarsa merge gerçekleşir.

![image](https://user-images.githubusercontent.com/65497602/186845713-483fb8d5-ea41-47e0-a759-899005d76849.png)

İşlem tamamlandıktan sonra alt branch istenilirse silinebilir.

![image](https://user-images.githubusercontent.com/65497602/186845781-89d216aa-85fe-476f-bc7f-616926a65f66.png)

<br/><br/>

# Yeni Organizasyon Oluşturma 


Yine GitHub’ın her yerinden ulaşılabilen butondan yeni organizasyon oluştura tıklıyoruz.

Karşımıza çıkan planlardan free olanı seçiyoruz.


<img style="float: left;" src="https://user-images.githubusercontent.com/65497602/186846113-9264d8f2-3516-48d2-973c-05a87fce69db.png" width="200">

<img style="float: right;" src="https://user-images.githubusercontent.com/65497602/186846236-e9e95794-a9e6-49a6-832b-efbcb94abccd.png" width="260">

<br/><br/><br/><br/><br/><br/><br/><br/>
<br/><br/><br/><br/><br/><br/><br/><br/>
<br/><br/><br/>
- Gerekli boşlukları doldurup seçimleri yaptıktan sonra eğer davet edilecek kişiler varsa davet gönderiliyor

- Daha sonra organizasyonunuz hakkında bilgileri girip submitledikten sonra organizasyonumuz oluşmuş oluyor.

<br/>

<img  src="https://user-images.githubusercontent.com/65497602/186847385-d0612b74-0922-409a-8879-84db58624ed5.png" width="300"></p>

<img style="float: left;" src="https://user-images.githubusercontent.com/65497602/186847462-e10abc18-f42e-495b-b180-ce33bf021502.png" width="300">

<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

# Sunum Dosyası 

[GitHub Sunum Dosyası](https://github.com/bimser-intern/docs/files/9430945/GitHub.pptx)
