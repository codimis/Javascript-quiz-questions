1)const clothes = ['jacket', 't-shirt'];
clothes.length = 0;

clothes[0]; // => ???

A)jacket
B)null
C)undefined
D)t-shirt

2)const codimis = {
        year : 2021,
        month: 3,
        howIsKahoot : function howIsKahoot(){
            return "awesome";
        }
}
const lesson = "JavaScript";
console.log(codimis.lesson);

A)JavaScript
B)null
C)undefined
D)awesome


3)const person1 = {
    age: 27,
    name: "Bob"
}

const person2 = person1;

person1.age = 10;

console.log(person1.age);
console.log(person2.age);

A) 27-27
B) 10-27
C) 10-10
D) Bob-Bob


4)const a = {},
    b = {c:'b'},
    c = {b:'c'};

a[b] = 111;
a[c] = 333;

console.log(a[b]);

A)111
B)333
C)undefined
D)b

5)const object = {
  message: 'Hello, World!',

  getMessage() {
    const message = 'Hello, Earth!';
    return this.message;
  }
};
console.log(object.getMessage());

A)undefined
B)Hello, Earth!
C)Hello, World!
D){message:"Hello, World!}


6)"Aşağıdaki kod çıktısında console'a hiçbir değer basılmaz"

const wolverine = {
    firstName: 'Logan',
    height: 158,
    strenght: 35,
    fightingSkills: 95,
    friends: ['storm', 'theProffesor', 'cyclops']
};
 
for (let i = 0; i < wolverine.length; i++) {
    console.log(wolverine[i]);
}

True
False

7)Aşağıdakilerden hangisi doğrudur?

const bird = {
  size: 'small',
};

const mouse = {
  name: 'Mickey',
  small: true,
};

A: mouse.bird.size is not valid
B: mouse[bird.size] is not valid
C: mouse[bird["size"]] is not valid
D: All of them are valid


8)Aşağıdaki kodun çıktısı ne olur?

function getAge() {
  'use strict';
  age = 21;
  console.log(age);
}

getAge();

A: 21
B: undefined
C: ReferenceError
D: TypeError

9)Aşağıdaki kodun çıktısı ne olur?

const obj = { a: 'one', b: 'two', a: 'three' };
console.log(obj);

A: { a: "one", b: "two" }
B: { b: "two", a: "three" }
C: { a: "three", b: "two" }
D: SyntaxError
10)Aşağıdaki kodun çıktısı ne olur?

for (let i = 1; i < 5; i++) {
  if (i === 3) continue;
  console.log(i);
}

A: 1 2
B: 1 2 3
C: 1 2 4
D: 1 3 4

11)Aşağıdaki kodun çıktısı ne olur?

const shape = {
  radius: 10,
  diameter() {
    return this.radius * 2;
  },
  perimeter: () => 2 * Math.PI * this.radius,
};

console.log(shape.diameter());
console.log(shape.perimeter());

A: 20 and 62.83185307179586
B: 20 and NaN
C: 20 and 63
D: NaN and 63

12)Aşağıdaki kodun çıktısı ne olur?

let c = { greeting: 'Hey!' };
let d;

d = c;
c.greeting = 'Hello';
console.log(d.greeting);

A: Hello
B: Hey!
C: undefined
D: ReferenceError

13) Objelerdeki tanımlarken özelliklerin alfabetik sıraya göre olması gerekir.
A: Doğru
B: Yanlış

14) Objelerin alanlarına ulaşırken dot(nokta) notation(gösterim) ile birlikte expression kullanabiliriz.
A: Doğru
B: Yanlış

15) Obje tanımlarken objelerin özelliklerinin isimlendirilmesinde reserved keyword(özel tanımlı kelimeler) kullanılabilir.
A: Doğru
B: Yanlış

16) 
const human = {
  age: 28,
  name: 'Uğur',
  calcBirthYear : function() {
    return 2021 - age;
  }
};

console.log(human.calcBirthYear());

A: 1993
B: null
C: undefined
D: ReferenceError

17) 
const _human = {
  'yaş': 28,
  name: 'Uğur',
  calcBirthYear : function() {
    return 2021 - this['yaş'];
  }
};

console.log(_human.calcBirthYear());

A: 1993
B: null
C: SyntaxError
D: ReferenceError

18) Aşağıdaki kodun çıktısı ne olur?
 
for (let i = 1; i < 5; i++) {
  console.log(i);
  if (i === 2) break;
}


A: 1 
B: 1 Nan 3 4
C: 1 2
D: 1 3 4

19) Çıktısı ne olur?
for(let i = 0; i < 10; i = i+3) {
  console.log(i);
}


A: 0 3 6 9
B: 3 6 9
C: 0 3 6 
D: 0 3 6 9 NaN


20) Çıktısı ne olur?
for(let i = 0; ; i++) {
  console.log(i);
}


A: SyntaxError
B: ReferenceError
C: Infinite Loop
D: 0 1 2 3 4 5 6 7 8 9 10

21) Prettier hangi işe yarar?

A: Yazılan kodu renklendirir.
B: Daha hızlı kod yazmak için kullanılır.
C: Yazılan kodu okunurluğunu arttırmak için formatlama yapar.
D: Javascript kodunu editörde çalıştırmaya yarar.

22) 
for (let i = 1; i < 5; i++) {
  console.log(i);
  if (i === 2) return i;
}

A: 1 
B: SyntaxError
C: 1 2
D: ReferenceError


23) 
function calc() {
for (let i = 1; i < 5; i++) {
  console.log(i);
  if (i === 2) return i;
}
}

calc();

A: 1 
B: SyntaxError
C: 1 2
D: ReferenceError
