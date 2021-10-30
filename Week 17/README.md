# CODIMIS 

## Javascript Eğitimi Onyedinci Hafta Soruları

1 - Aşağıdakilerden hangisi HTTP requestlerinden biri değildir?

* A) GET
* B) POST
* C) PUT
* D) OPEN

2 - XmlHttpRequest ile aşağıdaki Web Api'den veri alırken 3.adımda hangi kod yer almalıdır?
```javascript
//1.adım
const request = new XMLHttpRequest();
//2.adım
request.open('GET',`https://restcountries.com/v2/name/${country}`);
//3.adım

//4.adım
 request.addEventListener('load',function(){
     const [data] = JSON.parse(this.responseText);
     console.log(data);
 });
```

* A) request.get();
* B) request.post();
* C) request.send();
* D) request.retrieve();

3 - Hangisi Promise'ın statelerinden biri değildir?

* A) Rejected
* B) Fulfilled
* C) Pending
* D) Delayed

4 - "Promise.finally() metodu hata alındığında çalışır"

* A) Doğru
* B) Yanlış

5 - "setTimeout() metodu synchronous çalışır"

* A) Doğru
* B) Yanlış

6 - cook() metodu çalışırken bir hata olursa

```javascript
Pasta()
.then(cook)
.then(eat)
.catch(complain)
```

* A) eat() ve complain() metodu çalışır
* B) complain() metodu çalışır
* C) hiçbir metod çalışmaz

7 - Aşağıdaki kodda konsola hangi çıktı basılır?
```javascript
fetch('https://www.website.com/api/user/1')
  .then(res => res.json())
  .then(res => console.log(res));
```

* A) Fetch metodunun sonucu
* B) Fetch metodunun ikinci kez çağrılmasının sonucu
* C) İlk then() metodunun sonucundan dönen değer
* D) undefined

8 - "JavaScript birden fazla thread (multiple thread) çalıştırabileceğiniz bir dildir."

* A) Doğru
* B) Yanlış

9 - Aşağıdaki kodun çıktısının sırası nasıl olur?

```javascript
setTimeout(() => console.log(1), 0);
Promise.resolve(2).then(result => console.log(result));
console.log(3);
```

* A) 1 2 3
* B) 2 1 3
* C) 3 2 1
* D) 3 1 2
  
10 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const myPromise = () => Promise.resolve('I have resolved!');

function firstFunction() {
  myPromise().then(res => console.log(res));
  console.log('second');
}

async function secondFunction() {
  console.log(await myPromise());
  console.log('second');
}

firstFunction();
secondFunction();
```

* A) I have resolved!, second ve I have resolved!, second
* B) second, I have resolved! ve second, I have resolved!
* C) I have resolved!, second ve second, I have resolved!
* D) second, I have resolved! ve I have resolved!, second

11 - Aşağıdaki kodun çıktısı ne olur?

```javascript
const myPromise = Promise.resolve('Some cool data');

const tryCatchExpFunction = async function() {
  try {
    console.log(await myPromise);
  } catch {
    throw new Error(`Error`);
  } finally {
    console.log('Finally');
  }
}
tryCatchExpFunction();
```

* A) Some cool data
* B) Finally
* C) Some cool data - Finally
* D) Error - Finally

12 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const promise1 = Promise.resolve('First')
const promise2 = Promise.reject('Second')

const runPromises = async () => {
	const res = await Promise.all([promise1, promise2])
	return res;
}

runPromises()
	.then(res => console.log(res))
	.catch(err => console.log(err))
```

* A) ["First","Second"]
* B) "First"
* C) "Second"
* D) undefined

13 - Aşağıdaki kodun çıktısı ne olur?

```javascript
async function getData() {
  return await Promise.resolve('I made it!');
}

const data = getData();
console.log(data);
```

* A) "I made it!"
* B) Promise {<resolved>: "I made it!"}
* C) Promise {<pending>}
* D) undefined

14 - Aşağıdaki kodun çıktısı ne olur?
```javascript
const firstPromise = new Promise((res, rej) => {
  setTimeout(res, 500, 'one');
});

const secondPromise = new Promise((res, rej) => {
  setTimeout(res, 100, 'two');
});

Promise.race([firstPromise, secondPromise]).then(res => console.log(res));
```

* A) "one"
* B) "two"
* C) "two" "one"
* D) "one" "two"