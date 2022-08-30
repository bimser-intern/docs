İçindekiler

---

- [Kotlin Nedir?](#kotlin-nedir)
- [Kotlin Java programlama diline göre ne gibi avantajlar sağlıyor?](#kotlin-java-programlama-diline-göre-ne-gibi-avantajlar-sağlıyor)
- [Kotlin'de Değişken Tanımlama](#kotlinde-değişken-tanımlama)
- [Kotlin'de Data Tipleri](#kotlinde-data-tipleri)
- [Kotlin'de String Tanımlama](#kotlinde-string-tanımlama)
- [String Elemanlarına Erişme](#string-elemanlarına-erişme)
- [Kotlin’de Yorum Satırları](#kotlinde-yorum-satırları)
- [Kotlin If ... Else](#kotlinif--else)
- [Kotlin'de When ve While Döngüsü](#kotlindewhen-ve-while-döngüsü)
- [Kotlinde For Döngüsü ve Fonksiyon Oluşturma/Çağırma](#kotlinde-for-döngüsü-ve-fonksiyon-oluşturmaçağırma)
- [Kotlin'de Break ve Continue](#kotlindebreak-ve-continue)
- [Kotlin Arrays](#kotlinarrays)
- [Kotlin Sunum Dosyası](#kotlinsunum-dosyası)
   

<br /><br />

# Kotlin Nedir?

Kotlin, JVM, Android, JavaScript ve Native'i hedefleyen, açık kaynaklı, statik olarak yazılmış bir programlama dilidir. Kotlin, hem nesne yönelimli hem de işlevsel yapılara sahiptir. Hem OO hem de fonksiyonel yapı stillerinde kullanabilir veya ikisinin öğelerini karıştırabilirsiniz.

- Kotlin’i [play.kotlinlang.org](https://play.kotlinlang.org/) sitesinden kullanabilirsiniz.
- Ayrıca Android Studio’da da kullanabilirsiniz.

<br /><br />

# Kotlin Java programlama diline göre ne gibi avantajlar sağlıyor?

- <ins>Etkileyici ve özlü:</ins> Daha azıyla daha fazlasını yapabilirsiniz. Kotlin'i kullanan profesyonel geliştiricilerin %67'si, Kotlin'in üretkenliklerini artırdığını söylüyor.

- <ins> Daha güvenli kod:</ins> Kotlin, boş işaretçi istisnaları gibi yaygın programlama hatalarından kaçınmanıza yardımcı olacak birçok dil özelliğine sahiptir. Kotlin kodu içeren Android uygulamalarının çökme olasılığı %20 daha düşüktür.

- <ins> Birlikte çalışabilir:</ins> Kotlin, Java programlama diliyle %100 birlikte çalışabilir, bu nedenle projenizde istediğiniz kadar az veya çok Kotlin'e sahip olabilirsiniz.

- <ins>Yapılandırılmış Eşzamanlılık:</ins> Kotlin eşyordamları, eşzamansız kodla çalışmayı engelleme kodu kadar kolay hale getirir. Eşyordamlar, ağ aramalarından yerel verilere erişmeye kadar her şey için arka planda görev yönetimini önemli ölçüde basitleştirir.

<br /><br />

# Kotlin'de Değişken Tanımlama

Kotlin, değişkenleri bildirmek için iki farklı anahtar kelime kullanır: **val** ve **var**.

- Değeri asla değişmeyen bir değişken için **val** kullanın. val kullanılarak bildirilen bir değişkene yeniden değer atayamazsınız.
  
- Değeri değişebilen bir değişken için ise **var** kullanın.

- Ayrıca Kotlin’de değişken tanımlanırken *camelCase* adı verdiğimiz değişken isimlendirme yöntemi kullanılır. Zorunlu değildir ama kodu okumayı kolaylaştırır. 
  
  ![Değişken örneği](https://user-images.githubusercontent.com/65497602/186871759-fb8d0ce2-62e1-4b97-9b11-c9399215c1fe.png)


<br /><br />

# Kotlin'de Data Tipleri

Kotlin'de bir değişken tanımlarken tipini belirtmek zorunda değiliz. Ama belirtmek sonradan yaşanma ihtimali olan sorunları azaltır.

![image](https://user-images.githubusercontent.com/65497602/186872221-3b271f5a-c8a9-445f-ae96-8aa1cf70fc61.png)

![image](https://user-images.githubusercontent.com/65497602/186872345-198a9fad-f9ad-4195-85fe-850f823b9a94.png)

<br /><br />

# Kotlin'de String Tanımlama

![image](https://user-images.githubusercontent.com/65497602/186872707-95286f65-414a-4f11-8f4b-e4e53e1e9b3a.png)
![image](https://user-images.githubusercontent.com/65497602/186872840-61cdff37-6c25-46e3-9613-2239101c47ef.png)

Resimlerde görünen iki şekilde de String tanımı yapılabilir.

<br />

<ins>**Not:**</ins> Değeri atamadan (ve değeri daha sonra atamadan) bir String oluşturmak istiyorsanız, değişkeni bildirirken tipi belirtmelisiniz.

![image](https://user-images.githubusercontent.com/65497602/186873177-4fefa167-d1bd-43a3-98d3-08b44812c85c.png)

İkinci resimdeki atama yanlıştır.

![image](https://user-images.githubusercontent.com/65497602/186873291-8c3c8250-1be0-4be0-9077-f076b86ac34e.png)

<br /><br />

# String Elemanlarına Erişme
Bir dizenin karakterlerine (öğelerine) erişmek için köşeli parantez içindeki dizin numarasına başvurmanız gerekir.

![image](https://user-images.githubusercontent.com/65497602/186873874-52e6ebe3-b8f8-4750-b283-1c45d5444dcf.png)

<br /><br />

# Kotlin’de Yorum Satırları

Tek satırlı yorumlar iki eğik çizgiyle (//) başlar. // ile satırın sonu arasındaki herhangi bir metin Kotlin tarafından yok sayılır (yürütülmez).

![image](https://user-images.githubusercontent.com/65497602/186874211-a947c1f3-62a9-41a6-9a81-146f115d1530.png)

Çok satırlı yorumlar /* ile başlar ve */ ile biter. Bu iki işaret arasındaki herhangi bir metin Kotlin tarafından yok sayılır.

![image](https://user-images.githubusercontent.com/65497602/186874280-36b7c4f1-2df3-4c61-84c8-e977ad12fda7.png)

<br /><br />

# Kotlin If ... Else

- Bir koşul doğruysa yürütülecek bir kod bloğu belirtmek için if öğesini kullanın.

- Koşul yanlışsa yürütülecek kod bloğunu belirtmek için else kullanın.

![image](https://user-images.githubusercontent.com/65497602/186876198-59aa2c65-07f3-4405-8c37-971cabd4bde2.png)

![image](https://user-images.githubusercontent.com/65497602/186876239-3be69276-4a9f-4a08-8c64-f552f9e5a1e9.png)


<br /><br />

# Kotlin'de When ve While Döngüsü

Birçok if..else ifadesi yazmak yerine, okunması çok daha kolay olan when ifadesini kullanabilirsiniz.

![image](https://user-images.githubusercontent.com/65497602/186876609-57292e7c-ea8d-4327-9e1e-e730653f0a4f.png)


Aşağıdaki örnekte, sayaç değişkeni (i) 5'ten küçük olduğu sürece döngüdeki kod tekrar tekrar çalışacaktır:

![image](https://user-images.githubusercontent.com/65497602/186876734-b667538b-fcd3-4503-bfed-ac2ff9d7d988.png)

<br /><br />

# Kotlinde For Döngüsü ve Fonksiyon Oluşturma/Çağırma

Dizi öğeleri arasında döngü oluşturmak için, in operatörüyle birlikte for döngüsünü kullanın:

![image](https://user-images.githubusercontent.com/65497602/186876927-d1a8414b-dac0-43a2-9918-5f42654aeeb7.png)

![image](https://user-images.githubusercontent.com/65497602/186876996-8c015798-1e1c-435b-a4aa-20446438149e.png)

<br />

Fonksiyon, yalnızca çağrıldığında çalışan bir kod bloğudur. Parametre olarak bilinen verileri bir işleve geçirebilirsiniz. İşlevler, belirli eylemleri gerçekleştirmek için kullanılır ve bunlar yöntem olarak da bilinir.

![image](https://user-images.githubusercontent.com/65497602/186877098-d0bd0075-2baf-4c3c-a76c-2f650c12321e.png)

![image](https://user-images.githubusercontent.com/65497602/186877130-3e70dc6d-f19c-4149-b895-6a782d69273b.png)

<br /><br />

# Kotlin'de Break ve Continue

Break ifadesi bir döngüden çıkmak için kullanılır. Aşağıdaki örnek, i 4'e eşit olduğunda döngüden atlar:

![image](https://user-images.githubusercontent.com/65497602/186877393-1bddc2a6-7451-46d4-b4f0-4ae1c69de758.png)

<br />

Devam ifadesi, belirtilen bir koşul oluşursa bir yinelemeyi (döngüde) keser ve döngüdeki bir sonraki yinelemeyle devam eder. Bu örnek 4 değerini atlıyor:


![image](https://user-images.githubusercontent.com/65497602/186877464-312e18b9-e27d-4185-9600-1db3caba5123.png)

<br /><br />

# Kotlin Arrays

Dizi elemanına köşeli parantez içindeki indeks numarasına bakarak ulaşabilirsiniz. Bu örnekte, arabalardaki ilk elemanın değerine erişiyoruz:

![image](https://user-images.githubusercontent.com/65497602/186877856-9b36d89d-daba-4917-a1df-e08368d55583.png)

<br />

Belirli bir öğenin değerini değiştirmek için dizin numarasına bakın:

![image](https://user-images.githubusercontent.com/65497602/186877937-408941f3-ca37-404c-b020-b8ccbe3b88c8.png)


<br /><br />

# Kotlin Sunum Dosyası

[Kotlin Sunum Dosyası](https://github.com/bimser-intern/docs/files/9432116/Kotlin.pptx)

