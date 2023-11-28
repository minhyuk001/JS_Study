# 반복문
* 반복문 역시 C, 자바와 매우 유사합니다
* for, while, forEach, for-in, for-of-for 등이 있습니다

## for
* 기본 구조는 시작, 종료조건, 증감식을 가지는 형태 입니다
* 다음 예제는 세개의 값을 가지는 배열을 선언하고 배열값을 모두 출력하는 예제 입니다

### for Ex
```javascript
const colors = ['red', 'blue', 'green'];
for (let i = 0; i < colors.length; i++) {
	console.log( colors[i] );
}
```

## while
* 조건이 성립하는 경우 계속 반복하는 구문입니다
* 무한 루프가 되지 않도록 코드 중간에 조건을 반드시 변경해 주어야 합니다

### while Ex
```javascript
const colors = ['red', 'blue', 'green'];
var i=0;
while (colors[i] != null) {
  console.log( colors[i] );
  i++;
}
```

## forEach
* ES5에서 사용가능하게 된 문법으로 배열의 모든 원소에 대해 특정 코드블럭을 수행할 수 있는 방법입니다

### forEach Ex
```javascript
const colors = ['red', 'blue', 'green'];
colors.forEach(function(value) {
  console.log(value);
});
```

## for-in, for-of
* 최근 다른 언어들에 도입된 -in 형태의 구문 입니다
* 다만 -in 의 경우 배열원소의 값에 접근할 수 없고 키 혹은 인덱스만 접근이 가능하므로 다른 언어에서의 -in과 같은 형태로 사용하려면 for-of를 사용해야 합니다

### for-in, for-of Ex
```javascript
const colors = ['red', 'blue', 'green'];
for (var index in colors) {
	console.log( colors[index] );
}

for (var value of colors) {
	console.log( value );
}
```

## for-in

* 객체의 모든 열거 가능한 속성에 대해 반복
* 즉, 배열 뿐만 아니라 일반적인 객체의 속성들을 모두 반복할 때도 사용 가능
* 모든 객체의 key(배열의 경우 인덱스)에 접근할 수 있지만 value에 접근할 수는 없음

## for-of
* 반복 가능한(Iterable)객체의 값을 순환. 배열 이외 문자열 데이터(유니코드 이모지 포함) 처리도 가능
* ES6에 새로 추가된 MAP, SET 에도 적용 가능
* Object를 대상으로 하지 않으며 객체의 속성을 순회하려면 for-in 을 사용
* Object를 사용할 경우 object.keys()로 키 값을 구해서 순회하면서 출력할 수 있음
