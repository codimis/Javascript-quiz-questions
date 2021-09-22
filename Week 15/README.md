# CODIMIS 

## Javascript Eğitimi Advanced DOM And Events Soruları

1 - Formdaki buton için yazılmış event listener, butona tıklandığında sayfayı yenilemektedir. Hangi fonksiyon sayfanın yenilenmesini engeller?

```javascript
button.addEventListener(
  'click',
  function (e) {
    button.className = 'clicked';
  },
  false,
);
```

* A) e.blockReload();
* B) button.preventDefault();
* C) button.blockReload();
* D) e.preventDefault();

2 - DOM'a yeni bir eleman eklemek için hangi metod kullanılır?

* A) document.addElement()
* B) document.createElement()
* C) html.createElement()
* D) html.addElement()

3 - Event propagation'ın 3 adımının sırası nasıldır?

* A) Target > Capturing > Bubbling
* B) Bubbling > Target > Capturing
* C) Target > Bubbling > Capturing
* D) Capturing > Target > Bubbling

4 - "Bütün DOM eventleri bubbling'i desteklemektedir."

* A) Doğru
* B) Yanlış

5 - Aşağıdaki örnekteki data-columns elemanının değerine DOM üzerinde erişmek için hangi seçenekteki kullanım doğrudur? 
```html

<article
  id="electric-cars"
  data-columns="3"
  data-index-number="12314"
  data-src="cars">
...
</article>
```

```javascript
const article = document.querySelector('#electric-cars');
//??
```

* A) article.data-columns
* B) article.data.columns
* C) article.dataset.columns
* D) article.dataset.getColumns()

6 - Butona tıklandığında event'in div elemanında dinlenmesinin engellenmesi için 17.satırda hangi fonksiyon kullanılır?

```html
<div id="wrapper">
    <button id="signup">Sign Up</button>
</div>
```

```javascript
const div = document.querySelector('#wrapper');
const btn = document.querySelector('#signup');

// add <div> event handler
div.addEventListener('click', (e) => {
    console.log('The wrapper box was clicked!');
});

// add button event handler
btn.addEventListener('click', (e) => {
    //??
    console.log('The button was clicked!');
});
```

* A) e.preventDefault()
* B) return;
* C) e.stopPropagation()
* D) btn.closest.removeEventListener()

7 - Aşağıdaki NodeList objesini spread operator ile array e dönüştürmek için hangi kod yazılmalıdır?
```javascript
const divs = document.querySelectorAll('div');
```

* A) const divsArr = Array.prototype.slice.call(divs);
* B) const divsArr = Array.from(divs);
* C) const divsArr = [...divs];
* D) 

8 - Aşağıdaki kodun çıktısı ne olur?

```html
<ul>
    <li>Hamburger</li>
    <li>Pizza</li>
    <li id="drink">Drink
      <ul>
        <li class="drink">Coke</li>
        <li>Water</li>
        <li>Mojito</li>
      </ul>
       </li>   
    <li>Dessert</li>
    <li>Cake</li>
</ul>
```

```css
.drink {
  color : red;
}
```
```javascript
const drink = document.querySelector('#drink');
const sibling = drink.nextElementSibling;
console.log(sibling);
```

* A) `<li>Water</li>`
* B) `<li>Dessert</li>`
* C) `<li>Pizza</li>`
* D) `<li id="drink">Drink</li>`

9 - Paragrafa tıklandığında kodun çıktısı ne olur?

```html
<div onclick="console.log('div')">
  <p onclick="console.log('p')">
    Click here!
  </p>
</div>
```

* A) p div
* B) div p
* C) p
* D) div

10 - Butona tıklandığında event.target hangisi olur?

```html
<div onclick="console.log('first div')">
  <div onclick="console.log('second div')">
    <button onclick="console.log('button')">
      Click!
    </button>
  </div>
</div>
```

* A) first div'i print eden div
* B) second div'i print eden div
* C) button
* D) İç içe bütün elemanların olduğu bir array

11 - Aşağıdaki kod hangi sonucu verir?

```javascript
let li = document.querySelector('li');
li.style.color = "red";
```

* A) Her li elemanı kırmızı olur.
* B) Her listedeki ilk li elemanı kırmızı olur.
* C) DOM'daki ilk li elemanı kırmızı olur.
* D) CSS'de bir renk uygulanmadıysa ilk li elemanını kırmızı yapar.

12 - Aşağıdaki kodun çıktısı ne olur?

```html
<div id="foo">
  <button id="but">button</button>
</div>
```

```javascript
document.querySelector('#foo').addEventListener('click',
  function (e) {
    console.log('div clicked');
  });

document.querySelector('#but').addEventListener('click',
  function (e) {
    console.log('button clicked');
    e.stopPropagation();
  });
```

* A) button clicked
* B) button clicked - div clicked
* C) Error
* D) undefined

13 - Aşağıdakilerden hangisi DOM hiyerarşisindeki elemanlar arasındaki ilişkilerden biri değildir?

* A) parent
* B) child
* C) sibling
* D) cousin

14 - Sticky navigation gibi bir yapıyı scroll event ini dinleyerek yapabildiğimiz gibi ________ kullanarak da yapabiliriz.

* A) Lazy Loading
* B) Intersection Observer
* C) Event Propagation
* D) DOM Traversing

15 - Web sayfası tamamen yüklendiğinde ______ eventi, kullanıcı sayfadan ayrıldığında ise ______ eventi tetiklenir.

* A) mouseenter - mouseleave
* B) enter - exit
* C) load - beforeunload
* D) focus - blur

16 - IntersectionObserver'a verilen callback'in ilk parametresinin türü nedir?

```javascript
IntersectionObserver(callback,options);
```
* A) Object
* B) HTML kod
* C) Selector Array
* D) Array

17 - DOMContentLoaded eventi ne zaman gerçekleşir?

* A) Tarayıcı sayfayı yeniden çizdiğinde
* B) Tarayıcı HTML ve CSS'i tamamen yüklediğinde
* C) Tarayıcı HTML, CSS ve JS'i tamamen yüklediğinde
* D) Tarayıcı HTML ve DOM Tree'yi tamamen yüklediğinde

18 - "Bir script dosyasının HTML body ve head kısmında tanımlanması arasında bir fark yoktur."

* A) Doğru
* B) Yanlış

19 - defer ve async arasındaki fark nedir?

* A) defer, sadece Promise lar ile çalışır
* B) defer, synchronous olarak çalışır
* C) defer, sadece head bölümünde kullanılır
* D) defer kullanıldığında scriptlerin çalışması sırayla gerçekleşir