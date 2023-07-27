# git 협업

<h3>gitFlow</h3>

1. main
```
안전할 때만
```
2. develop
```
main 복사본 : 새로운 기능 추가 시 사용
feature에서 merge된 것을 main으로 push 할수도 있지만 안전한건 release이용..
```
3. feature
```
새로운 기능 개발 후 잘 되면 merge
```
4. release
```
v 1.0 출시 전 여러가지 테스트
완성되면 main에 합침
develop에도 합침
```
5. hotfix
```
버그수정
1.0.1 등으로 표기
수정 후 main, develop merge
```

<h3>Trunk-based</h3>

```
브랜치 하나만 잘 관리하자
develop 브랜치 이런게 왜 필요하냐
```

- 테스트 자주 필요
- 한 곳에 정리되어 깔끔
- 안정화된 프로그램에서 주로 사용
