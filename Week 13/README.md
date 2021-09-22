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
const numbers = [1, [2, 3, [4, 5]]];

console.log(numbers.flat(1));
```

* A) [1, [2, 3, [4, 5]]]
* B) [1, 2, 3, [4, 5]]
* C) [1, [2, 3, 4, 5]]
* D) [1, 2, 3, 4, 5]

6 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [2, 4, 6];
const result = arr.every(ele => ele * 2);
console.log(result);
```

* A) true
* B) [4,8,12]
* C) false
* D) [2,4,6]

7 - "sort() metodu orijinal array üzerinde değişiklik yapar."

* A) Doğru
* B) Yanlış

8 - Aşağıdaki kodun çıktısı ne olur?
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

9 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = new Array(3);
console.log(arr);
```

* A) undefined
* B) [3]
* C) [3 tane boş]
* D) Hiçbiri

10 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const arr = [1, 3, 5, 7];
console.log(arr.fill(6, 1, 3));
```

* A) [1, 6, 6, 7]
* B) [1, 6, 6, 6]
* C) [6, 1, 3, 7]
* D) [6, 1, 3, 6]

11 - Hangi satırdaki array tanımlamaları doğrudur?
```javascript
1- const arr = [2, 4, 6];
2- const arr = new Array(2, 4, 6);
3- const arr = Array(2, 4, 6);
```

* A) 1 ve 2
* B) 1
* C) 2 ve 3
* D) 1,2,3

12 - indexOf() fonksiyonu ile findIndex() fonksiyonu arasındaki fark nedir? 

* A) indexOf true ya da false döner
* B) tamamen aynıdır
* C) findIndex sadece obje alırken indexOf koşul alır
* D) findIndex koşul alırken indexOf obje ile çalışır

13 - flat() fonksiyonu iç içe olan arraylerdeki tüm elementleri tek seviyeye indirmeye yarar.

* A) Doğru
* B) Yanlış