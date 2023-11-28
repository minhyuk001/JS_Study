## 조건문
* C, 자바와 매우 유사합니다
* if, else, switch등이 있습니다

## if, else if
* 특정 조건이 참인 경우 수행되는 코드 블럭을 정의 합니다.
* else 와 결합해 조건 범위나 조건을 세분화하는 것이 가능하며 AND, OR 연산을 함께 사용할 수 있습니다.
### if, else if Ex
```javascript
var score = 85;

if (score >= 90)
	console.log('A');
else if (score >= 80)
	console.log('B');
else if (score >= 70)
	console.log('C');
else
	console.log('F');
```

## switch
* 입력값에 따라 처리를 다르게 하는 경우 사용합니다
* 내용적으로는 if ~ else if 와 유사합니다

### switch Ex
```javascript
var level = 'B';

switch(level) {
  case 'A' :
    console.log('Admin');break;
  case 'B' :
    console.log('User');break;
  default :
    console.log('Not');break;
}
```
