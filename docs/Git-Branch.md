# İçerik

1. [Git Branch Nedir?](#git-branch-nedir)
2. [Merge](#merge)
3. [Fast Forward](fast-forward)
4. [Merge Conflict](#merge-conflict)
5. [Stash](#stash)
6. [Pop](#pop)
7. [Sunum Dosyası](#sunum-dosyası)
8. [Kaynakça](#kaynakça)

# Git Branch Nedir?

Git branch, bir projede birden çok sürümü organize etmemize yardımcı olur. 

* git branch   Repositorydeki tüm branchleri listeler.
* git branch (branchname)  branchname adında yeni bir branch oluşturur.
* git switch (branchname)   branchler arası geçiş yapmamızı sağlar.
* git checkout (branchname) branchler arası geçiş yapmamızı sağlar.
* git checkout –b (branchname) branch oluşturur ve direkt o branch e geçiş yapar.


# Merge 

Bir branch i başka bir branche bağlama işlemine denir.
git merge komutu ile yapılır.

# Fast Forward

Bazı durumlarda branch'lerden bir tanesinde herhangi bir değişiklik yapılmamıştır ve bu branch'in ortak commit'i ve son commit'i aynıdır. Bu durumda merge işlemi çok basitleşir ve git diğer branch'in tüm commit'lerini ortak commit'in üzerine ekleyerek merge işlemini yapar. Bu özel duruma Git terminolojisinde "Fast-Forward Merge" denir ve her iki branch'in tarihçesi de ortaktır

# Merge Conflict

* Bir versiyon kontrol sistemi kullandığınızda yaşayacağınız en büyük problem çakışmalardır.
* Çakışma aslında çok basit bir şekilde karşımıza çıkabilir. İki kişi aynı dosyayı ve aynı satırı değiştirirse ve git otomatik olarak merge edemezse bu durumda conflict yani çakışma olacaktır. Bu durumda çakışma yaşayan kişi ,ekipteki diğer kişi ile beraber oturup çakışmayı çözdükten sonra merge işlemine devam etmelidir.

# Stash

Bazen Commit işlemi yaptıktan sonra yüzlerce satır komut yazarsınız. Sonra birden yazdığınız kodlardan önceki versiyon üzerinde değişiklik yapmanız gerekebilir. Bu durumda bu yazdığınız komutları bir yere saklamanız gerekir. İşte bu gibi durumlarda git stash kullanmamız gerekir.

> 'git stash' 

komutu ile sağlanır.

# Pop

git stash pop komutu ile listenin en üstünde yer alan değişiklik geri yüklenecek ve bu değişiklik listeden silinecek.

# Sunum Dosyası

[Git Branch Sunumu](https://drive.google.com/file/d/1wcX0y-HYyKV9QG_tGR_VLqwbHUv41P3X/view?usp=sharing)

# Kaynakça

* [BTK Akademi Atıl Samancıoğlu Git&Github Kullanımı Kursu](https://www.btkakademi.gov.tr/portal/course/versiyon-kontrolleri-git-ve-github-19439)

* [Git Branch Tutorial](https://www.atlassian.com/git/tutorials/using-branches#:~:text=The%20git%20branch%20command%20lets,checkout%20and%20git%20merge%20commands.)

* [Git Branch Documentation](https://git-scm.com/docs/git-branch)


