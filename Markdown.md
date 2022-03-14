
## İçindekiler

1. [Markdown Nedir?](#markdown-head)
2. [Markdown Elements](#markdown-elements)
   - [Inline Elements](#markdown-inline-elements)
   - [Block Elements](#markdown-block-elements) 

---
<br>
<br>
<br>


<h3 id="markdown-head"></h3>

# Markdown Nedir?

----

Günümüzde dijital ortamlarda makale, blog yazısı gibi metin diagramları oluştururken, metnin akışına uygun olarak başlık, liste ve tablo gibi görsel biçimler kullanırız. Günümüzde bu tarz içerikleri üretirken *HTML(Hyper Text Markup Language)* işaretleme dilini kullanırız. Fakat bir yazı için hem uğraştıcı olup hem de hataların oluşmasına neden olabilir. İşte bu zamanlarda işimizi kolaylaştıracak bir text to *HTML* yapısı ile dönüştürme aracı olan **Markdown** karşımıza çıkıyor.

## Markdown
John Gruber, Markdown dilini 2004 yılında Aaron Swartz ile sözdiziminde işbirliği yaparak oluşturdu, insanların okuma ve yazması kolay düz metin biçimini kullanarak isteğe bağlı olarak XHTML'ye veya HTML'e dönüştürme amacını taşıyordu.
	
Markdown, düz-metin-biçimlendirme sözdizimine sahip hafif bir işaretleme dili. Tasarımı, birçok çıktı biçimine dönüştürülmesine izin verir, ancak aynı ada sahip orijinal araç yalnızca HTML'yi destekler. Markdown genellikle BENİOKU (README) dosyalarını biçimlendirmek, çevrimiçi tartışma forumlarına mesaj yazmak ve düz metin düzenleyicisi kullanarak zengin metin oluşturmak için kullanılır. Markdown’un ilk tanımı belirsizlikler ve cevaplanmamış sorular içerdiğinden, yıllar boyunca ortaya çıkan uygulamaların ince farklılıkları vardır ve çoğu sözdizimi, dosya uzantılarıyla birlikte gelir.


<h3 id="markdown-elements"></h3>

## Markdown Elements


<h3 id="markdown-inline-elements"></h3>

### Inline Elements 


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



<h3 id="markdown-block-elements"></h3>

###  Block Elements

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
```
![images](https://user-images.githubusercontent.com/73849259/156150747-ab8cccfd-c209-4773-b143-b1c6fd4536d7.png)`
```

![images](https://www.lordiz.com/resimler/lordiz/webp-image_zpsakyq03sw.png)




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
<br>





