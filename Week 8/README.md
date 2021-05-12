# CODIMIS 
## Javascript Eğitimi Sekizinci Hafta Soruları

1- "Arrow function ile tanımlanandan fazla parametre almak için arguments kullanılır."
   
* A) Doğru
* B) Yanlış
  
2- "İçi boş olan bir javascript dosyasını bile yüklediğimizde, global execution context oluşur."
   
* A) Doğru
* B) Yanlış
  
3- Aşağıdaki kodun çıktısı ne olur?
```javascript
var firstname = computeName();

let name = "Caner";

function computeName() {
  return `${name} Unal`;
}

console.log(firstname);
```
* A) Caner Unal
* B) undefined Unal
* C) ReferenceError
* D) SyntaxError

4- Aşağıdaki kodun çıktısı ne olur?
```javascript
const shape = {
  radius: 10,
  diameter() {
    return this.radius * 2;
  },
  perimeter: () => 2 * Math.PI * this.radius,
};

console.log(shape.diameter());
console.log(shape.perimeter());
```
* A) 20 and 62.83185307179586
* B) 20 and NaN
* C) 20 and 63
* D) NaN and 63

5- Aşağıdaki kodun çıktısı ne olur?

```javascript
function a() {
    let c = 'Hello';
}

function b() {
    a();
    console.log(c);
}

console.log(b());
```
* A) Hello
* B) ReferenceError
* C) undefined
* D) SyntaxError

6- Aşağıdaki kodun çıktısı ne olur?
```javascript
const animals = ['Cow', 'Horse', 'Dog', 'Cat', 'Rabbit'];
for(let i=0; i<animals.length; i++){
    const animals = ['Whale', 'Dolphin'];
    console.log(animals[i]);
}
```
* A) Whale, Dolphin, Dog, Cat, Rabbit
* B) Cow, Horse, Dog, Cat, Rabbit
* C) Whale, Dolphin, undefined, undefined, undefined
* D) Whale, Dolphin

7- Aşağıdaki kodun çıktısı ne olur?
```javascript
function foo() {
    function bar() {
        console.log(someVar);
    }
    var someVar = 10;
    bar()
}

var someVar = 20;
foo()
```
* A) 20
* B) 10
* C) undefined
* D) ReferenceError

8- Aşağıdaki kodun çıktısı ne olur?
```javascript
function calcAge(birthDate) {
  const age = 2021 - birthDate;
  if (age > 15) {
     console.log(firstName);
  }
  var firstName = "Caner";
  return age;
}
const firstName = "Codimis";
calcAge(2000);
```
* A) Codimis
* B) Caner
* C) null
* D) undefined

9- Aşağıdaki kodun çıktısı ne olur?
```javascript
function calcAge(birthDate) {
  const age = 2021 - birthDate;
  console.log(firstName);
  return age;
}
calcAge(2000);
const firstName = "Codimis";
```
* A) Codimis
* B) 21
* C) undefined
* D) ReferenceError

10- Aşağıdaki kodun çıktısı ne olur? 
```javascript
function scopeQuestion() {
  let name = "Codimis";
  function innerFunction() {
    if(!name) {
      console.log(name);
      let name = "Test";
    } else {
      console.log("Fail");
    }
    var name = "Scope";
  }
  innerFunction();
}
const name = "Test";
scopeQuestion();
```
* A) ReferenceError
* B) Test
* C) Scope
* D) Fail

11- Aşağıdaki kodun çıktısı ne olur?
```javascript
function scopeQuestion() {
  let name = "Codimis";
  function innerFunction() {
    var name = "Scope";
    console.log(name);
  }
  innerFunction();
}
const name = "Test";

function thirdFunction() {
  innerFunction();
}

thirdFunction();
```
* A) Codimis
* B) Test
* C) Scope
* D) ReferenceError

12- Aşağıdaki kodun çıktısı ne olur?
```javascript
let c = { greeting: 'Hey!' };
let d;

d = c;
c.greeting = 'Hello';
console.log(d.greeting);
```
* A) Hello
* B) Hey!
* C) undefined
* D) ReferenceError

13- Aşağıdaki kodun çıktısı ne olur?
```javascript
const person1 = {
    age: 27,
    name: "Bob"
}

const person2 = person1;

person1.age = 10;

console.log(person1.age);
console.log(person2.age);
```
* A) 27-27
* B) 10-27
* C) 10-10
* D) Bob-Bob
