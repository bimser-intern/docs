# Tailwind Nedir?

Adam Wathan tarafından 4 kişilik bir ekiple geliştirilen, özelleştirilebilir yapıya sahip bir CSS kütüphanesidir. Bootstrap ve Foundation’dan farklı olarak bir UI Kit değildir, içerisinde hazır bir tema ile gelmez. Tailwind’de, UI KIT yerine daha low-level tasarım abstraction’ları vardır.

Tailwind’in temel özellikleri:

- Daha detaylı çalışabilmeyi sağladığından dolayı daha fazla esneklik sağlar.
- Birleşen(Component) oluşturmaya çok elverişlidir.
- Tüm elementleri responsive dizayna uyumludur.
- Genişletilebilir ve özelleştirilebilir yapıya sahiptir.

## React Projesi İçerisine Tailwind CSS  Nasıl Dahil Edilir?

1. Yeni bir react projesi oluştur. 

>``` npx create-react-app my-project ``` 

2. Oluşturulan reac projesi içerisine gir. 
>``` cd my-project ```
3. Tailwind CSS paketini indir. 
>``` npm install -D tailwindcss postcss autoprefixer ```
4. *tailwind.config.js* ve *postcss.config.js* dosyalarını indir. 
>``` npx tailwindcss init -p ```
5.  *tailwind.config.js* dosyası içerisinde bütün dosya uzantılarını ekleyelim. 
```
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```  
6. Proje dosyası içerisine bir css klasörü oluşturun ve @tailwind yönergelerini oluşturduğunuz css klasörünüze ekleyin.
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Tailwind Nasıl Çalışır?

```
export default function App() {
  return (
    <h1 className="text-3xl font-bold underline">
      Hello world!
    </h1>
  )
}
```
Örnekte görüleceği üzere **inline** olarak kullanılır. Bu şekilde sadece inline olarak tanımladığımız css kodunun tanımlandığı elementler üzerinde etkisi olur.