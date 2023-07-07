## Branch

: 분기된 가지(다른 차원)

- 프로젝트를 하나 이상의 모습으로 관리

  ex) 실배포용, 테스트서버용...

- 여러 작업들이 각각 독립되어 진행

  ex) 신기능1, 신기능2, 코드개선 ...

---

## 기본 명령어

```bash
git branch 브랜치명 #브랜치 생성

git branch # 브랜치 확인

git switch 브랜치명 #해당 브랜치로 이동

git switch -c 브랜치명 #브랜치 생성과 동시에 이동

git branch -d 브랜치명 #브랜치 삭제

git branch -D 브랜치명 #강제 삭제

git log --all --decorate --oneline --graph #여러브랜치의 내역 편리하게 보기
```

## Branch를 합치는 두가지 방법

- merge : 두 브랜치를 한 커밋에 이어붙임
- rebase : 브랜치를 다른 브랜치에 이어붙임

<img src="https://1drv.ms/i/s!AowQ-jL0dAJCgZVoDgqILfm_trzHhQ?e=CBKx0T">

## 합치기 명령어

```bash
git merge 브랜치명 #'main' 이동 후 실행
- 'merge'는 'reset'으로 되돌리기 가능

git rebase main #'브랜치명' 이동 후 실행, merge와 반대
- main 이동 후 'git merge 브랜치명' 을 통해서 '브랜치명'의 시점으로 fast-forward
```

## 충돌해결 명령어

```bash
1. merge 충돌
git merge --abort #merge 중단

2. rebase 충돌
git rebase --abort #rebase 중단

git rebase --continue #해결 가능할 시 충돌부분 수정 후 git add . 한 다음 위 명령어로 계속
```
