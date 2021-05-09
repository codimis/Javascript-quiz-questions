# CODIMIS 
## Javascript Eğitimi Birinci Hafta Soruları
1 - Hangisi doğru bir değişken ismi olarak kullanılamaz? 
* A) apple 
* B) threeBirds 
* C) .toYears 
* D) a4Size

2 - Hangisi javascript için özel kelime (reserved keyword) değildir? (reserved keywords için kaynak : https://www.w3schools.com/js/js_reserved.asp)
* A) new 
* B) for 
* C) false 
* D) correct

3 - Hangisi EC5 sonrasında özel kelime olarak eklenmemiştir? 
* A) final 
* B) class 
* C) let 
* D) enum

4 - Hangisi EC5 sonrasında özel kelime olmaktan çıkarılmıştır? 
* A) throws 
* B) with 
* C) super 
* D) import


5 - Hangisi bir değişken isimlendirme stili değildir? 
* A) kebab case 
* B) worm case  
* C) snake case 
* D) camel case

6 - Hangisi javascript data tiplerinden birisidir? 
* A) Decimal 
* B) BigInt 
* C) Float 
* D) Int

7 - Hangisi javascript değişkeni tanımlamak için kullanılmaz? 
* A) var 
* B) for 
* C) let 
* D) const

8 - Hangisi hatasız bir değişken tanımlamasıdır? 
* A) let day = 5;  
* B) const YEAR; 
* C) const 5years = 5; 
* D) var = 3days;

9 - Hangisinin data tipi number değildir? 
* A) 1963 
* B) NaN 
* C) null 
* D) 23.3

10 - '19' === 19 işleminin sonucu nedir? 
* A) true 
* B) false

11 - (true and false) işleminin sonucu nedir? 
* A) true 
* B) false

12 - (!true || false) işleminin sonucu nedir? 
* A) true 
* B) false

13 - If statement aşağıdakilerden hangisi için kullanılır? 
* A) Tekrar eden işlemleri gerçekleştirmek için 
* B) Koşula bağlı tekrar eden işlemleri gerçekleştirmek için 
* C) Koşula bağlı işlemleri gerçekleştirmek için 
* D) Obje oluşturmak için

14 - Çıktısı ne olur?

```javascript
console.log(+true);
console.log(!'Codimis');
```

* A) +true, !'Codimis' 
* B) 1, false 
* C) 0, true
* D) 1, 'Codimis'

15 - Çıktısı ne olur?

```javascript
let a = 5;
let b = new Number(5);
let c = '5';

console.log(a == b);
console.log(a === b);
console.log(b === c);
```

* A) false, false, false
* B) true, true, true
* C) true, false, false
* D) true, true, false

16 - Çıktısı ne olur?

```javascript
function sum(a, b) {
  return a + b;
}

console.log(sum(2, '3'));
```

* A) NaN
* B) "23"
* C) Syntax Error
* D) 5

17 - Çıktısı ne olur?

```javascript
let number = 1;
console.log(number++);
console.log(++number);
console.log(number);
```

* A) 1 2 3
* B) 2 2 3
* C) 1 3 3
* D) 2 3 3

18 - Çıktısı ne olur?

```javascript
var num = 8;
var num = 10;

console.log(num);
```

* A) 8
* B) 10
* C) Syntax Error
* D) Reference Error


19 - Çıktısı ne olur?

```javascript
console.log(typeof typeof 1);
```

* A) "number"
* B) "string"
* C) "object"
* D) "undefined"

20 - Çıktısı ne olur?

```javascript
console.log(!!null);
console.log(!!'');
console.log(!!1);
```

* A) false, false, false
* B) true, true, true
* C) false, false, true
* D) false, true, true

21 - Çıktısı ne olur?
```javascript
console.log(30/5*2);
```

* A) 3
* B) 12
* C) 36
* D) 1.2


22 - Çıktısı ne olur?
```javascript
x = 5;
var x;
console.log(x);
```

* A) ReferenceError
* B) SyntaxError
* C) 5
* D) undefined


23 - Çıktısı ne olur?
```javascript
x = 5;
let x;
console.log(x);
```

* A) ReferenceError
* B) SyntaxError
* C) 5
* D) undefined

24 - Çıktısı ne olur?
```javascript
var a = 'a'/5;
var b = 'b'/5;
if (a === b) {
  console.log("a b'ye eşit");
} else {
  console.log("a b'ye eşit değil");
}
```

* A) a b'ye eşit
* B) a b'ye eşit değil
* C) ReferenceError
* D) undefined

25 - Çıktısı ne olur?
```javascript
if (NaN === NaN) {
  console.log("NaN ve NaN eşittir");
} else {
  console.log("NaN ve NaN eşit değildir");
}
```

* A) NaN ve NaN eşittir
* B) NaN ve NaN eşit değildir
* C) ReferenceError
* D) SyntaxError


26 - Çıktısı ne olur?
```javascript
var x = 10;
if (true) {
  var x = 15;     
  console.log(x);
}
console.log(x);
```

* A) 15, 15
* B) 10, 10
* C) 15, 10
* D) 10, 15


27 - Çıktısı ne olur?
```javascript
let x = 10;
if (true) {
  let x = 15;     
  console.log(x); 
}
console.log(x);
```

* A) 15, 15
* B) 10, 10
* C) 15, 10
* D) 10, 15

28 - Değişkenin tipini değiştirmeden karşılaştırma yapmak için hangisi kullanılır?

* A) =
* B) ==
* C) ===
* D) typeof

29 - Çıktısı ne olur?

```javascript
/* console.log(1); */
// console.log(2);
console.log(3);
```

* A) 1
* B) 1, 2, 3
* C) 3
* D) 2

30 - Çıktısı ne olur?

```javascript
var x, y = 42;
console.log(x);
```

* A) 42
* B) null
* C) undefined
* D) ReferenceError

31 - Switch-case kullanırken break statementını yazmazsak ne olur?

* A) Default case ile çalışmaya devam eder.
* B) Çalışma sırasında hata verir.
* C) Switch-case çalışmaz.
* D) Bir sonraki case ile çalışmasını sürdürür.

32 - Çıktısı ne olur?

```javascript
let result = 100 + "200"
```

* A) NaN
* B) 300
* C) 100200
* D) TypeError


33 - Çıktısı ne olur?

```javascript
let result = 10;
result += 5;
console.log(result);
```

* A) 10
* B) 15
* C) 25
* D) NaN

34- Çıktısı ne olur?
```javascript
let score = 85;
let grade = score >= 80 ? "A" : "B";

console.log(`Your exam grade is ${grade}`);
```
* A) Your exam grade is A
* B) Your exam grade is B
