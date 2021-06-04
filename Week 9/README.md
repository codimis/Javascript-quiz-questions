1- Aşağıdaki kodun çıktısı ne olur?
```javascript
const [a=1, , b, [c,d] ,f] = [undefined,5,6,[3,4]]
console.log(a,b,c,d,f);
```
* A) undefined 5 6 3 4
* B) 1 6 3 4 undefined
* C) ReferenceError
* D) 1 1 6 3 4 undefined

2- Aşağıdaki kodun çıktısı ne olur?
```javascript
const obj = {food: 'Soup', drink: 'Water'};

{food,drink} = obj;

console.log(food);
console.log(drink);
```
* A) Soup Water 
* B) Pizza Cola
* C) SyntaxError
* D) Water Soup

3- Aşağıdaki kodun çıktısı ne olur?
```javascript
const listA = [1, 2, 3];
const listB = [...listA];
listB.push(4);
console.log('listA:', listA);
console.log('listB:', listB);
```
* A) [1,2,3] - [1,2,3,4]
* B) [1,2,3,4] - [1,2,3]
* C) ReferenceError - [1,2,3]
* D) [1,2,3,4] - [1,2,3,4]

4- Aşağıdaki kodun çıktısı ne olur?
```javascript
const one = NaN || {} || null;
const two = null || false || '';
const three = [] || 0 || true;

console.log(one, two, three);
```
* A) false null []
* B) null "" true
* C) {} "" []
* D) null null true

5- Aşağıdaki kodun çıktısı ne olur?
```javascript
const person = {
  name: 'Caner',
  age: 27,
};

for (const [x, y] of Object.entries(person)) {
  console.log(x, y);
}
```
* A) name Caner ve age 27
* B) ["name", "Caner"] ve ["age", 27]
* C) ["name", "age"] ve undefined
* D) Error


6- Aşağıdaki kodun çıktısı ne olur?
```javascript
const set = new Set();

set.add(1);
set.add('Caner');
set.add({ name: 'Caner' });

for (let item of set) {
  console.log(item + 2);
}
```
* A) 3, NaN, NaN
* B) 3, 7, NaN
* C) 3, Caner2, [object Object]2
* D) "12", Caner2, [object Object]2


7- Aşağıdaki kodun çıktısı ne olur?
```javascript
const numbersSet = new Set([1,1,2,2,3,4,5,6,6,7]);

console.log(numbersSet.has('1'));
console.log(numbersSet.has(1));
```
* A) true true
* B) false true
* C) false false
* D) true false

8- Hangi seçenekteki gibi fonksiyon çağrılırsa 6 sayısını return eder?
```javascript
function sumValues(x, y, z) {
  return x + y + z;
}
```
* A) sumValues([...1, 2, 3])
* B) sumValues([...[1, 2, 3]])
* C) sumValues(...[1, 2, 3])
* D) sumValues([1, 2, 3])

9- Hangi satırlar 'Hello world!' yazısını print eder?
```javascript
const myMap = new Map();
const myFunc = () => 'greeting';

myMap.set(myFunc, 'Hello world!');

//1
console.log(myMap.get('greeting'));
//2
console.log(myMap.get(myFunc));
//3
console.log(myMap.get(() => 'greeting'));
```
* A) 1
* B) 2
* C) 2 ve 3
* D) Hepsi

10- Aşağıdaki kodun çıktısı ne olur?
```javascript
  const hero = {
  name: 'Batman',
  realName: 'Bruce Wayne'
};
const prop = 'name';
const { [prop]: name } = hero;
console.log(name);
```
* A) undefined
* B) Batman
* C) SyntaxError
* D) ReferenceError

11- Aşağıdaki kodun çıktısı ne olur?
```javascript 
const hero = {
  name: 'Batman',
  realName: 'Bruce Wayne',
};

const { name, ...realHero } = hero;

console.log(typeof name);
console.log(typeof realHero); 
```
* A) string, string
* B) string, object
* C) object, object

12- Aşağıdaki kodun çıktısı ne olur?
```javascript
const nested = [2, 3, 9, [5, 6]];

const [, i, , j] = nested;
[j, i] = [i, j];

console.log(j, i);
```
* A) [5] , 3
* B) [5,6] , 3
* C) TypeError
* D) SyntaxError

13- Aşağıdaki kodun çıktısı ne olur?
```javascript
const name = 'Caner Ünal';
console.log(name.padStart(13));
console.log(name.padStart(2));
```
* A) "Caner Ünal", "Caner Ünal"
* B) "[13 tane boşluk]Caner Ünal", "[2 tane boşluk]Caner Ünal"
* C) "[3 tane boşluk]Caner Ünal", "Caner Ünal"
* D) "Caner Ünal", "Can"

14- Aşağıdaki kodun çıktısı ne olur?
```javascript
const rest = new Map();
rest
  .set('name', 'Turkish Restaurant')
  .set(1, 'Iskender')
  .set('2', 'Kebap')
  .set(3, 'Baklava');

console.log(rest.get(1), rest.get(2), rest.get(3));
```
* A) Iskender, Kebap, Baklava
* B) Undefined, Undefined, Undefined
* C) Iskender, Undefined, Baklava