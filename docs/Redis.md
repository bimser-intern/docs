# İçindekiler

1. [Redis nedir?](#redis-nedir)
2. [Redis 'in avantajları nelerdir?](#redis-in-avantajları-nelerdir)
3. [Redis 'in dezavantajları nelerdir?](#redis-in-dezavantajları-nelerdir)
4. [Örnek redis sorguları](#örnek-redis-sorguları)

# Redis nedir?
- Redis, geliştiriciler tarafından en çok kullanılan ve bilinen NoSQL veritabanlarından birisidir.
- Redis, açık kaynaktır ve kaynak kodlarına GitHub üzerinden erişilebilmektedir. C dili ile yazıldığı için yüksek performanslı sonuçlar vermektedir.
- C dili ile yazıldığı için yüksek performanslı sonuçlar vermektedir. 
- Linux ve türevi işletim sistemleri tarafından desteklenmekte fakat Windows tarafı için resmi bir destek olmasa da community tarafından desteklenmektedir.

![image](https://devnot.com/wp-content/uploads/2020/04/redis.png)

- Redis günümüz sistemlerinde en çok kullanılan anahtar-değer veritabanıdır ve genellikle caching, session yönetimi, pub/sub, message broker amacıyla kullanılmaktadır.


# Redis 'in avantajları nelerdir?

#### Yüksek Performans 
- Redis, verileri disklerde (HDD veya SSD) tutan veri tabanlarının aksine bellek (RAM) üzerinde tutar bu sayede disklere erişim ihtiyacını ortadan kaldırarak gecikmeleri, I/O bağlantılarını önler ve daha az CPU kullanan basit algoritmalar ile verilere erişir.

#### In-Memory Veri Yapıları 
- Redis verileri bellek üzerinde <key,value> çifti olarak tutmaktadır, burada her bir anahtara denk gelen değerler farklı veri yapılarında tutulabilmektedir. 
- Redis kullanılarak neredeyse her türlü veri bellekte saklanabilir.

#### Replication 
- Redis, master-slave mimarisini kullanır, master genel olarak yazma işlemlerini yapar ve slave dediğimiz yapılar da master’in birer kopyasıdır, master güncellendikçe ona bağlı bütün slave’ler de güncellenir. Burada master’da oluşacak herhangi bir çökmede, hatada direkt bir slave master olarak seçilir ve sistem çalışmaya devam eder.

#### Çoklu Dil Desteği 
- Redis birçok dil tarafından desteklenmektedir, bunlar; Java, Python, PHP, C, C ++, C #, JavaScript, Node.js, Ruby, R, Go gibi dillerdir ve bunların yanı sıra daha fazla da dil bulunmaktadır.

# Redis 'in dezavantajları nelerdir?
- Her kaynak gibi Redis’in de avantajlarının yanı sıra birkaç dezavantajı vardır. Redis’i kullanırken karşılaşılabilecek bazı önemli zorluklar aşağıdaki şekildedir:

#### Temel güvenlik düzeyi  
Redis, yalnızca bulut sunucusu düzeyinde temel güvenlik (erişim hakları gibi) sağlar. RDBMS, ayrıntılı, nesne başına erişim kontrol listeleri sağlar (role management olarak da bilinir).

#### Esneklik
- Redis’te sorgulama dili yoktur, sadece komutlar vardır. İlişkisel cebir için herhangi bir destek de yoktur. Kişi herhangi bir geçici sorgu gönderemez. Tüm veri erişimlerinin bir geliştirici tarafından öngörülmesi ve uygun veri erişim yolları tasarlanması gerekir. Bu nedenle esnekliğin kaybolduğuna inanılır.

#### Veri yönetimi  
- Tüm veriler belleğe sığmalıdır. RDBMS genellikle disklerdeki bilgi ve verilerin önbellek kısmını bellekte saklar. Bir RDBMS kullanarak, sahip olduğu bellekten daha fazla veri yönetilebilir. Redis ile bu mümkün değildir.

#### Kalıcılık 
- Redis’in kalıcılık için yalnızca 2 seçeneği vardır: Normal anlık görüntü alma ve yalnızca ekleme dosyaları. Bunların hiçbiri, yineleme/geri alma günlük kaydı, belirli bir noktada kurtarma, blok sağlama toplamı, flashback yetenekleri vb. sunan gerçek işlem sunucusu kadar güvenli değildir.

# Örnek Redis Sorguları
[Dokümana bu linke tıklayarak erişebilirsiniz.](https://devnot.com/2020/redis-nedir-temel-kullanim-alanlari-nelerdir/)





