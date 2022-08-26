# Markdown
## İçindekiler:
1. [Markdown Tarihi](#markdown-tarihi)
2. [Markdown Nedir](#markdown-nedir)
3. [Markdown Etiketleri](#markdown-etiket)
4. [Sunum Dosyası](#sunum-dosyasi) 
5. [Kaynakça](#kaynakca)

<h3 id="markdown-tarihi"></h3>

## Markdown Tarihi?
John Gruber, Markdown dilini 2004 yılında [Aaron](https://www.wikiwand.com/tr/Aaron_Swartz)  [Swartz](https://www.wikiwand.com/tr/Aaron_Swartz) ile sözdiziminde işbirliği yaparak oluşturdu, insanların okuma ve yazması kolay düz metin biçimini kullanarak isteğe bağlı olarak [XHTML](https://www.wikiwand.com/tr/XHTML)'ye veya [HTML](https://www.wikiwand.com/tr/HTML)'e dönüştürme amacını taşıyordu.

<h3 id="markdown-nedir"></h3>

## Markdown Nedir ve Nerelerde Kullanılır?
- HTML'e (text-to-HTML) dönüşüm için kullanılan hafif bir işaretleme dilidir.
- GitHub gibi platformları kullananların aşina olduğu Markdown formatı, yaygın kanının aksine sadece README dosyaları oluşturmak için kullanılmaz. Temel amaç okunabilirliği ve kullanılabilirliği arttırmaktır. Basitliği ve sadeliği sayesinde forumlarda ileti yazmaktan, kitap yazmaya kadar pek çok yerde kullanılabilir. Asıl güçlü olduğu kısım klavyeden elinizi kaldırmadan tablolardan, matematiksel ifadelere kadar ihtiyaç duyduğunuz her şeyi oluşturabilmeniz ve sonrasında biçimlendirebilmenizdir.

<h3 id="markdown-etiket"></h3>

## Markdown Etiketleri

### Başlık
Başlıklar için diyez (#) işareti kullanılmaktadır. Diyez işaretini arttırdıkça başlık boyutu küçülmektedir. Burada önemli olan diyez işaretinden sonra yazılan başlık ile diyez arasında bir boşluk bırakılmasıdır. 
# heading h1
`# heading h1`
## heading h2
`## heading h2`
### heading h3
`### heading h3`
#### heading h4
`#### heading h4`
##### heading h5 
`##### heading h5`
###### heading h6
`###### heading h6`

### Yazı Tipleri
- Eğik yazı için tek yıldız arasına yazılır.
`*eğik yazı*`
*eğik yazı*
- Kalın yazı için iki yıldız arasına yazılır.
`**kalın yazı**`
**kalın yazı**
- Hem eğik hem kalın yazı için üç yıldız arasına yazılır.
`*hem eğik hem kalın yazı*`
***Hem eğik hem kalın***
- Üstü çizili yazı için:
`~~Üstü çizili~~`
~~üstü çizili~~

### Liste
- Sırasız liste oluşturmak için kısa çizgi veya yıldız kullanılabilir. İç içe liste için listeleme işlemine devam ederken tab tuşuna basmak yeterli olur. Örneğin:
 ```
 -list1
 -list2
	 -list3
	 -list4
 ```
- list1
- list2
	- list3
	- list4

- Sıralı liste oluşturmak için sayıdan sonra nokta konulur. Sıralı listemelerde kullanılan sayılar farklı ve alakasız olsa da markdown onu sıralı bir liste haline getirecektir. Örneğin:
 ```
1. list1
9. list2
7. list3
```

1. list1
2. list2
3. list4 

### Link Oluşturma
Köşeli parantez açılıp kapatılır ve ardından normal parantez açılıp kapatılır. Köşeli parantez link açıklaması içindir bu alanın doldurulması zorunlu değildir. Normal parantezin içine link bırakılır. 
`[Açıklama](https://www.google.com.tr)`
[Açıklama](https://www.google.com.tr)

### Resim Ekleme
Link oluşturmaktan tek farkı en başa ünlem işareti konulur.
`![resim](https://cdn.iconscout.com/icon/free/png-256/markdown-433293.png)`

![resim](https://cdn.iconscout.com/icon/free/png-256/markdown-433293.png)

### Tablo Oluşturma
```
|Ürün no|Ürün Açıklaması|Ürün fiyatı|
|:--|:---:|--:|
|1|açıklama|fiyat|
|2|açıklama2|fiyat2|
```

|Ürün no|Ürün Açıklaması|Ürün fiyatı|
|:--|:---:|--:|
|1|açıklama|fiyat|
|2|açıklama2|fiyat2|

### Bölümleme
Yazıları birbirinden ayırıp bölmek ve araya bir çizgi çekmek için aşağıdaki gibi çizgi işareti kullanılır.
`---`

### Alıntı Oluşturmak
Alıntılama yapmak için büyüktür işareti kullanılır.
```
metin yazıları
>alıntılanan metin 
metin yazıları
```
metin yazıları
>alıntılanan metin

metin yazıları

### Kod Görünümü Oluşturma
- Tek satır kod için ters kesme işareti kullanılır. Bunun için 'ALT GR' + ',' kombinasyonunu deneyebilirsiniz. Tek ters kesme işaretinin arasına yazılır. Aşağıdaki gibi bir çıktı alınır.
`print("Hello World!")`

- Çok satır kod için kodun başına ve sonuna üç ters kesme işareti konulmalıdır. Eğer yazılan kodun diline göre renklenmesi isteniyorsa baştaki üç ters kesme işaretinden sonra kullanılan dilin adı yazılır.
 ```javascript
function(){
console.log("Hello World!")
}
```
<h3 id="sunum-dosyasi"></h3>

## Sunum Dosyası

[Markdown Sunum Dosyası](https://docs.google.com/presentation/d/1g78QctP8L4YZxgttjn3kP7hd9i3Xr_d1/edit?usp=sharing&ouid=102583537910212255774&rtpof=true&sd=true)

<h3 id="kaynakca"></h3>

## Kaynakça

[Markdown Yazma Rehberi](https://www.technopat.net/2019/12/09/markdown-ile-yazi-yazma-rehberi/)
[Markdown Makale](https://prototurk.com/makaleler/markdown-nedir-nasil-kullanilir)