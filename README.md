# Markdown Nedir?

Günümüzde dijital ortamlarda makale, blog yazısı gibi metin diagramları oluştururken, metnin akışına uygun olarak başlık, liste ve tablo gibi görsel biçimler kullanırız. Günümüzde bu tarz içerikleri üretirken *HTML(Hyper Text Markup Language)* işaretleme dilini kullanırız. Fakat bir yazı için hem uğraştıcı olup hem de hataların oluşmasına neden olabilir. İşte bu zamanlarda işimizi kolaylaştıracak bir text to *HTML* yapısı ile dönüştürme aracı olan **Markdown** karşımıza çıkıyor.

## Markdown
John Gruber, Markdown dilini 2004 yılında Aaron Swartz ile sözdiziminde işbirliği yaparak oluşturdu, insanların okuma ve yazması kolay düz metin biçimini kullanarak isteğe bağlı olarak XHTML'ye veya HTML'e dönüştürme amacını taşıyordu.
	
Markdown, düz-metin-biçimlendirme sözdizimine sahip hafif bir işaretleme dili. Tasarımı, birçok çıktı biçimine dönüştürülmesine izin verir, ancak aynı ada sahip orijinal araç yalnızca HTML'yi destekler. Markdown genellikle BENİOKU (README) dosyalarını biçimlendirmek, çevrimiçi tartışma forumlarına mesaj yazmak ve düz metin düzenleyicisi kullanarak zengin metin oluşturmak için kullanılır. Markdown’un ilk tanımı belirsizlikler ve cevaplanmamış sorular içerdiğinden, yıllar boyunca ortaya çıkan uygulamaların ince farklılıkları vardır ve çoğu sözdizimi, dosya uzantılarıyla birlikte gelir.

## Markdown Elements

### Inline Examples 


#### Italic Text

`*Italic*` <br>					
*Italic*


#### Strong Text

`**Strong** Text` <br>					
**Strong** Text


#### Strikethrough

`~~Üstü Çizgili~~` <br>			
~~Üstü Çizgili~~


#### Links

