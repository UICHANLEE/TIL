# Node.js

---
- 설치
  npm install -g @vue/cli

- 프로젝트 생성
  vue create 프로젝트명

- 구조
```node
<template>HTML</template>
<script>JS</script>
<style>CSS</style>
```

- 미리보기
  npm run serve   
- 폴더
  node_modules: 프로젝트에 쓰는 라이브러리들
  src: 소스파일 다 담는 곳
  public: html파일, 기타파일 보관
  package.json: 라이브러리 버전, 프로젝트 설정기록

{{데이터바인딩}}
- JS데이터를 HTML에 옮겨 넣을때
- 값 변경 용이
- Vue의 실시간 렌더링
- HTML 속성도 데이터 바인딩 가능
  ```
  :속성 "데이터이름"
  ```

- Vue의 HTML 반복문
```
<a v-for="작명 in 반복횟수" :key="작명">{{ 작명 }}</a>>
*반복횟수 대신 array나 object 집어넣기 가능 (데이터의 갯수만큼 반복, 작명은 데이터 안의 자료)
- :key 의 용도 = 반복문 돌린 요소를 컴퓨터가 구분하기 위해 사용
- 작명은 2개까지 가능
```

- 이벤트 핸들러
```
버튼을 눌렀을때 JavaScript실행
전통: onclick=""
Vue방식: @click=""
 ```

-Vue에서 함수 만들기
```
methods: { 함수(){} }
- 함수 안에서 데이터를 사용할 때는 this.데이터명
```
