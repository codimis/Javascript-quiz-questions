# CODIMIS 

## Javascript Eğitimi Onüçüncü Hafta Soruları

1 - "find() metodunun sonucunda bir dizi döner."

* A) Doğru
* B) Yanlış

2 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function getFruit(fruits) {
	console.log(fruits?.[1]?.[1])
}

getFruit([['pineapple', 'banana'], ['apple']])
getFruit()
getFruit([['pineapple'], ['apple', 'banana']])
```
* A) null, undefined, 'banana'
* B) [], null, 'banana'
* C) [], [], 'banana'
* D) undefined, undefined, 'banana'

3 - Aşağıdaki kodun çıktısı ne olur?
```javascript
function addToList(item, list) {
  return list.push(item);
}

const result = addToList('apple', ['banana']);
console.log(result);
```

* A) ['apple', 'banana']
* B) 2
* C) true
* D) undefined

4 - "findIndex() fonksiyonunda arattığımız eleman dizide yoksa method 0 return eder."

* A) Doğru
* B) Yanlış

5 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const groceries = ['banana', 'apple', 'peanuts'];

if (groceries.indexOf('banana')) {
  console.log('We have to buy bananas!');
} else {
  console.log(`We don't have to buy bananas!`);
}
```
* A) We have to buy bananas!
* B) We don't have to buy bananas
* C) undefined
* D) 16

6 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const numbers = [1, [2, 3, [4, 5]]];

console.log(numbers.flat(1));
```

* A) [1, [2, 3, [4, 5]]]
* B) [1, 2, 3, [4, 5]]
* C) [1, [2, 3, 4, 5]]
* D) [1, 2, 3, 4, 5]

7 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [2, 4, 6];
const result = arr.every(ele => ele * 2);
console.log(result);
```

* A) true
* B) [4,8,12]
* C) false
* D) [2,4,6]

8 - "sort() metodu orijinal array üzerinde değişiklik yapar."

* A) Doğru
* B) Yanlış

9 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr1 = ['a', 'b', 'c'];
const arr2 = ['b', 'c', 'a'];

console.log(
  arr1.sort() === arr1,
  arr2.sort() == arr2,
  arr1.sort() === arr2.sort()
);
```

* A) true true true
* B) true true false
* C) false false false
* D) true false true

10 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = new Array(3);
console.log(arr);
```

* A) undefined
* B) [3]
* C) [3 tane boş]
* D) Hiçbiri

11 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [1, 3, 5, 7];
console.log(arr.fill(6, 1, 3));
```

* A) [1, 6, 6, 7]
* B) [1, 6, 6, 6]
* C) [6, 1, 3, 7]
* D) [6, 1, 3, 6]

12 - Hangi satırdaki array tanımlamaları doğrudur?
```javascript
1- const arr = [2, 4, 6];
2- const arr = new Array(2, 4, 6);
3- const arr = Array(2, 4, 6);
```

* A) 1 ve 2
* B) 1
* C) 2 ve 3
* D) 1,2,3

13 - Aşağıdaki kodun çıktısı ne olur?
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

14 - Aşağıdaki kodun çıktısı ne olur?
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

15 - preventDefault() fonksiyonu ne yapar?

* A) Sayfayı sıfırlar
* B) Event'in temel özelliklerini varsayılana çevirir
* C) Event'in sahip olduğu varsayılan özelliklerinin ortaya çıkmasını engeller
* D) Sayfanın refresh olmasına engel olur

16 - input üzerindeki imleci kaldırmak için hangi fonksiyon kullanılır?

* A) blur
* B) focus
* C) cancel
* D) remove

17 - indexOf() fonksiyonu ile findIndex() fonksiyonu arasındaki fark nedir? 

* A) indexOf true ya da false döner
* B) tamamen aynıdır
* C) findIndex sadece obje alırken indexOf koşul alır
* D) findIndex koşul alırken indexOf obje ile çalışır

18 - flat() fonksiyonu iç içe olan arraylerdeki tüm elementleri tek seviyeye indirmeye yarar.

* A) Doğru
* B) Yanlış