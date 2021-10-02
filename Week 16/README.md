# CODIMIS 

## Javascript Eğitimi Object Oriented Programming Soruları

1 - "Constructor function ile Object oluşturma yöntemi Arrow functionlar ile yapılamaz."

* A) Doğru
* B) Yanlış

2 - "Prototype'a bir fonksiyon tanımladığımızda o prototype'a sahip instancelara fonksiyon kopyalanır."

* A) Doğru
* B) Yanlış

3 - Aşağıdaki kodun çıktısı ne olur?

```javascript
 const Car = function (make, speed) {
   this.make = make;
   this.speed = speed;   
 };

Car.prototype.tyre = "Michelin";

const bmw = new Car('BMW', 120);
const mercedes = new Car('Mercedes',95);

console.log(bmw.hasOwnProperty('tyre'));
console.log(mercedes.__proto__ === Car.prototype); 
console.log(bmw instanceof Object);
```

* A) false false false
* B) false true true
* C) true true true
* D) true true false

4 - Aşağıdaki dizi için prototype chain'de kaç tane object vardır?

```javascript
let arr = [];
```

* A) 3
* B) 2
* C) 1
* D) 0

5 - Aşağıdaki kodun çıktısı ne olur?

```javascript
function Dog(name) {
  this.name = name;
  this.speak = function() {
    return 'woof';
  };
}

const dog = new Dog('Pogo');

Dog.prototype.speak = function() {
  return 'arf';
};

console.log(dog.speak());
```

* A) woof
* B) arf
* C) undefined
* D) Error

6 - Aşağıdaki kodun çıktısı ne olur?

```javascript
class Counter {
  constructor() {
    this.count = 0;
  }

  increment() {
    this.count++;
  }
}

const counterOne = new Counter();
counterOne.increment();
counterOne.increment();

const counterTwo = counterOne;
counterTwo.increment();

console.log(counterOne.count);
```

* A) 0
* B) 1
* C) 2
* D) 3

7 - Aşağıdaki koda göre X'in bir objesinden 42 sonucunu elde etmek için hangi seçenekteki yazılış doğrudur?

```javascript
class X {
  get Y() {
    return 42;
  }
}
```

* A) x.get('Y')
* B) x.Y
* C) x.Y()
* D) x.get().Y

8 - Aşağıdaki kodun çıktısı ne olur?

```javascript
class Calc {
	constructor() {
		this.count = 0 
	}

	increase() {
		this.count ++
	}
}

const calc = new Calc()
new Calc().increase()

console.log(calc.count)
```

* A) 0
* B) 1
* C) undefined
* D) ReferenceError

9 - TaxCalculator classını kullanarak 50 doların vergisini nasıl hesaplarız?

```javascript
class TaxCalculator {
  static calculate(total) {
    return total * 0.05;
  }
}
```

* A) calculate(50);
* B) new TaxCalculator().calculate($50);
* C) TaxCalculator.calculate(50);
* D) new TaxCalculator().calculate(50);

10 - Aşağıdaki kodun çıktısı ne olur?

```javascript
function Person(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}

const member = new Person('Caner', 'Unal');
Person.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

console.log(member.getFullName());
```

* A) TypeError
* B) ReferenceError
* C) Caner Unal
* D) undefined undefined

11 - Aşağıdaki kodun çıktısı ne olur?

```javascript
String.prototype.giveDefaultQuestionTitle = () => {
  return 'Aşağıdaki kodun çıktısı ne olur?';
};

const name = 'Caner';

console.log(name.giveDefaultQuestionTitle());
```

* A) "Aşağıdaki kodun çıktısı ne olur?"
* B) TypeError: not a function
* C) SyntaxError
* D) undefined

12 - Aşağıdaki kodun çıktısı ne olur?
```javascript
class Person {
  constructor(name) {
    this.name = name;
  }
}

const member = new Person('John');
console.log(typeof member);
```

* A) "class"
* B) "function"
* C) "object"
* D) "string"
  
13 - Aşağıdaki kodun çıktısı ne olur?
```javascript
class Chameleon {
  static colorChange(newColor) {
    this.newColor = newColor;
    return this.newColor;
  }

  constructor({ newColor = 'green' } = {}) {
    this.newColor = newColor;
  }
}

const freddie = new Chameleon({ newColor: 'purple' });
console.log(freddie.colorChange('orange'));
```

