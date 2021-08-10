# CODIMIS 
## Javascript Eğitimi Onuncu Hafta Soruları

1- Aşağıdaki kodun çıktısı ne olur?
 ```javascript
function multiply(a) {
  return a;
}

function multiply(a, b) {
  return a * b;
}

console.log(multiply(5, 2)); 
console.log(multiply(5));
```
* A) 10, 5
* B) 10, Undefined
* C) 10, NaN
* D) SyntaxError

2 - Aşağıdaki kodun çıktısı ne olur?

```javascript
function sum(num1, num2 = num1) {
  console.log(num1 + num2);
}

sum(10);
```

* A) NaN
* B) 20
* C) ReferenceError
* D) undefined

3- Aşağıdaki kodun çıktısı ne olur?
```javascript
function test(num = 1) {
  console.log(typeof num)
}

test();
test(undefined); 
test('');
test(null);
```
* A) Number, Undefined, Undefined, Undefined
* B) Number, Undefined, Number, Number
* C) Number, Number, String, Object

4- Aşağıdaki kodun çıktısı ne olur?
```javascript
function add(x = 1,  z = x + y,  y = x) {
    return x + y + z;
}

console.log(add());
```
* A) SyntaxError
* B) 4
* C) ReferenceError
* D) NaN

5- Aşağıdaki kodun çıktısı ne olur?
```javascript
function add(x, y = 1, z = 2) {
    console.log( arguments.length );
    return x + y + z;
}

console.log(add(10));
console.log(add(10,20));
```
* A) 1, 13  - 2, 32
* B) 3, 13  - 3, 32

6- "JavaScript pass by value olarak çalışır"
   
* A) Doğru
* B) Yanlış

7- "Closure manuel olarak oluşturabileceğimiz bir yapıdır"

* A) Doğru
* B) Yanlış

8- Aşağıdaki kodun çıktısı ne olur?
```javascript
const discount = function (price,rate,fixedRate=0.1){
    return price - price * fixedRate - price * rate;
}
console.log(discount(100,0.5));
```

* A) 50
* B) 40
* C) NaN
* D) ReferenceError

9- Aşağıdaki kodun çıktısı ne olur?
```javascript
const person = {
  firstName: 'Caner',
  lastName: 'Unal',
  pet: {
    name: 'Torun',
    breed: 'Chow Chow',
  },
  getFullName() {
    return `${this.firstName} ${this.lastName}`;
  },
};

console.log(person.pet?.name);
console.log(person.pet?.family?.name);
console.log(person.getFullName?.());
console.log(member.getLastName?.());
```
* A) undefined undefined undefined undefined
* B) Torun undefined Caner Unal ReferenceError
* C) Torun null Caner Unal null
* D) null ReferenceError null ReferenceError

10- Aşağıdaki kodun çıktısı ne olur?
```javascript
const person = { name: 'Caner' };

function sayHi(age) {
  return `${this.name} is ${age}`;
}

console.log(sayHi.call(person, 27));
console.log(sayHi.bind(person, 27));
```

* A) undefined is 27 - Caner is 27
* B) function - function
* C) Caner is 27 - Caner is 27
* D) Caner is 27 - function

11- Aşağıdaki kodun çıktısı ne olur?
```javascript
const add = x => x + x;

function myFunc(num = 2, value = add(num)) {
  console.log(num, value);
}

myFunc();
myFunc(3);
```
* A) 2 4 ve 3 6
* B) 2 NaN ve 3 Nan
* C) 2 Error ve 3 6
* D) 2 4 ve 3 Error

12- Aşağıdaki kodun çıktısı ne olur?
```javascript
const add = x => y => {
  console.log(x, y);
  return x + y;
};

add(4)(5);
```
* A) 4 5
* B) 5 4
* C) 4 function
* D) undefined undefined

13 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function compareMembers(person1, person2 = person) {
  if (person1 !== person2) {
    console.log('Not the same!');
  } else {
    console.log('They are the same!');
  }
}

const person = { name: 'Caner' };

compareMembers(person);
```

* A) Not the same!
* B) They are the same!
* C) ReferenceError
* D) SyntaxError

14 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function changeStuff(a, b, c)
{
  a = a * 10;
  b.item = "changed";
  c = {item: "changed"};
}

var num = 10;
var obj1 = {item: "unchanged"};
var obj2 = {item: "unchanged"};

changeStuff(num, obj1, obj2);

console.log(num);
console.log(obj1.item);
console.log(obj2.item);
```
* A) 100, unchanged, unchanged
* B) 10, unchanged, unchanged
* C) 10, changed, unchanged
* D) 10, changed, changed

15 - Aşağıdaki gibi oluşturulduğu anda çalıştırılan fonksiyonlara ne ad verilir?
```javascript
(function () {
    const header = document.querySelector('h1');
    header.style.color = 'red';
    document.querySelector('body').addEventListener('click',function(){
        header.style.color = 'blue';
    });
})();
```
* A) Callback
* B) Higher-Order Function
* C) Function with default parameters
* D) Immediately Invoked Function Expression (IIFE)

16 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const person = {
  name: 'Caner',
  age: 21,
};

const changeAge = (x = { ...person }) => (x.age += 1);
const changeAgeAndName = (x = { ...person }) => {
  x.age += 1;
  x.name = 'Uğur';
};

changeAge(person);
changeAgeAndName();

console.log(person);
```

* A) {name: "Uğur", age: 22}
* B) {name: "Uğur", age: 23}
* C) {name: "Caner", age: 22}
* D) {name: "Caner", age: 23}

17 - Aşağıdaki kodun çıktısı ne olur?

```javascript
(() => {
  y = 10;
  let x = 10;
})();

console.log(typeof x);
console.log(typeof y);
```

* A) "undefined", "number"
* B) "number", "number"
* C) "object", "number"
* D) "number", "undefined"