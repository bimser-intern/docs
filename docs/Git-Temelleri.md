## Git Komutları ve Kullanımı

Günümüzde ortak projeler geliştirmek, açık kaynaklı kişisel kod geliştirmek için bir çok kişi GİT tercih ediyor. Bu kaynak kontrol aracı ile geliştirilen projeler host edilmesi için GitHub, GitLab platformlarıda oldukça popüler olarak kullanılmaktadır.
2 Sebepten dolayı kaynak kontrol sistemine ihtiyaç duyarız;

* Kaynak kodunuzun değişimlerini takip etmek ve bunu yönetebilmek
* Birlikte kod geliştirmek.


1. [Git init](#git-init)
2. [Git veri akışı](#git-veri-akışı)
3. [Untracked Files](#untracked-files-i̇zleri-oluşturulmamış-dosyalar)
4. [Staging Taşıma](#staging-taşıma)
5. [Local Dosyaları Değiştirmek](#local-kendi-çalışma-ortamınızdaki-dosyaları-değiştirmek)
6. [Commit](#commit-save-to-local-repo)
7. [Push](#pushsave-to-remote-repo)

![image](https://miro.medium.com/max/875/1*OaiXIVZeRMDc4YFXb_wUfQ.png)

# Git init

<br>

Bir klasör oluşturup içerisinde git init fonksiyonu çalıştırdığımızda .git altında ufak bir dosya yönetim sistemi oluşturduğunu görebilirsiniz.

* > `git init `  

Bu klasörün içerisinde dosyalarınızın state(versiyonlarını) tutacaktır.
* Bu dosyalar arasındaki farklar,
* commit sırasındaki kesitler
hepsi bu dosyalar içerisinde tutulmaktadır.



# Git veri akışı

<br>

![image](https://miro.medium.com/max/500/1*ZNPtH5cPV0yLXqbmAOU8kQ.png)



# Untracked Files (İzleri oluşturulmamış dosyalar)

<br>

* > `git status ` komutu ile izi oluşmamış dosyaları görebilirsiniz.  

![image](https://i.ytimg.com/vi/wdT8_yQkruc/maxresdefault.jpg)


#  Staging Taşıma

* > `git add ` komutu ile izi oluşmamış dosyaları Staging alanına geçirmiş oluruz.

![image](https://miro.medium.com/max/579/1*k2ar0H4JMVxye5qnIU97RA.png)

İstediğiniz dosyayı Staging Alanından çıkarmak için

* > `git reset HEAD <filename> ` komutunu kullanmanız yeterlidir.



# Local (Kendi Çalışma Ortamınızdaki) Dosyaları Değiştirmek

Çalışma yaptığınız klasör altındaki dosya durumları hakkında aşağıdaki komutları çalıştırarak değişiklikleri görebiliriz.

* > `git status` dosyanın local tarafta modified olduğunu görebiliriz.
* > `git diff` dosyada hangi alanların değiştiğini görebiliriz.
* > `git checkout --filename ` ile yaptığınız değişikliği geriye alabilirsiniz.

Git checkout komutunun veri akışına etkisi böyledir.

![image](https://static.javatpoint.com/tutorial/git/images/git-checkout.png)



#  Commit (Save to Local Repo)

* > `git commit -m 'info' `komutu ile dosyalarınızı Local Repo’nuzda kaydedin..

![image](https://static.javatpoint.com/tutorial/git/images/git-commit4.png)


# Push (Save to Remote Repo)

* > `git push origin master ` komutu ile uzaktaki repo üzerine kayıt yapabilirsiniz.

![image](https://assets-global.website-files.com/61c02e339c11997e6926e3d9/61c2e47b4d436d4d1a382d76_5e2a1539b3437be8c9018c2f_cover-git-push-force2.png)
