# CODIMIS
## Javascript Eğitimi Üçüncü Hafta Soruları

1- 
```javascript
const clothes = ['jacket', 't-shirt'];
clothes.length = 0;

clothes[0]; // => ???
```
- A) jacket
- B) null
- C) undefined
- D) t-shirt

2- 
```javascript
const codimis = {
        year : 2021,
        month: 3,
        howIsKahoot : function howIsKahoot(){
            return "awesome";
        }
}
const lesson = "JavaScript";
console.log(codimis.lesson);
```

- A)JavaScript
- B)null
- C)undefined
- D)awesome

3- 
```javascript
const a = {},
    b = {c:'b'},
    c = {b:'c'};

a[b] = 111;
a[c] = 333;

console.log(a[b]);
```
- A) 111
- B) 333
- C) undefined
- D) b

4-
 ```javascript
 const object = {
  message: 'Hello, World!',

  getMessage() {
    const message = 'Hello, Earth!';
    return this.message;
  }
};
console.log(object.getMessage());
```

- A) undefined
- B) Hello, Earth!
- C) Hello, World!
- D) {message:"Hello, World!}


5- "Aşağıdaki kod çıktısında console'a hiçbir değer basılmaz."
```javascript
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
```
  A) Doğru
- B) Yanlış

6- Aşağıdakilerden hangisi doğrudur?

```javascript

const bird = {
  size: 'small',
};

const mouse = {
  name: 'Mickey',
  small: true,
};
```
- A) mouse.bird.size is not valid
- B) mouse[bird.size] is not valid
- C) mouse[bird["size"]] is not valid
- D) All of them are valid


7- Aşağıdaki kodun çıktısı ne olur?
```javascript
function getAge() {
  'use strict';
  age = 21;
  console.log(age);
}

getAge();
```

- A) 21
- B) undefined
- C) ReferenceError
- D) TypeError

8- Aşağıdaki kodun çıktısı ne olur?
```javascript
const obj = { a: 'one', b: 'two', a: 'three' };
console.log(obj);
```
- A) { a: "one", b: "two" }
- B) { b: "two", a: "three" }
- C) { a: "three", b: "two" }
- D) SyntaxError

9- Aşağıdaki kodun çıktısı ne olur?
```javascript
for (let i = 1; i < 5; i++) {
  if (i === 3) continue;
  console.log(i);
}
```
- A) 1 2
- B) 1 2 3
- C) 1 2 4
- D) 1 3 4

10- Objelerdeki tanımlarken özelliklerin alfabetik sıraya göre olması gerekir.
- A) Doğru
- B) Yanlış

11- Objelerin alanlarına ulaşırken dot(nokta) notation(gösterim) ile birlikte expression kullanabiliriz.
- A) Doğru
- B) Yanlış

12- Obje tanımlarken objelerin özelliklerinin isimlendirilmesinde reserved keyword(özel tanımlı kelimeler) kullanılabilir.
- A) Doğru
- B) Yanlış

13- Aşağıdaki kodun çıktısı ne olur?
```javascript  
const human = {
  age: 28,
  name: 'Uğur',
  calcBirthYear : function() {
    return 2021 - age;
  }
};

console.log(human.calcBirthYear());
```

- A) 1993
- B) null
- C) undefined
- D) ReferenceError

14- Aşağıdaki kodun çıktısı ne olur?
```javascript   
const _human = {
  'yaş': 28,
  name: 'Uğur',
  calcBirthYear : function() {
    return 2021 - this['yaş'];
  }
};

console.log(_human.calcBirthYear());
```
- A) 1993
- B) null
- C) SyntaxError
- D) ReferenceError

15- Aşağıdaki kodun çıktısı ne olur?
 ```javascript
for (let i = 1; i < 5; i++) {
  if (i === 2) break;
  console.log(i);
}
```

- A) 1 
- B) 1 Nan 3 4
- C) 1 2
- D) 1 3 4

16- Aşağıdaki kodun çıktısı ne olur?
```javascript
for(let i = 0; i < 10; i = i+3) {
  console.log(i);
}
```
- A) 0 3 6 9
- B) 3 6 9
- C) 0 3 6 
- D) 0 3 6 9 NaN


17- Aşağıdaki kodun çıktısı ne olur?
```javascript
for(let i = 0; ; i++) {
  console.log(i);
}
```
- A) SyntaxError
- B) ReferenceError
- C) Infinite Loop
- D) 0 1 2 3 4 5 6 7 8 9 10

18- Prettier hangi işe yarar?

- A) Yazılan kodu renklendirir.
- B) Daha hızlı kod yazmak için kullanılır.
- C) Yazılan kodu okunurluğunu arttırmak için formatlama yapar.
- D) Javascript kodunu editörde çalıştırmaya yarar.

19- Aşağıdaki kodun çıktısı ne olur?
```javascript  
for (let i = 1; i < 5; i++) {
  console.log(i);
  if (i === 2) return i;
}
```
- A) 1 
- B) SyntaxError
- C) 1 2
- D) ReferenceError


20- Aşağıdaki kodun çıktısı ne olur?
```javascript
function calc() {
  for (let i = 1; i < 5; i++) {
    console.log(i);
    if (i === 2) return i;
  }
}

calc();
```
- A) 1 
- B) SyntaxError
- C) 1 2
- D) ReferenceError
