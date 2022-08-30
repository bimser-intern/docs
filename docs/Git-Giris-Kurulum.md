# Git Giriş Ve Kurulumu

## İçindekiler:

1. [Git Versiyon kontrol sistemi](#git-versiyon-kontrol)
2. [Git Nedir](#git-nedir)
3. [Git'in Versiyonlama Mantığı](#git-mantık)
4. [Git Kurulum Aşamaları](#git-kurulum)

<h3 id="git-versiyon-kontrol"></h3>

# Git Versiyon Kontrol Sistemi

Düşünün bir yazılım takımınız var ve bir projeye başladınız. Projeyi modüllere ayırdınız ve her kişiye ilgili görevi atandı. Takım halinde çalışabilmeniz için bir yönetim aracı gerekli ve bir kitabın baskıları gibi bir baskı da hata çıktığı zaman hemen versiyonu değiştirip eski haline getirmeniz lazım. Burada imdadınıza (birçok iş ilanında da gördüğünüz üzere) git koşuyor. En büyük avantajlarından birisi ise merkezi yapıda bulunmamasıdır. (Dağıtık Sistem)

 <h3 id="git-nedir"></h3>

### Git Nedir?

Git, kısa süre içerisinde yazılımcıların vazgeçilmezleri arasına giren bir sürüm/versiyon kontrol sistemidir. Yazdığımız projeleri, bilgisayarımızda ya da harici disklerde binbir tehlike altında değilde internet üzerinde tutmamızı ve yönetmemizi sağlayan bir sistemdir.

<h3 id="git-mantık"></h3>

### Git'in Versiyonlama Mantığı

Az önce dağıtık yapıda bulunur dedik. Ne demek bu şimdi ?

Git ile versiyonladığınız proje dosyaları her geliştirici de saklanır. Ve proje de bir değişiklik yapıldığı zaman sadece değişen kısım değil o an projeden bir snapshot alınır (projeyi bir bütün halinde saklar) ve böylelikle yapılan katkı bir bütün halinde kolaylıkla görülmüş olur.

<h3 id="git-kurulum"></h3>

### Git Kurulum Aşamaları

Windows'a kurulum için gerekli dosyayı resmi web sayfasından indirmemiz gerekiyor.
Bunun için `https://git-scm.com/downloads` adresine tıklıyoruz.

![git-site](https://1.bp.blogspot.com/-PcOj171mmEE/XnGpJQd_obI/AAAAAAAAHoE/-wTtwvyT7GMGtSY9DDbPANU1b0Jy77psACLcBGAsYHQ/s640/git-windows-setup-01.png)

<br>

Açılan sayfa da göreceğiniz üzere sadece Windows için değil, diğer işletim sistemleri içinde kurulum dosyalarının mevcut olduğunu görebilirsiniz. Lakin diğer başlıkları incelediğiniz de buna pek gerek olmadığını fark edeceksiniz.
Şimdi sağ tarafta işletim sistemimize uygun kurulum dosyasını indirmek için "Download 2.25.1 for Windows" butonuna indirme işlemini başlatıyoruz.

<br>

![git-site2](https://1.bp.blogspot.com/-LkzHjSK78Ck/XnGpJY9A5TI/AAAAAAAAHoA/0s7ubsy38XkmCm2tljPx8PuONkXlt4MdgCLcBGAsYHQ/s1600/git-windows-setup-02.png)

İndirme işlemi otomatik başlaması gerekiyor. Aksi halde "Click here to download manually" linkine tıklayarak dosyayı indirmeye başlayabilirsiniz. Bu aşamada programın başarılı bir şekilde indirilmesini bekliyoruz. İndirme işlemi tamamlandığında programı çalıştırmanız gerekiyor.
<br>

![git-site3](https://1.bp.blogspot.com/-ZYB5h6MNRk0/XnGpIyaU0CI/AAAAAAAAHn8/RVplTCX2cGw2K-PIe9yh3ufvl-Ld-byQwCLcBGAsYHQ/s1600/git-windows-setup-03.png)
<br>

Kullanıcı hesab denetimi ayarlarınız açık ise karşınıza böyle bir pencere gelecektir. Bu aşama da işlemin tarafımızdan gerçekleştirildiğini onaylamamız gerekiyor. "Evet" seçeneğini seçerek işleme izin veriyoruz.
<br>

![git-site4](https://1.bp.blogspot.com/-Dbzp9PHKNBU/XnGpJhoIOyI/AAAAAAAAHoI/SeaNL1kiAF87tN8Vyhcm3z0HUzPZQGlBgCLcBGAsYHQ/s400/git-windows-setup-04.png)

Kurulumun ilk aşamasında bizi "GNU General Public License" lisansı karşılamaktadır. "Next" butonuna tıklayarak bir sonra ki aşamaya geçiyoruz.

![git-site5](https://1.bp.blogspot.com/-1VQ_J4Sa9Gw/XnGpKOOtrMI/AAAAAAAAHoM/xorby-STfbgtGKoE90jMXQvC0J75VcW1ACLcBGAsYHQ/s400/git-windows-setup-05.png)

Bu aşamada Git'in kurulacağı dizini belirtmemiz gerekiyor. Eğer farklı bir dizin seçmeyecek seniz, "Next" butonu ile bir sonra ki aşamaya geçiyoruz.

![git-site6](https://1.bp.blogspot.com/-RcPQrORH8-8/XnGpKegi1DI/AAAAAAAAHoQ/sJq8IuCFquUskhelLjVX6TplnYllXPoPACLcBGAsYHQ/s400/git-windows-setup-06.png)

Bu aşamada kurmak istediğiniz ekstra bileşenler varsa bu aşamada seçiyoruz. Bu aşamayı da "Next" butonu ile geçiyoruz.

![git-site7](https://1.bp.blogspot.com/-0RJncDfd9Y0/XnGpKkQbXGI/AAAAAAAAHoU/rnW1hYuvVOwRaJbFjmIUe9YykzpQw6NXwCLcBGAsYHQ/s400/git-windows-setup-07.png)

Bu aşama da başlat menüsünde kısa yollarının oluşturulması için gerekli dizini belirtmemizi istiyor. Değiştirmek istemiyorsak, sonra ki aşamaya geçiyoruz.

![git-site8](https://1.bp.blogspot.com/-fZ9FkuGDmh0/XnGpK8Ee83I/AAAAAAAAHoY/hyVbOJXvrv8T7AR60KrU91GmBdUZdYv9QCLcBGAsYHQ/s400/git-windows-setup-08.png)

Varsayılan olarak kullandığımız bir editör varsa, burada belirtmemiz gerekiyor. Ben varsayılan olarak Visual Studio Code kullandığımdan "Use Visual Studio Code as Git's default editor" seçeneğini seçtim. Eğer bu seçimi yaptıysanız, sonra ki aşamaya geçelim.

![git-site9](https://1.bp.blogspot.com/-0jwIuJx8kHA/XnGpLB6eERI/AAAAAAAAHoc/iC24b6H5dAYYKozGG1NCcA1UWQjKHkC7ACLcBGAsYHQ/s400/git-windows-setup-09.png)

Burada Git'in kullanımı nasıl gerçekleştireceğimizi belirliyoruz. Önerilen "Git from the command line and also from 3rd-party software" seçeneğidir. Bu seçenek sayesinde "Git Bash" programını kullanabildiğimiz gibi "Cmd" (komut istem) penceresi ile Git komutlarını kullanabiliriz. Bunun için Git dizinin ortam değişkenlerine eklenmesi gerekiyor.

![git-site10](https://1.bp.blogspot.com/-T3G5oOGhvrA/XnGpLa3h7_I/AAAAAAAAHog/-nUANLb1GCYaRjjTA74rN30l3jTkGDzvQCLcBGAsYHQ/s400/git-windows-setup-10.png)

Bu aşamada ise bağlantı sağlayacağımız yöntemi seçmemiz gerekiyor.

![git-site11](https://1.bp.blogspot.com/-DQKcKtr1mTs/XnGpLkSz6rI/AAAAAAAAHok/qxn-RMOyB5kFnnyYQXpHpll5LWdx88ojQCLcBGAsYHQ/s400/git-windows-setup-11.png)

Bu aşamada satır sonu stilini seçmemiz lazım. İşletim sistemine göre bu stil değişebileceğinden seçim yapmamız isteniyor. Lakin varsayılan seçenek işimizi görüyor.

![git-site12](https://1.bp.blogspot.com/-jKMLN3vYGuI/XnGpL8m9ikI/AAAAAAAAHoo/n4liUYJyhLY1kwNusVgBK6qmo7tqAELogCLcBGAsYHQ/s400/git-windows-setup-12.png)

Bu aşamada Git Bash'ın kullanacağı terminali belirtiyoruz. İsterseniz MinTTY gibi çok fonksiyonlu bir terminal kullanabilir veya klasik "Komut istemci-sini" kullanabilirsiniz.

![git-site13](https://1.bp.blogspot.com/-JlLXbbUl8-E/XnGpMD6_nfI/AAAAAAAAHos/NLtrc-rwRyM7xLhNtu2XTtfPi2oPCrE1ACLcBGAsYHQ/s400/git-windows-setup-13.png)

Burada Git kullanımıyla ilgili ekstra ayarlar bulunmaktadır. Varsayılan seçenekler ile "Install" butonuna basarak, kurulum işlemini başlatıyoruz.

![git-site14](https://1.bp.blogspot.com/-xutkf069C_0/XnGpMcL_kWI/AAAAAAAAHow/VUg9pMwnjqkk37rJXCX6ubOCxpSoXQ3XACLcBGAsYHQ/s400/git-windows-setup-14.png)

Biraz bekledikten sonra kurulum işlemi tamamlanacaktır.

![git-site15](https://1.bp.blogspot.com/-c5uxUpG7uhg/XnGpMWZrqvI/AAAAAAAAHo0/xroVB5vaWW8jbMDtBPaTcahUse9k5OZLQCLcBGAsYHQ/s400/git-windows-setup-15.png)

Kurulum işlemi başarıyla tamamlandı. Bundan sonra Git'in başarılı bir şekilde çalışıp, çalışmadığını kontrol etmemiz gerekiyor.

![git-site16](https://1.bp.blogspot.com/-5fstVklgvAM/XnGpNAiey5I/AAAAAAAAHo8/3vPtFITSmuYtthAJX9HKtAj2-dbWsD0oACLcBGAsYHQ/s400/git-windows-setup-16.png)

Bunun için "Başlat" menüsünden "Git Bash" kısayolunu bulup, çalıştırıyoruz.

![git-site17](https://1.bp.blogspot.com/-LPsRpfaUpvg/XnGpNGJ_vmI/AAAAAAAAHo4/O6yeDoCYnxo-mrBEpLjeAAYMVtKk4aA4ACLcBGAsYHQ/s640/git-windows-setup-17.png)

Açılan pencerede aşağıda ki komutu uyguluyoruz.

`git --version`

git version 2.25.1
Eğer Git sürümünü görüyorsanız, başarılı bir şekilde kurulum tamamlanmış demektir.

Örnek :
`git config --global user.name "Ali Han Pertek"`
`git config --global user.email "apertek1@gmail.com"`

Global ayarlara göz atalım:

git config --list --global

kayıtlı kullanıcı adı veya email'imizi unuttuysak

git config user.name
git config user.email
şeklinde görebiliriz.
