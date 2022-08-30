# İçerik

1. [Git Branch Nedir?](#git-branch-nedir)
2. [Merge](#merge)
3. [Fast Forward](#fast-forward)
4. [Merge Conflict](#merge-conflict)
5. [Stash](#stash)
6. [Pop](#pop)
7. [Checkout](#checkout)
8. [Reset](#reset)
9. [Revert](#revert)
10. [Diff](#diff)
11. [Rebase](#rebase)
12. [Sunum Dosyası](#sunum-dosyası)
13. [Kaynakça](#kaynakça)

# Git Branch Nedir?

Git branch, bir projede birden çok sürümü organize etmemize yardımcı olur. 

* > `git branch`   
Repositorydeki tüm branchleri listeler.

* > `git branch (branchname)`  
(branchname) adında yeni bir branch oluşturur.

* > `git switch (branchname) `   
Branchler arası geçiş yapmamızı sağlar.

* > `git checkout (branchname)` 
Branchler arası geçiş yapmamızı sağlar.

* > `git checkout –b (branchname)` 
Branch oluşturur ve direkt o branch e geçiş yapar.


# Merge 

Bir branchi başka bir branche bağlama işlemine denir.

>`git merge `
Komutu ile yapılır.

# Fast Forward

Bazı durumlarda branch'lerden bir tanesinde herhangi bir değişiklik yapılmamıştır ve bu branch'in ortak commit'i ve son commit'i aynıdır. Bu durumda merge işlemi çok basitleşir ve git diğer branch'in tüm commit'lerini ortak commit'in üzerine ekleyerek merge işlemini yapar. Bu özel duruma Git terminolojisinde "Fast-Forward Merge" denir ve her iki branch'in tarihçesi de ortaktır

# Merge Conflict

* Bir versiyon kontrol sistemi kullandığınızda yaşayacağınız en büyük problem çakışmalardır.
* Çakışma aslında çok basit bir şekilde karşımıza çıkabilir. İki kişi aynı dosyayı ve aynı satırı değiştirirse ve git otomatik olarak merge edemezse bu durumda conflict yani çakışma olacaktır. Bu durumda çakışma yaşayan kişi ,ekipteki diğer kişi ile beraber oturup çakışmayı çözdükten sonra merge işlemine devam etmelidir.

# Stash

Bazen Commit işlemi yaptıktan sonra yüzlerce satır komut yazarsınız. Sonra birden yazdığınız kodlardan önceki versiyon üzerinde değişiklik yapmanız gerekebilir. Bu durumda bu yazdığınız komutları bir yere saklamanız gerekir. İşte bu gibi durumlarda git stash kullanmamız gerekir.

>`git stash`

komutu ile sağlanır.

# Pop

`git stash pop` komutu ile listenin en üstünde yer alan değişiklik geri yüklenecek ve bu değişiklik listeden silinecek.

# Checkout

>`git checkout` komutu branch'ler arasında geçiş yapmak için kullanılır.

# Reset

>`git reset "commithash"` komutu ile önceki commitlere geri dönebiliriz. "commithash", dönmek istediğimiz commitin hash kodudur. Döndüğümüz committen sonraki değişikler artık görünmez ancak silinmez de. İstediğimizde bu commitleri geri alabiliriz.

>`git reset --hard "commithash"` komutu ise döndüğümüz committen sonraki değişikleri tamamen siler.

# Revert

>`git revert "commithash"` komutu geri almak istediğimiz commit için yeni bir commit ekler. Bu yeni eklenen commit "commithash" hash kodlu commit içeriğine sahip olur. 

# Diff

>`git diff <"kaynak branch"> <"hedef branch">` komutu iki branch arasındaki farkları gösterir. Commit hash kodları kullanılarak iki commit arasındaki farklar da görülebilir. `git diff` olarak kullanıldığında mevcut çalışma dosyası içindeki değişikleri gösterir.

# Rebase 

>`git rebase` komutunu commit kalabalığı oluşmuş branchleri sadeleştirmek için kullanırız. Merge işlemine benzer ancak rebase yapıldığında commitlerin kronolojik sırası kaybolur.

# Sunum Dosyası

[Git Branch Sunumu](https://drive.google.com/file/d/1wcX0y-HYyKV9QG_tGR_VLqwbHUv41P3X/view?usp=sharing)

[Git Branch Komutlar Sunumu](https://drive.google.com/file/d/1Ca64nJTjPvDuZ89SIDCj9OneEDTvtb7L/view)

# Kaynakça

* [BTK Akademi Atıl Samancıoğlu Git&Github Kullanımı Kursu](https://www.btkakademi.gov.tr/portal/course/versiyon-kontrolleri-git-ve-github-19439)

* [Git Branch Tutorial](https://www.atlassian.com/git/tutorials/using-branches#:~:text=The%20git%20branch%20command%20lets,checkout%20and%20git%20merge%20commands.)

* [Git Branch Documentation](https://git-scm.com/docs/git-branch)


