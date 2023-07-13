# JavaScript

### 변수선언

```javascript
const = 변하지 않는 값
let = 변할 수 있는 값
```
- 변수는 문자와 숫자, $와 _만 사용
  > const MY_HOME = "***";
  let _ = 1;
  let $ = 3;
- 첫글자는 숫자가 될 수 없음
  > let 1stGrade = "A+"; 와 같이 선언 불가
- 예약어는 사용불가
  > let let = 99;
- 상수는 대문자로
  > let MAX_SIZE = 99;
- 변수명은 읽기 쉽고 이해할 수 있게
  > let a = 1; 보다는 let userNumber = 3;

### 자료형

- typeof: 타입확인   


### alert | prompt | confirm

- alert: 팝업창
- prompt: 입력창
- confirm: 확인받음

```JS
const name = prompt("이름을 입력하세요");
alert(`안녕하세요, ${name}님, 환영합니다.`);
```

```javascript
const name = prompt("예약일을 입력해주세요.", "2023-07-");

const isAdult = confirm("당신은 성인입니까?");
console.log(isAdult)
```



