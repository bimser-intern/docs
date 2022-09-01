## İçindekiler

1. [Yazılım Test Mühendisinin Görevleri](#Yazılım-Test-Mühendisinin-Görevleri)
2. [Yazılım Testi Neden Önemli?](#Yazılım-Testi-Neden-Önemli?)
3. [Manuel Test Nedir?](#Manuel-Test-Nedir?)
4. [Otomasyon Testi Nedir?](#Otomasyon-Testi-Nedir?) 
5. [Manuel Test ile Otomasyon Testi Arasındaki Farklar](#Manuel-Test-ile-Otomasyon-Testi-Arasındaki-Farklar)
6. [Manuel Test ile Otomasyon Testinin Avantajları ve Dezavantajları](#Manuel-Test-ile-Otomasyon-Testinin-Avantajları-ve-Dezavantajları) 
7. [Sunum Dosyası](#sunum-dosyası)
8. [Kaynakça](#kaynakça)

<br>


# Yazılım Test Mühendisinin Görevleri?


* Tüm belgeleri okumak ve neyin test edilmesi gerektiğini anlamak.
* Nasıl test edileceğine karar vermek.
* Test liderine yazılım testi için tüm kaynakların gerekeceği hakkında bilgi vermek. 
* Test senaryoları geliştirmek ve test faaliyetlerine öncelik vermek.
* Tüm test senaryosunu yürütmek ve hataları bildirmek, her hata için ciddiyeti ve önceliği tanımlamak.
* Hataları düzeltmek için kodda her değişiklik yapıldığında regresyon testini gerçekleştirmek.
* Hata raporlarını yazarak ilgili birimleri/kişileri bilgilendirmek.
* Hatalar/Sorunlar giderildikten sonra yeniden testin yapılması.
* Müşteri ve kullanıcı memnuniyetini göz önünde bulundurarak analiz ve test aşamalarında gerekli düzenlemeleri sağlamak.
* Son kullanıcıya bırakılmadan önce analiz ve testlerdeki tüm hataların düzeltilmesini sağlayarak hatasız ürünler sunmak.

# Yazılım Testi Neden Önemli?

* Yazılım Testi neden önemli sorusuna genelde insanın olduğu yerde hata kaçınılmaz olarak cevap vermem yeterli olur mu bilemedim. 
Çünkü hepimiz hata yapıyoruz/yapabiliriz. Bu hataların bazıları önemsizdir, ancak bazıları pahalı veya tehlikeli boyutlarda olabiliyor. 
Ürettiğimiz her şeyi kontrol etmeliyiz çünkü işler her zaman istediğimiz gibi gitmeyebilir. Bu yüzden yazılım testi aşağıdaki 
nedenlerden dolayı çok önemlidir:

* 1. Yazılım testi, geliştirme aşamalarında yapılan hataları belirtmek için gereklidir.
- Mesela programcılar yazılımın uygulanması sırasında hata yapabilirler. Bunun için programcının deneyim eksikliği, 
programlama dili hakkında bilgi eksikliği, alanda yetersiz deneyim, karmaşık mantık nedeniyle algoritmanın yanlış 
uygulanması veya sadece insan hatası gibi birçok neden olabilir. beklenir.
* 2. Müşterinin kuruluşu güvenilir bulmasını ve uygulamadaki memnuniyetini korumasını sağlaması önemlidir.
- Müşteri test organizasyonunu güvenilir bulmazsa veya teslim edilebilir ürünün kalitesinden memnun değilse, bir rakip 
organizasyona geçebilir.
- Bazen sözleşmeler, ürünün zaman çizelgesi ve kalitesiyle ilgili parasal cezalar da içerebilir. Bu gibi durumlarda, uygun yazılım 
testi yapılması parasal kayıpları da önleyebilir
* 3. Ürünün Kalitesini sağlamak çok önemlidir. Müşterilere sunulan kaliteli ürün güvenlerini kazanmaya yardımcı olur.
- Bir önceki noktada açıklandığı gibi, zamanında kaliteli ürün sunmak, müşterilerin şirkete olan güvenini arttırır.
* 4. Daha düşük bakım maliyeti gerektiren ve dolayısıyla daha doğru, tutarlı ve güvenilir sonuçlara yol açan yüksek kaliteli ürün veya 
yazılım uygulaması gibi müşterilere kolaylık sağlamak için testler gereklidir.
- Yüksek kaliteli ürünün tipik olarak daha az kusuru vardır ve daha az bakım çabası gerektirir, bu da daha düşük maliyet anlamına gelir.
* 5. Yazılım uygulamasının veya ürünün etkili bir performansı için test yapılması gerekir.
* 6. Uygulamanın herhangi bir arızaya neden olmamasını sağlamak önemlidir, çünkü gelecekte veya geliştirmenin sonraki aşamalarında çok pahalı olabilir.
- Doğru test, hataların ve sorunların ürünün veya uygulamanın yaşam döngüsünün erken aşamalarında tespit edilmesini sağlar.
- Gereksinimler veya tasarımla ilgili kusurlar yaşam süresinde geç tespit edilirse, uygulamanın yeniden tasarlanması ve yeniden test 
edilmesini gerektirebileceğinden bunları düzeltmek çok pahalı olabilir

# Manuel Test Nedir?

* Manuel test, testlerin QA tarafından manuel olarak yürütüldüğü yazılımın test edilmesidir. Geliştirilmekte olan yazılımdaki hataları keşfetmek için yapılır.
Manuel testte, uygulamanın veya yazılımın tüm temel özellikleri kontrol edilir. Bu süreçte, yazılım testçileri test senaryolarını yürütür ve otomasyon yazılımı test araçlarının yardımı olmadan test raporlarını oluşturur.

# Otomasyon Testi Nedir?

* Otomasyon Yazılım Testinde, test kullanıcıları testin yürütülmesini otomatikleştirmek için kod / test komut dosyaları 
yazarlar. Test kullanıcıları, test komut dosyalarını geliştirmek ve yazılımı doğrulamak için uygun otomasyon araçlarını kullanır. 
Amaç, test uygulamasını daha kısa sürede tamamlamaktır.Otomasyon testi, tamamen gerçek sonucu beklenen sonuçlarla 
karşılaştırmak için otomatik olarak çalışan önceden yazılmış teste dayanır. Bu, test edicinin bir uygulamanın beklendiği gibi 
performans gösterip göstermediğini belirlemesine yardımcı olur.

# Manuel Test ile Otomasyon Testi Arasındaki Farklar
Manuel Test ile Otomasyon Testi arasındaki farkları kısaca sizlerle 10 maddede paylaşmak isterim. Bu maddeleri çoğaltabiliriz .

### Manuel Test:

* 1. Manuel Testte, test senaryoları bir birey tarafından gerçekleştirilir.
* 2. Manuel Test zaman alıcıdır ve insan kaynaklarını kullanır.
* 3. Manuel Testte keşif testi yapmak mümkündür.
* 4. Manuel Test yöntemi, kullanıcı dostu bir sistem sunmak için yararlı olabilecek insan gözlemine izin verir.
* 5. Performans Testi manuel olarak mümkün değildir.
* 6. Manuel Testler toplu işlenemez.
* 7. Manuel Testte programlamaya gerek yoktur.
* 8. Tekrarlayan Manuel Test Yürütme sıkıcı ve hataya açık olabilir.
* 9. Manuel Test, önceden belirlenmiş test tarihini kaçırmak için daha yüksek bir risk taşır.
* 10. Manuel Test, Keşif, Kullanılabilirlik ve Adhoc Testleri için uygundur. Ayrıca AUT’nin sık sık değiştiği yerlerde kullanılmalıdır.

### Otomasyon Testi :

* 1. Otomasyon Testi, test senaryolarını yürütmek için otomasyon araçlarını kullanır.
* 2. Otomasyon Testi, manuel bir yaklaşımdan çok daha hızlıdır.
* 3. Otomasyon Testi düzensiz testlere izin vermiyor.
* 4. Otomasyon Testi insan düşünmesini içermez. Böylece hiçbir zaman kullanıcı dostu ve olumlu müşteri deneyimi güvencesi veremez.
* 5. Yük Testi, Stres Testi, Spike Testi vb. Performans Testleri zorunlu olarak bir otomasyon aracı ile test edilmelidir.
* 6. Birden fazla Test Komut Dosyasını Toplu İşleyebilirsiniz.
* 7. Otomasyon Testinde programlama bilgisi şarttır.
* 8. Araçlar tarafından yapılır.
* 9. Otomasyon Testleri, önceden belirlenmiş bir testi kaçırma riskini sıfırlar.
* 10. Otomasyon Testi, Regresyon Testi, Performans Testi, Yük Testi veya yüksek oranda tekrarlanabilir fonksiyonel test durumları için uygundur.

# Manuel Test ile Otomasyon Testinin Avantajları ve Dezavantajları

### Manuel Testin Avantajları:

* Manuel Test her türlü uygulamada yapılabilir.
* Kısa ömürlü ürünler için tercih edilir.
* Yeni tasarlanan test senaryoları manuel olarak yürütülmelidir.
* Uygulama otomatikleştirilmeden önce manuel olarak test edilmelidir.
* Gereksinimlerin sık sık değiştiği projelerde ve GUI’nin sürekli 
değiştiği ürünler için tercih edilir.
* Otomasyon testine kıyasla ilk yatırım açısından daha ucuz.
* Test cihazının adhoc testi yapmasına izin verir.
* Test cihazının Otomasyon Araçları hakkında bilgi sahibi olmasına gerek yoktur.

### Manuel Testin Dezavantajları:

* Manuel Test esas olarak regresyon testi yaparken zaman alıcıdır.
* Manuel test, insanlar tarafından yürütüldüğü için otomasyon  
testine göre daha az güvenilirdir. Yani her zaman hata ve hatalara eğilimli olacaktır.

### Otomasyon Testinin Avantajları:
* Otomasyon Testi uygulamada daha hızlı.
* Uzun vadede manuel testlere göre daha ucuz.
* Otomasyon Testi daha güvenilirdir.
* Otomasyon Testi daha güçlü ve çok yönlüdür.
* Çoğunlukla regresyon testi için kullanılır.
* Tekrar kullanılabilir çünkü otomasyon süreci kaydedilebilir.
* İnsan müdahalesi gerektirmez. Test komut dosyaları katılımsız olarak çalıştırılabilir.
* Test kapsamını artırmaya yardımcı olur.

### Otomasyon Testinin Dezavantajları:

* Sadece kararlı ürünler için önerilir.
* Otomasyon Testi başlangıçta pahalıdır.
* Otomasyon araçlarının çoğu pahalıdır.

# Sunum Dosyası

[Test Mühendisinin Görevleri Sunumu](https://drive.google.com/file/d/1ccrrH3b14d3-5q5OjPbx0troYQwEfhYG/view?usp=sharing)

# Kaynakça

* [Kaynakça](https://miktadozturk.medium.com/yaz%C4%B1l%C4%B1m-test-m%C3%BChendisli%C4%9Fi-ve-yaz%C4%B1l%C4%B1m-testine-genel-bak%C4%B1%C5%9F-40585be2fc58)

