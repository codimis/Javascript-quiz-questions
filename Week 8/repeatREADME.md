1 - Aşağıdaki kodun çıktısı ne olur?
```javascript
var v = 1;
var f1 = function () {
  console.log(v);
};

var f2 = function () {
  var v = 2;
  f1();
};

f2();
```

 * A) 2
 * B) 1
 * C) Error
 * D) undefined

2 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const obj1 = {
  a : "Apple",
  showA : function() {
    console.log(this.a);
  }
}

const obj2 = obj1;

obj2.a = "Banana";

obj1.showA();
```

* A) Error
* B) Apple
* C) Banana
* D) undefined

3 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const mySet = new Set([{ a: 1 }, { a: 1 }]);
const result = [...mySet];
console.log(result);
```

* A) [{a: 1}, {a: 1}] 
* B) [{a: 1}]
* C) Error
* D)

4 - Aşağıdaki kodun çıktısı ne olur?
```javascript
console.log(a)
console.log(b)
var a = 2
let b = 2
```

* A) 2 - 2
* B) undefined - 2
* C) undefined - Error
* D) Error - Error

5 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const a = false;
const result = a ?? "Hello";
console.log(result);
```

* A) false
* B) "Hello"

6 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const func = () => 'here';
const a = !! '   ';
const b = 1 && 2 && 3
const c = '' && false && NaN
const d = false || 2 || 3
const e = 1 && func && func();
console.log(a,b,c,d,e);
```

* A) false 1 '' false 1
* B) true 3 NaN 3 'here'
* C) true 3 '' 2 'here'
* D) true 1 NaN false undefined

String videosu kontrol edilecek
7 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const a = "Backbencher";
const b = new String("Backbencher");
console.log(a === b);
```

* A) true
* B) false

8 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const user = { name: 'Caner', age: 28 };
const admin = { admin: true, ...user };

console.log(admin);
```

* A) { admin: true, user: { name: "Caner", age: 21 } }
* B) { admin: true, name: "Caner", age: 28 }
* C) { admin: true, user: ["Caner", 21] }
* D) { admin: true }

9 - Aşağıdaki metodlardan hangisi "bird" String inin 4. indexte olduğu belirtir?

```javascript
const word = 'The bird is the word';
```

* A) length
* B) indexOf
* C) find
* D) split

10 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const animals = {};
let dog = { emoji: '🐶' }
let cat = { emoji: '🐈' }

animals[dog] = { ...dog, name: "Mara" }
animals[cat] = { ...cat, name: "Sara" }

console.log(animals[dog])

```

* A) { emoji: "🐶", name: "Mara" }
* B) { emoji: "🐈", name: "Sara" }
* C) undefined
* D) ReferenceError