`[Referans bir isim](https://www.gooogle.com)`	<br>	
[Referans bir isim](https://www.gooogle.com)


#### Auto Links

`Autolinks <https://www.gooogle.com>` <br>	
Autolinks <https://www.gooogle.com> 




### Block Elements

#### Headings
(#) Bölüm başlarını (Heading; h1, h2, h3...h6) ifade eder ve adedi kadar heading'i tanımlar. 
					

`# Heading h1`						
# Heading h1

`## Heading h2`						
## Heading h2

`### Heading h3`						
### Heading h3

`#### Heading h4`						
#### Heading h4

`##### Heading h5`						
##### Heading h5

`###### Heading h6`						
###### Heading h6



#### Paragraphs

Paragraflar, bir veya daha fazla boş satırla ayrılmış bir veya daha fazla bitişik metin satırıdır. Bir HTML etiketi olan <**br**> eklemek isterseniz, bir paragrafı iki veya daha fazla boşlukla sonlandırabilir ve ardından yeni bir paragrafa başlayabilirsiniz. Paragraf için `<p></p>` şeklinde belirtmeye gerek yoktur. Öncesinde bir satır boşluk olan yazı bloğu paragraf olarak algılanır.



#### Lists

Yıldız işaretleri, artılar veya kısa çizgiler kullanılarak sırasız listeler oluşturulabilir. Sırasız liste öğeleri , veya ile başlar * ve - alt + listeyi girintileyerek bir listeyi başka bir listenin içine yerleştirebilirsiniz, örn.
```
- List 1
- List 2
	- List 2.1
- List 3
```
- List 1 	
- List 2 
	- List 2.1 
- List 3 



Sıralı listeler bir sayı ve ardından bir nokta ile yapılır.
```
1. List 1
2. List 2	
3. List 3
```
1. List 1
2. List 2
3. List 3




#### Images

Resimler, bağlantılarla aynı şekilde yapılır, ancak önünde bir ünlem işareti bulunur!

`![images](https://user-images.githubusercontent.com/73849259/156150747-ab8cccfd-c209-4773-b143-b1c6fd4536d7.png)`




#### Quotation

Blok alıntılar aşağıdakilerden sonra yazılır >, örn.
```
> Quote here. 	
>
> -- <cite>Benjamin Franklin</cite>
```	

> Quote here.
>
> -- <cite>Benjamin Franklin</cite>



#### Tables
```
|   | Fiyat   | Adet  |	
| --|:-------:| -----:|
| A | 1000TL  | 1     |	
| B | 100TL   | 10    |	
| C | 1TL     | 1000  |	
```

|   | Fiyat   | Adet  |
| --|:-------:| -----:|
| A | 1000TL  | 1     |
| B | 100TL   | 10    |
| C | 1TL     | 1000  |

# Git Versiyon Kontrol Sistemi

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

## Temel Git Komutları

1. **git config** 
Bu komut ile kullanıcı adı ve e-posta adresi yapılandırılır ve sonraki tüm projelerde bu kullanıcı adı ve e-posta adresi kullanılır. 
`git config --global user.name kullanici_adi`
`git config --global user.email email@itu.edu.tr`



<br>

2. **git init** 
Bu komut kullanılarak bulunulan dizin boş bir git repository’si haline getirilir ve .git isimli bir dizin oluşturulur.
`git init`

<br>

3. **git clone**
Bu komut var olan bir Git repository’sinin kopyalanması için kullanılır. Git clone komutu ile öncelikle yerel bir repository işaret edilerek bu repository’nin bir kopyası, yeni bir dizine kopyalanır. Orijinal repository lokalde olabileceği gibi uzak bir cihazda yer alıyor da olabilir.
`git clone URL`


<br>

4. **git add**
Bu komut kullanılarak işaret edilen dosya veya tüm proje, çalışılan dizine eklenir. 
`git idd`

<br>

5. **git commit**
Bu komut kullanılarak çalışılan dizinde bulunan dosyalar paketlenerek .git klasörü içindeki head isimli kısıma eklenir. Daha sonra gelen pencerede bir commit mesajı girilir.
`git commit` 

<br>


6. **git status**
Bu komut kullanılarak üzerinde çalışılan Repository’nin o anki durumu görüntülenir. Üzerinde değişiklik yapılan dosyalar, yeni eklenmiş dosyalar ve commit komutu uygulanmamış dosyalar konsol üzerinde listelenir.
`git status`

<br>


7. **git checkout –b**
Bu komut kullanılarak yeni bir branch oluşturulur ve o branch üzerine geçilir.
`git checkout -b yeni_branch`

<br>


8. **git checkout**
Bu komut kullanılarak üzerinde çalışılan branch’dan bir başka branch’a geçilir.
`git checkout`

<br>


9. **git branch**
Bu komut kullanılarak repository’deki tüm branch’lar listelenir ve üzerinde olunan branch görüntülenir.
`git branch`

<br>


10.  **git branch –d**
Bu komut kullanılarak işaret edilen branch silinir.
`git branch -d diger_branch`

<br>


11.  **git pull**
Bu komut kullanılarak uzak bir repository’deki değişiklikler üzerinde çalışılan dizine getirilir ve bu dizin ile birleştirilir.
`git pull` 

<br>


12. **git merge**
Bu komut kullanılarak farklı bir branch, üzerinde çalışılan branch ile birleştirilir.
`git merge diger_branch`

<br>


13.  **git diff**
Bu komut temel dosya ile olan farklılıkları gösterir.Bu komut, git diff **<"kaynak branch">** **<"hedef branch">** şeklinde kulanıldığında işaret edilen iki branch arasındaki farklar görüntülenir.
`git diff` 

<br>



14. **git log**
Bu komut kullanılarak proje üzerindeki kayıt geçmişi en son kayıt en üstte olacak şekilde ters kronolojik sıra ile görüntülenir. Her kayıt, o kaydı alan kişinin adı, adresi, kayıt tarihi ve kayıt mesajı ile birlikte görüntülenir.
`git log` 

<br>

15. **git log --oneline**
Bu komut kullanılarak sadece commit ID’lerinin ilk 7 karakteri ve hemen yanında commit mesajı olacak şekilde kayıt geçmişi daha temiz bir şekilde görüntülenir ve proje üzerinde yapılmış değişiklikler hakkında daha kolay bilgi edinilir.
`git log --oneline`

<br>


16. **git rebase -i**
Bir proje üzerinde uzun süre çalışılıp çok fazla değişiklik commit edildiğinde commit tarihçesi çok uzun ve karmaşık görünür. Oysa ki yapılan değişiklikler tek commit mesajı ile de açıklanabilir ve böylece projeyi inceleyen kişiler proje üzerinde yapılan değişiklikleri kısa ve öz biçimde görebilirler. Bir proje üzerinde alınan birden fazla commit, git log komutu ile görüntülenmek istendiğinde kayıt alan kişilerin ismi, adresi, kayıt tarihi ve commit mesajı ile birlikte aşağıdaki gibi görünecektir.  Tüm bu değişiklikleri tek bir commit mesajı ile belirtmek ve kayıt tarihçesini daha anlaşılır kılmak için git rebase -i HEAD komutu ile işleme başlanır. Bu komutta HEAD kelimesi branch’in en uç noktasını temsil eder ve onun yanına eklenecek sayı ile kaç commit kadar geriye gidileceği belirtilir.
`git rebase -i` 

<br>
<br>


#### References
- https://bidb.itu.edu.tr/seyir-defteri/blog/2019/02/13/git
- https://git-scm.com/book/tr/v2/Ba%C5%9Flang%C4%B1%C3%A7-Versiyon-Kontrol
- https://www.hasantezcan.dev/blog/versiyon-kontrol-sistemi-git.html
- https://bookdown.org/yihui/rmarkdown/markdown-syntax.html
- https://learnxinyminutes.com/docs/markdown/
- https://www.ibm.com/docs/en/SSYKAV?topic=train-how-do-use-markdown

### Contributors
- Özgür Tıpırdamaz
- Ufuk Yetişkin
