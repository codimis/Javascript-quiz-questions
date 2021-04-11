# CODIMIS 
## Javascript Eğitimi Beşinci Hafta Soruları
1 - Çıktısı nedir?
```javascript
let a = 1, b = 2;
[a, b] = [b, a];
console.log(a);
console.log(b);
```
* A)1, 1 
* B)1, 2 
* C)2, 1 
* D)2, 2

2 - Çıktısı nedir? 
```javascript
let a = [];
a[5] = 1
console.log(a.length)
```
* A)1 
* B)6 
* C)5 
* D)0

3 - Çıktısı nedir?
```javascript
const a = {
  c:'b',
  toString : function (){
    return "c";
  } 
}
const b = {
  a:'c',
  toString : function (){
    return "a";
  }
}
const c = {
  a:'b',
  toString : function (){
    return "c";
  }
}
a[b]=1;
a[c]=2;
console.log(a[b]);
console.log(a[a]);
```
* A)c, b 
* B)2, 2 
* C)2, b 
* D)1, 2

4 - DOM, JavaScript'in yapısında bulunan özelliklerden biridir 
* A) Doğru 
* B) Yanlış

5 -
``` html
<input type="number" class="guess" />
```
HTML input elementinin değerini 5 ile değiştirmek için document.querySelector('.guess').textContent = 5 kodu yazılır. 
* A) Doğru 
* B) Yanlış

6 - Dom yapısı hangi veri tipinde tutulur? 
* A) Tree 
* B) Stack 
* C) Array 
* D) Queue

7 - Aşağıdakilerden hangisi html elementleri arasındaki bir ilişki tipi değildir? 
* A) child 
* B) parent 
* C) cousin 
* D) sibling

8 - Web api javascriptin temel kütüphanelerinden bir tanesidir. 
* A) Doğru 
* B) Yanlış

9 - WEB API leri ecmascript kurulu tarafından geliştirilir. 
* A) Doğru 
* B) Yanlış

10 - 
```html
<button id="test">Test</button>
<script>
 const testBtn = document.getElementById("test");
  console.log(testBtn);
  testBtn.addEventListener("Click", function() {
    console.log('Codimis');
  })
</script>
```
Görseldeki kodun çalışmamasının sebebi nedir? 
* A) querySelector kullanılmaması.
* B) getElementById fonsiyonuna verilen test stringinin #test olmaması
* C) const ile tanımlanmış testBtn değişkenine event listener verilmesi
* D) Event listener da "click" event tipinin yanlış yazılması

11 - Javascript ile style manipulation yapılırken CSS property(özellik) isimleri hangi şekilde kullanılır? 
* A) CSS yazılırken kullanıldığı stilde 
* B) Özellik adı snake case'e çevrilerek 
* C) Özellik adı kebab case'e çevrilerek 
* D) Özellik adı camel case'e çevrilerek

12 - Çıktısı nedir?
```html
<p id="message">Your message</p>
<p class="message">Their message</p>
<script>
  console.log(document.querySelector(".message"));
</script>
```
* A) ```<p class="message">Their message</p>```
* B) ```<p id="message">Your message</p>```
* C) Your message
* D) Their message

13 - Çıktısı nedir?
```html
<p id="message">Your message</p>
<p class="message">Their message</p>
<script>
  console.log(document.querySelector(".message").value);
</script>
```
* A) undefined
* B) null
* C) Your message
* D) Their message

14 - Çıktısı nedir?

```javascript
let a, b, rest;
[a, b] = [10, 20];

[a, b, ...rest] = [10, 20, 30, 40, 50];

console.log(rest);
```
* A) 50
* B) 40, 50
* C) 30, 40, 50
* D) 50, 40