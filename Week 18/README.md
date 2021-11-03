# CODIMIS 

## Javascript Eğitimi Onsekizinci Hafta Soruları

1 - Aşağıdaki kodun çıktısı ne olur?
```javascript
// index.js
console.log('running index.js');
import { sum } from './sum.js';
console.log(sum(1, 2));

// sum.js
console.log('running sum.js');
export const sum = (a, b) => a + b;
```

* A) running index.js, running sum.js, 3
* B) running sum.js, running index.js, 3
* C) running sum.js, 3, running index.js
* D) running index.js, undefined, running sum.js

2 - Named export ları kullanarak aşağıdaki değişkenleri nasıl export ederiz?
```javascript
let elephant = {...};
let sheep = {...};
let animalCount = 2;
let revenue = 320;
```

* A) export default elephant, sheep, animalCount, revenue;
* B) export { elephant, sheep, animalCount, revenue };
* C) export default { elephant, sheep, animalCount, revenue };
* D) export default Animals;

3 - Hangi seçenekte hem named export hem de default export, import edilmiştir?

* A) import {cake, gifts, dinner, dj} from './celebration.js';
     import venue from './celebration.js';
* B) import {celebration} from './celebration.js';
* C) import {cake, gifts, dinner, dj} from './celebration.js';
* D) import {all} from './celebration.js';

4 - Bir NPM paketini global olarak yüklemek için hangi komut kullanılır ? 

* A) npm run start
* B) npm install <package-name>
* C) npm install -g <package-name>
* D) npm i <package-name>

5 - Aşağıdaki araçlardan hangisi module bundler olarak kullanılır?

* A) Node.js
* B) Parcel
* C) Babel
* D) NPM

6 - npm init komutunu çalıştırdığımızda projemizde hangi dosya oluşur?

* A) config.json
* B) .prettierrc
* C) .babelrc
* D) package.json

7 - Aşağıdaki kod parçası ___________ programming in kullanıldığı bir örnektir."

```javascript
const longPasswords = passwords.filter(password => password.length >= 9);
```
* A) Declarative
* B) Object Oriented
* C) Imperative
* D) ES6

8 - Terminalde komut yazarken hangi tuşa bastığımızda komut otomatik tamamlanır?

* A) space
* B) shift
* C) enter
* D) tab

9 - JavaScript'te değişken tanımlarken var keyword ü ile tanım yapmamaya dikkat etmeliyiz."

* A) Doğru
* B) Yanlış

10 - Dersteki örnekte aşağıdaki kod parçası ile devreye aldığımız, modüllerin sayfayı yenilemeden güncellenmesi özelliğinin adı nedir?

```javascript
if (module.hot) {
  module.hot.accept();
}
```

* A) Polyfilling
* B) Named Export
* C) Transpiling
* D) Hot Module Replacement

11 - Parcel'i başlattığımız komut aşağıdakilerden hangisidir?

* A) npm start index.html
* B) npx parcel index.html
* C) npm run start
* D) npm run parcel