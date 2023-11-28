# 변수 선언
* 변수수이름은 대소문자를 구별.
* 여러 변수를 한번에 선언할 수 있음.
* 지역변수와 전역변수가 있음.

```javascript
var firstNumber;
firstNumber = 10;
```
# var, let, const, string
* var는 지역변수 개념으로 함수 범위에서 유효함
* var를 선언하지 않으면 자동으로 전역변수가 됨
* let과 const 는 ES6 에서 등장한 block-scoped 변수 선언
* let은 값의 재할당이 가능하고 const 는 불가능
* const로 선언된 배열이나 객체의 경우 새로운 객체로 재할당하는 것은 안되고, 배열값의 변경/추가, 객체의 필드 변경등은 가능
* Stirng은 문자열을 표현할때 "",'' 둘다 사용 가능

# var Ex
```javascript
var foo = 'foo1';
console.log(foo); // foo1
 
if (true) {
  var foo = 'foo2';
  console.log(foo); // foo2
}

console.log(foo); // foo
```

# let, const Ex
```javascript
let foo = 'foo1';
const bar = 'bar1';
console.log(foo); // foo1
 
if (true) {
  let foo = 'foo2';
  console.log(foo); // foo2
  console.log(bar); // bar1
}
 
console.log(foo); // foo1
bar = 'bar2'; // error
```
# String 변수
```javascript
var string;
string = "Java Script"; // 혹은 'Java Script'
```
