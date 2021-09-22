# CODIMIS 

## Javascript Eğitimi Onikinci Hafta Soruları

1 - Aşağıdaki kodun çıktısı ne olur?
```javascript
let name = 'Caner';

function getName() {
  console.log(name);
  let name = 'Uğur';
}

getName();
```
* A) Caner
* B) Uğur
* C) undefined
* D) ReferenceError

2 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function checkAge(age) {
  if (age < 18) {
    const message = "Sorry, you're too young.";
  } else {
    const message = "Yay! You're old enough!";
  }

  return message;
}

console.log(checkAge(21));
```

* A) "Sorry, you're too young."
* B) "Yay! You're old enough!"
* C) ReferenceError
* D) undefined

3 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const person = {
  name: 'Caner Unal',
  hobbies: ['coding'],
};

function addHobby(hobby, hobbies = person.hobbies) {
  hobbies.push(hobby);
  return hobbies;
}

addHobby('running', []);
addHobby('dancing');
addHobby('baking', person.hobbies);

console.log(person.hobbies);
```

* A) ["coding"]
* B) ["coding","dancing"]
* C) ["coding","dancing","baking"]
* D) ["coding","running","dancing","baking"]

4 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const user = {
	email: "my@email.com",
	updateEmail: email => {
		this.email = email
	}
}

user.updateEmail("new@email.com")
console.log(user.email)
```
* A) my@email.com
* B) new@email.com
* C) undefined
* D) ReferenceError

5 - Aşağıdaki kodun çıktısı ne olur?
```javascript
let randomValue = { name: "Caner" }
randomValue = 23

if (!typeof randomValue === "string") {
	console.log("It's not a string!")
} else {
	console.log("Yay it's a string!")
}
```
* A) It's not a string!
* B) Yay it's a string!
* C) TypeError
* D) undefined

6 - Hangi methodlar emojis arrayinde değişiklik yapacaktır?
```javascript
const emojis = ['✨', '🥑', '😍'];

emojis.map(x => x + '✨');
emojis.filter(x => x !== '🥑');
emojis.reduce((acc, cur) => acc + '✨');
emojis.slice(1, 2, '✨');
emojis.splice(1, 2, '✨');
```
* A) Hepsi
* B) map reduce slice splice
* C) map slice splice
* D) splice

7 - Aşağıdaki kodun çıktısı ne olur?
```javascript
[1, 2, 3].map(num => {
  if (typeof num === 'number') return;
  return num * 2;
});
```

* A) []
* B) [null, null, null]
* C) [undefined, undefined, undefined]
* D) [ 3 tane boş ]

8 - Aşağıdaki kodun çıktısı ne olur?
```javascript
let namesArray = ["ugur", 0, "caner", null, "codimis", false];
let filteredArray = namesArray.filter(Boolean);
console.log(filteredArray);
```

* A)["ugur",0,"caner",null,"codimis",false]
* B)["ugur","caner","codimis]

9 - Aşağıdaki kodun çıktısı ne olur?
```javascript
[[0, 1], [2, 3]].reduce(
  (acc, cur) => {
    return acc.concat(cur);
  },
  [1, 2],
);
```
* A) [0, 1, 2, 3, 1, 2]
* B) [6, 1, 2]
* C) [1, 2, 0, 1, 2, 3]
* D) [1, 2, 6]

10 - Aşağıdaki kodun çıktısı ne olur?
```javascript
[1, 2, 3, 4].reduce((x, y) => console.log(x, y));
```

* A) 1 2 - 3 3 - 6 4
* B) 1 2 - 2 3 - 3 4
* C) 1 undefined - 2 undefined - 3 undefined - 4 undefined
* D) 1 2 - undefined 3 - undefined 4

11 - "Map() ve ForEach() methodları side effect yaratır."

* A) Doğru
* B) Yanlış

12 -  Aşağıdaki kodun çıktısı ne olur?
```javascript
const input = [ 5, -4, 10, 0, -3, 20, -15];

input.filter(num => return num > 0)
  .reduce((accumulator, currentValue) => accumulator + currentValue, 0);
```

* A) 35
* B) SyntaxError
* C) 13

13 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const array = [-5, -1, -2, -3, -4];

const min = array.reduce((acc , curr) => {
if(acc>curr) return  acc; 
else return curr 
}, 0);

console.log(min);
```

* A) -5
* B) -1
* C) 0
* D) SyntaxError

14 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const myArr = ['a', 'b', 'c'];
const myMap = { a: 1, b: 2, c: 3 };

const result = myArr.map(letter => myMap[letter]);
console.log(result);
```

* A) 1, 2, 3
* B) a, b, c
* C) [1, 2, 3] 
* D) [a, b, c]

15 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [
  x => x * 1,
  x => x * 2,
  x => x * 3,
  x => x * 4
];
console.log(arr.reduce((agg, el) => agg + el(agg), 1));
```

* A) 1
* B) 60
* C) 100
* D) 120