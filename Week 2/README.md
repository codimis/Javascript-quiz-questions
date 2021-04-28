# CODIMIS 
## Javascript Eğitimi İkinci Hafta Soruları
1 - Strict mode hangisini önlemez? 
* A) Değişkenleri var, let, const olmadan tanımladığımızda hata dönmesini sağlar
* B) Fonksiyon parametrelerinde aynı isimle değişken tanımlanmasını önler
* C) JavaScript anahtar kelimelerini kullanıldığında hata verilmesini sağlar
* D) Tekrar etmeyen kod yazmamızı sağlar
  
2 - Function declaration ve function expression arasındaki farklardan biri değildir?
* A) Function expression kullanırken fonksiyon ismi yazmadan tanım yapılabilir
* B) Function declaration tanımlandığı yerden önce çağrılabilir
* C) Function expression tanımlandığı yerden önce çağrılabilir 
* D) Function declaration kullanırken fonksiyon ismi yazmak zorunludur

3 - Bir fonksiyonu hangisini kullanmak için yazmayız? 
* A) Tekrar edecek kod parçalarını tek bir yerde yazmak için 
* B) Özel tanımlı bir işlemi tek bir yerden yönetmek için 
* C) Değişken tanımlamak için 
* D) Hiçbiri

4 - Return anahtar kelimesi ne için kullanılır? 
* A) Fonksiyonu bir koşula göre çalıştırmaya 
* B) Fonksiyonun bir değer dönmesine 
* C)  Fonksiyonun çağırılmasına 
* D) Fonksiyonun çalıştırılmasına

5 - Arrow fonksiyonu return anahtar kelimesi kullanmadan değer dönmesine olanak tanır. 
* A) Doğru 
* B) Yanlış

6 - DRY konsepti neyi ifade eder? 
* A) Bir fonksiyondan başka bir fonksiyonu çağırmayı 
* B) Kendini tekrar etmemeyi 
* C) Okunabilir kod yazılmasını 
* D) Hepsi

7 - Aşağıdakilerden hangisi doğrudur? 
* A) Fonksiyonda returnden sonra olan kodlar return işlemi sonrasında çalışır 
* B) Function expression ile tanımlana fonksiyon tanımlandığı satırdan önce kullanılabilir 
* C) Fonksiyon içinde başka bir fonksiyon çağırılabilir. 
* D) Arrow fonksiyonlarında hiçbir zaman return yazmaya gerek yoktur.

8 - Javascriptte array indeksi kaçtan başlar? 
* A) 1 
* B) 0 
* C) 1 
* D) 2

9 - const ile tanımlanmış olan bir dizi(array) üzerinde değişiklik yapılabilir. 
* A) Doğru 
* B) Yanlış

10 - Diziler hakkındaki aşağıdaki bilgilerden hangisi doğrudur? 
* A) Dizilerin içinde dizi bulunamaz 
* B) Diziler sadece aynı veri tipindeki değerleri tutabilirler 
* C) Dizilerin içine değişken konulamaz 
* D) Dizilerin uzunluğu length ile bulunabilir

11 - Dizinin ilk indeksine eleman eklemek için hangi array fonksiyonu kullanılır? 
* A) unshift 
* B) shift 
* C) pop 
* D) push

12 - "Dizide bulunan elemanları includes fonksiyonu ile kontrol ettiğimizde..." cümlesini aşağıdakilerden hangisi ile bitiremezsiniz? 
* A) Eğer eleman varsa true döner 
* B) Eğer eleman yoksa false döner 
* C) Eğer eleman varsa veri tipi farklı olsa da true döner 
* D) Hiçbiri

13 - Aşağıdakilerden hangisi yanlıştır? 
* A) Pop fonsiyonu tamamlandıktan sonra çıkarılan elemanı döner 
* B) Shift fonsiyonu tamamlandıktan sonra çıkarılan elemanı döner 
* C) Unshift fonsiyonu tamamlandıktan sonra çıkarılan elemanı döner 
* D) Push fonsiyonu tamamlandıktan sonra çıkarılan dizinin uzunluğunu döner

14 - Çıktısı nedir?
```javascript
var a = 1
function foo(){
 var a = 2
 console.log(a)
}
foo()
console.log(a);
```
* A) 1,1  
* B) 2,2   
* C) 2,1   
* D) 1,2

15 - Çıktısı nedir?
```javascript
function evaluate() {
  console.log(brand);
  console.log(point);
  var brand = "Codimis";
  let point = 10;
}

evaluate();
```
* A) Codimis ve undefined
* B) Codimis ve ReferenceError
* C) ReferenceError ve 10
* D) undefined ve ReferenceError

16 - Çıktısı nedir?
```javascript
let arr =[1,2]
function test(array){
  array.push(3)
}
test(arr)
console.log(arr)
```
* A) [1,2]
* B) [1,2,3]
* C) [3,1,2]
* D) [1,3,2]

17 - Çıktısı nedir?
```javascript
let car;
var tire;
car = 'toyota';
tire = 4;
console.log(car, tire);
```
* A) toyota, 4 
* B) 4, toyota
* C) ReferenceError, undefined
* D) undefined, undefined

18 - Çıktısı nedir?
```javascript
let newCar;
var import;
car = 'toyota';
tire = 4;
console.log(car, tire);
```
* A) ReferenceError
* B) 4 toyota
* C) SyntaxError
* D) undefined, undefined

19 - Çıktısı nedir?
```javascript
var array = [];
console.log(array.pop());
```
* A) null
* B) undefined
* C) []
* D) Hiç bir şey yazmaz

20 - Çıktısı nedir?
```javascript
var array = [null,"ali", NaN, "", ,];
console.log(array.length);
```
* A) 4
* B) 5
* C) 6
* D) 3

21 - Çıktısı nedir?
```javascript
const x = [];
x.push("Hello", "World!");
console.log(x);
```
* A) ["Hello", "World!"]
* B) TypeError
* C) ReferenceError
* D) SyntaxError

22 - Çıktısı nedir?
```javascript
const x = [];
x = ["Hello", "World!"];
console.log(x);
```
* A) ["Hello", "World!"]
* B) TypeError
* C) ReferenceError
* D) SyntaxError


23 - Çıktısı ne olur?

```javascript
function foo(a, b, c) {
  console.log( b );
}
foo( 4, 5, 6 );
```

* A) 4
* B) 5
* C) 6
* D) b

24 - Çıktısı ne olur?

```javascript
let arr = [ 1, 2, 3 ];
console.log( arr[3] );
```

* A) 1
* B) 2
* C) 3
* D) undefined

25 - Çıktısı ne olur?

```javascript
var message = "no";
function foo(message) {
  message = "yes";
}
foo( message );
console.log( message );
```

* A) TypeError
* B) undefined
* C) no
* D) yes