* A) orange
* B) purple
* C) green
* D) TypeError

14 - "Bir objenin fieldlarını private yapıp, erişiminin kısıtlanması encapsulation prensibi ile ilişkilidir"

* A) Doğru
* B) Yanlış

15 - Aşağıdaki kodun çıktısı ne olur?
```javascript
class Counter {
  #number = 10

  increment() {
    this.#number++
  }

  getNum() {
    return this.#number
  }
}

const counter = new Counter()
counter.increment()

console.log(counter.#number)
```

* A) 10
* B) 11
* C) undefined
* D) SyntaxError

16 - Hangi seçenekteki constructor ile Dog classı başarıyla extend edilmiştir?
```javascript
class Dog {
  constructor(name) {
    this.name = name;
  }
};

class Labrador extends Dog {
  // 1
  constructor(name, size) {
    this.size = size;
  }
  // 2
  constructor(name, size) {
    super(name);
    this.size = size;
  }
  // 3
  constructor(size) {
    super(name);
    this.size = size;
  }
  // 4
  constructor(name, size) {
    this.name = name;
    this.size = size;
  }

};
```

* A) 1
* B) 2
* C) 3
* D) 4

17 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const Person = function (name){
  this.name = name;

  this.sayHello = function(){
    console.log("instance method say hello");
  }
}
Person.prototype.sayHello = function(){
  console.log("prototype method say hello");
}
const p = new Person("Caner");
p.sayHello();
```
* A) undefined
* B) "instance method say hello"
* C) "prototype method say hello"
* D) Error

18 - caner.greeting() "Hello" yu print eder

```javascript
class Person{
  constructor(name,job){
    this.name = name;
    this.job = job;
  }
  static greeting() {
    console.log("Hello");
  }
}
const caner = new Person('Caner','Developer');
caner.greeting();
```

* A) Doğru
* B) Yanlış

19 - Aşağıdaki kodun çıktısı ne olur?

```javascript
 const Car = function (make, speed) {
   this.make = make;
   this.speed = speed;   
 };

 const LuxuryCar = function (make,speed,price){
   Car.call(this,make,speed);
   this.price = price;
 }

 LuxuryCar.prototype = Object.create(Car.prototype);
 LuxuryCar.prototype.constructor = Car;
 const mercedes = new LuxuryCar('Mercedes',195,500000);
 Car.prototype.tyre = "Michelin";


console.log(mercedes.hasOwnProperty('tyre'));
console.log(mercedes.__proto__ === Car.prototype); 
console.log(mercedes instanceof Car);
```

* A) true true true
* B) false true true
* C) false false true
* D) false true false

20 - Aşağıdaki inheritance örneğinde accelerate() fonksiyonu EVCl classında override edilerek OOP'nin hangi prensibi uygulanmıştır?
```javascript
class CarCl {
  constructor(make,speed){
    this.make = make;
    this.speed = speed;
  }
  accelerate() {
    this.speed+=10;
    console.log(this.speed);
  }
}
class EVCl extends CarCl {
  constructor(make,speed,charge){
    super(make,speed);
    this.charge = charge;
  }
  accelerate(){
    this.speed+=20;
    console.log("speed changed");
  }
}
```

* A) Abstraction
* B) Inheritance
* C) Encapsulation
* D) Polymorphism

21 - Aşağıdaki kodun çıktısı ne olur?
```javascript
class Bird {
  constructor() {
    console.log("I'm a bird. 🦢");
  }
}

class Flamingo extends Bird {
  constructor() {
    console.log("I'm pink. 🌸");
    super();
  }
}

const pet = new Flamingo();
```

* A) I'm pink. 🌸
* B) I'm pink. 🌸 -  I'm a bird. 🦢
* C) I'm a bird. 🦢 -  I'm pink. 🌸
* D) Nothing, we didn't call any method

22 - square instance'ının alanını elde etmek için hangi seçenekteki kodu kullanırız?
```javascript
class Square {
  constructor(sideLength) {
    this.sideLength = sideLength;
  }

  get area() {
    return this.sideLength * this.sideLength;
  }
}

let square = new Square(5);
```

* A) square.getarea()
* B) square.area
* C) square.area()
* D) Square.area()