# git 명령어
---
**초기 설정**
```
- git init   
  init => initialize의 준말
  맨 처음 프로젝트를 올릴 때 사용

- git add .
  add: 어떤 파일을 올릴지 리스트로 확인
  .은 전부라는 뜻
  파일명으로 하나의 파일만 올릴 수도 있음

- git status
  git이 add한 파일을 체크해서 상태를 알려줌
  new: 새 파일
  modified: 수정된 파일

- git commit
  -m "history_name"
  히스토리를 만들어줌

- git remote add origin git@github.com:"repository_name"
  repository_name에 연결해줌

- git remote -v
  연결상태 확인

- git push origin branch_name
  branch 이름으로 푸쉬
```