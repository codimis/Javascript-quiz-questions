# CODIMIS 

## Javascript Eğitimi Ondördüncü Hafta Soruları

1 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const x = 0.1
const y = 0.2

console.log(x+y === 0.3);
```

* A) Doğru
* B) Yanlış

2 - parseInt() gibi global function ları objesi olmadan çağırabiliriz.

* A) Doğru
* B) Yanlış

3 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const num = parseInt('7*6', 10);
console.log(num);
```

* A) 42
* B) "42"
* C) 7
* D) NaN

4 - Aşağıdaki kodun çıktısı ne olur?
```javascript
let str = "1";
str = +!str;
console.log(typeof str)
```

* A) "boolean"
* B) "number"
* C) "string"
* D) "NaN"

5 - Aşağıdaki kodun çıktısı ne olur?
```javascript
if(Math.max([ 0 ], [ 1 ]) > Math.max(true,false)) {
    console.log("array won");
} else {
    console.log("array lost");
}
```

* A) array won
* B) array lost
* C) Error

6 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const x = 6 % 2;
const y = x ? 'One' : 'Two';
console.log(y);
```

* A) 'One'
* B) undefined
* C) TRUE
* D) 'Two'

7 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const result = 1n + 2n
console.log(typeof result);
```

* A) Number
* B) String
* C) BigInt
* D) NaN

8 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const x  = Number.MAX_SAFE_INTEGER + 1;
const y = Number.MAX_SAFE_INTEGER + 2;

console.log( x === y );
```

* A) Doğru
* B) Yanlış

9 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const date = new Date();
console.log(date.toISOString().slice(0,4));
```

* A) July
* B) 2021
* C) 06-29
* D) Error

10 - Aşağıdaki kodun çıktısı ne olur?
```javascript
console.log(Date.now() == new Date());
```

* A) Doğru
* B) Yanlış

11 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const date1 = new Date();
const date2 = new Date(0);

if(date1 === date2) {
    console.log("equal");
} else {
    console.log("not so much");
}
```
* A) equal
* B) not so much
* C) Error

12 - Aşağıdaki kodun çıktısı ne olur?
```javascript
console.log(typeof(Number.parseInt('a56px')));
```

* A) number
* B) string
* C) undefined
* D) null

13 - Aşağıdaki kodun çıktısı ne olur?
```javascript
let num = +'5x';
let num2 = 5/0;
if (isNaN(num) && isFinite(num2)) {
  console.log('a')
} else if (Number.isInteger(num2) && isFinite(num)) {
  console.log('b')
} else if (Number.isInteger(num) || isFinite(num2)) {
  console.log('c')
} else if (Number.isInteger(num) || isNaN(num)) {
  console.log('d')
}
```

* A) a
* B) b
* C) c
* D) d

14 - Aşağıdaki Math fonksiyonlarından hangisi sayıyı en yakın integer değerine tamamlar? (https://stackoverflow.com/a/38714503/4894891)

* A) round
* B) ceil
* C) trunc
* D) floor

15 - Aşağıdaki kodun çıktısı ne olur?
```javascript
console.log(typeof((2/3).toFixed(2)))
```

* A) number
* B) string
* C) undefined
* D) null

16 - Aşağıdaki kodun çıktısı ne olur?
```javascript
console.log(5n+4);
```

* A) 9
* B) 5n4
* C) Error
* D) 9n

17 - Aşağıdaki kodun çıktısı ne olur?
```javascript
for (var i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}

for (var i = 0; i < 3; i++) {
    (function(x) {
        setTimeout(function() { console.log(x); }, x * 1000 );
    })(i);
}

for (let i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}
```

A) 0 1 2 ve 0 1 2 ve 0 1 2
B) 0 1 2 ve 0 1 2 ve 3 3 3
C) 3 3 3 ve 0 1 2 ve 0 1 2
D) 3 3 3 ve 3 3 3 ve 0 1 2

18 - Aşağıdaki kod parçası için şıklardan hangisi doğrudur?
```javascript
let config = {
  alert: setInterval(() => {
    console.log('Alert!');
  }, 1000),
};

config = null;
```

A) console'da hiçbir şey yazmayacak
B) console'da bir kez Alert! yazacak
C) console'da her saniye Alert! yazacak
D) console'da bir kez null yazacak

19 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function func1(){
  setTimeout(()=>{
    console.log(x);
    console.log(y);
  },3000);

  var x = 2;
  let y = 12;
}

func1();
```

* A) undefined ve error
* B) 2 ve error
* C) undefined ve 12
* D) 2 ve 12

20 - Aşağıdaki kod parçasında çıktı hangi sırayla gelir?
```javascript
(function() {
  console.log(1);
  setTimeout(function() {
    console.log(2);
  }, 1000);
  setTimeout(function() {
    console.log(3);
  }, 0);
  console.log(4);
})();
```

* A) 1,2,3,4
* B) 4,2,1,3
* C) 1,4,3,2
* D) 4,3,2,1

21 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function getFine(speed, amount) {
  const formattedSpeed = new Intl.NumberFormat('en-US', {
    style: 'unit',
    unit: 'mile-per-hour'
  }).format(speed);

  const formattedAmount = new Intl.NumberFormat('en-US', {
    style: 'currency',
    currency: 'USD'
  }).format(amount);

  return `The driver drove ${formattedSpeed} and has to pay ${formattedAmount}`;
}

console.log(getFine(130, 300))
```

* A) The driver drove 130 and has to pay 300
* B) The driver drove 130 mph and has to pay $300.00
* C) The driver drove undefined and has to pay undefined
* D) The driver drove 130.00 and has to pay 300.00
