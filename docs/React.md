# React Nedir?

[React](https://github.com/reactjs), kullanıcı arayüzü (UI) oluşturmak için kullanılan en popüler JavaScript kütüphanesidir. Web siteleri işlemek için kullanıcı çıktısına harika yanıt sunan bir yöntemi kullanır.

Bu aracın bileşenleri Facebook tarafından geliştirilmiştir. 2013’de açık kaynaklı bir JavaScript olarak piyasaya sürülmüştür. Şu anda, çok satan listesinin en üstünde yer alan Angular ve Bootstrap gibi ana rakiplerinin önündedir.

## JSX 

JSX kısaca kullanıcı arayüzünün görünümünü tanımlamada kullanılır.

Herhangi bir web sitesinin merkezinde HTML dökümanları mevcuttur. Web tarayıcınız bu dökümanları okur ve bilgisayarınızın veya kullandığınız diğer elektronik cihazların ekranına web sayfaları olarak yansıtır. Bu işlem esnasında tarayıcılar Document Oriented Model (DOM) adında, sayfaların nasıl düzenlendiği ile ilgili bir yapı oluşturur. Geliştiriciler bu yapıyı JavaScript gibi programlama dilleriyle değiştirerek dinamik içerikler ekleyebilir.

**JSX (JavaScript eXtension)** ise geliştiricilerin basit, HTML tarzı bir kod ile kendi DOM’larını değiştirip geliştireceği bir React uzantısıdır ve JSX son haliyle beraber kullandığınız herhangi bir tarayıcı ile tamamen uyumlu çalışacak şekilde güncellenmiştir.

JSX kullanarak DOM’u güncellemek inanılmaz bir web sitesi performans artışı ve geliştirme verimliliğini beraberinde getirir. 

## Virtual DOM 

Eğer ReactJS kullanmıyorsanız, web siteniz DOM’u güncellemek için HTML kullanır. Bu, kullanıcının arayüz ile teması olmadan ekrandaki değişikliklerin olduğu işlemdir. Bu işlem statik web sitelerinde sorunsuz bir şekilde gerçekleşir, fakat yüksek kullanıcı yoğunluklarının olduğu dinamik web sitelerinde kullanıcı her yenile komutu verdiğinde tüm DOM’un güncellenmesi gerekir. Bu da ciddi problemlere yol açabilir.


![Virtual DOM](https://www.argenova.com.tr/uploads/virtual-dom.jpg)

Bunu önlemek için ReactJS tarafında Virtual DOM adında bir yapı geliştirilir. 

Virtual DOM sayesinde kullanıcı ne zaman yenile tarzında bir komut verse, ReactJS gerçek DOM’daki değişikleri tespit eder. Bu sayede tüm DOM’un güncellenmesinden ziyade sadece değişiklik yapılan alan için güncelleme sağlanmış olur. 

Bu özellik, kompleks ve yüksek kullanıcı etkileşimi içeren web sitelerinde ciddi anlamda düşük hesaplama güçleri ve yüklenme zamanları ile hem kullanıcılara, hem de geliştiricilere büyük avantaj sağlar.

## React  Projesi Nasıl Oluşturulur? 

Visual Studio Code IDE'si içerisinde yeni bir terminal (**ctrl+shift+"**) oluştururuz. Oluşturulan terminal üzerinden; <br>

**npx**
```
npx create-react-app my-app
```
**npm**
```
npm create-react-app my-app
```
**npx**
```
yarn create-react-app my-app
```
komutları ile yeni bir react projesi oluşturabiliriz. Oluşturulan projeyi ayağa kaldırmak için;

```
npm/yarn start 
```
komutu yazılır.

## React Nasıl Çalışır?

React nedir öğrendiğinize göre sırada React’in nasıl çalıştığı var. HTML kodlarını JavaScript’te yazabileceğinizi öğrendiğinize şaşırabilirsiniz. Ancak React de tam olarak böyle çalışır.

Örnek kod örneği;

```
import React from 'react'

function App{
   return (
      <div>
         <h1> React Nedir? </h1>
      </div>
   )
}

expert default App;

```
Bu kod bloğu üzerinde istenilen elementler oluşturulup dinamik bir hale getirilebilir.


