# CODIMIS 
## Javascript Eğitimi Onbirinci Hafta Soruları

1- Aşağıdaki kodun çıktısı ne olur?
```javascript
let arr = ['a', 'b', 'c', 'd', 'e'];
let arr2 = arr.slice(2);
arr.push('f');
console.log(arr2);
```
* A) ["c","d","e"]
* B) ["c","d","e","f"]
* C) ["d","e","f"]
* D) ["f"]

2- Aşağıdaki kodun çıktısı ne olur?
```javascript
let arr = [['a', 'b', 'c', 'd', 'e']];
let arr2 = arr.slice(0);
arr2[0].push('f');
console.log(arr);
```

* A) [["a","b","c","d","e","f"]] 
* B) [["a","b","c","d","e"]]
* C) ["a","b","c","d","e","f"]
* D) ["a","b","c","d","e"]

3- "Slice ve splice metodları orijinal array üzerinde değişiklik yapmaz." 
* A) Doğru
* B) Yanlış

4- "Join metodu birden fazla arrayi birleştirmek için kullanılır."
* A) Doğru
* B) Yanlış

5- Aşağıdaki kodun çıktısı ne olur?
```javascript
let arr = ['a', 'b', 'c', 'd', 'e'];
let arr2 = arr.slice(2, 1);
console.log(arr2);
```
* A) []
* B) ["c","d","e","a","b"]
* C) ["c"]
* D) ["c","d","e","a"]

6- Aşağıdaki kodun çıktısı ne olur?
```javascript
const num1 = [[1]];
const num2 = [2, [3]];
const numbers = [...num1, ...num2];

num1[0].push(4);

console.log(numbers);
```
* A) [[1], 2, [3]]
* B) [[1, 4], 2, [3]]
* C) [[1], 2, [3, 4]]
* D) [4, [1], 2, [3]]

7- forEach metodunda callback functionda index gibi parametrelerin sırası önemlidir. 
* A) Doğru
* B) Yanlış

8- Aşağıdaki kodun çıktısı ne olur?
```javascript
const num1 = [1, 2, 3, 4, 5, 6];

num1.forEach(function(i) {
  console.log(i);
  if (i === 2) {
    break;
  }
})
```
* A) 1 2 3 4 5 6
* B) 1 2
* C) 1
* D) SyntaxError

9- Aşağıdaki kodun çıktısı ne olur?
```javascript
let count = 0;
const nums = [0, 1, 2, 3];

nums.forEach(num => {
    if (num) count += 1;
})

console.log(count);
```
* A) 1
* B) 2
* C) 3
* D) 4

10- Aşağıdaki kodun çıktısı ne olur?
```javascript
const fruit = ['banana', 'orange', 'apple'];

fruit.slice(0, 1);
fruit.splice(0, 1);
fruit.unshift('raspberry');

console.log(fruit);
```
* A) ['banana','orange', 'apple']
* B) ['orange', 'apple']
* C) ['raspberry', 'orange', 'apple']
* D) ['raspberry', 'banana', 'orange', 'apple']

11- Hangi satır(lar)daki işlemler hata verecektir?
```javascript
const emojis = ['🎄', '🎅🏼', '🎁', '⭐'];

/* 1 */ emojis.push('🦌');
/* 2 */ emojis.splice(0, 2);
/* 3 */ emojis = [...emojis, '🥂'];
/* 4 */ emojis.length = 0;
```

* A) 1
* B) 1 ve 2
* C) 3 ve 4
* D) 3

12- Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [1,2,3,4,5];
const slicedArr = arr.slice(1,2);

arr.splice(1,2,...slicedArr);
console.log(arr);
```

* A) [1,2]
* B) [1,4,5,2]
* C) [1,2,4,5]
* D) [1,3,4,5,2]

13- "Map ile foreach kullanıldığında key ve value parametreleri hep aynı değeri alır."

* A) Doğru
* B) Yanlış

14- Aşağıdaki kodun çıktısı ne olur?
```javascript
const arraySparse = [1,3, ,7];

arraySparse.forEach(function(element) {
  console.log(element)
});
```

* A) 1,3,7
* B) 1,3,undefined,7