## JAVA script

- 객체 기반의 스크립트 프로그래밍 언어.
- Script태그를 이용해 HTML과 연결

---

### 이벤트

- 자바스크립트와 사용자 간의 상호연결

```js
//예시
onclick = "alert'('hi')";
onchange = "alert('changed')";
onkeydown = "alert('keydown')";
```

---

### 콘솔

- 콘솔을 통해 자바스크립트를 실행하면 웹페이지에서 자바스크립트가 실행된다.

---

### 자료형

- boolean
- null
- undefined
- number
- string
- symbol

---

### 기본 속성

```js
.length
//길이를 알려줌
.toupperCase
///대문자 만들어줌
.trim()
//공백 없애줌
.indexOf()
//()안의 열부터 시작
array.push()
//()안의 것을 배열에 추가
등등
```

---

### 변수와 연산자

- 형식 : var 변수명 = ' ';
- 변할수도 있는 값은 **let**으로, 변하지 않는 값은 **const**로 선언

```js
// 예시
 var = currentyear = 2021;
 var birthyear;
 var age;

 //산술연산자
 +, -, *, /, %, ++, --

 //할당연산자
 =, +=, -=, *=, /=, %=

 //비교연산자
 ==, ===, !=, !==, <, >, <=, >=

 //논리연산자
 OR연산자 : ||
 AND연산자 : &&
 NOT연산자 : !
```

---

### 함수

```js
// 예시
<script>
function addNumber(a,b) {
  var sum = a+b;
  alert(sum);;
}
</script>
```

---

### 배열과 객체

```js
// 예시
const dog ={
name : '멍멍이',
age : 2
}
​
const ironMan = {
name : '토니 스타크',
actor : '로버트 다우니 주니어',
alias : '아이언 맨'
}
​
const captainAmerica = {
name : '스티븐 로저스',
actor : '크리스 에반스',
alias : '캡틴 아메리카'
}
​
console.log(dog);
console.log(ironMan);
console.log(captainAmerica);
// 객체 만들기 예시

var numbers = ["one", "two", "threee", "four"] //배열 선언
```
