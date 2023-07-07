## Git

- 프로젝트의 **시간**과 **차원**을 자유롭게 넘나들수 있도록 해줍니다.
- 여러 사람들이 프로젝트에서 협업할 수 있게 도움

## CLI vs GUI

- 터미널에 명령어를 이용하는 CLI 방식
- 소스트리 등의 프로그램을 사용하는 GUI 방식

## 1. Git 최초 설정

```bash
git config --global user.name ""(본인 이름)""
git config --global user.email ""(본인 이메일)""
git config --global init.defaultBranch main #기본 브랜치명 변경
```

## 2. 프로젝트 생성 & Git 관리 시작

```bash
git init #폴더에 숨김모드로 .git 폴더 생성
git status #git 현재상태 확인
```

## 3. Git에게 맡기지 않을 것들

a. 포함할 **필요가 없을** 때

- 자동으로 생성 또는 다운로드되는 파일들

b. 포함하지 **말아야 할** 때

- 보안상 민간함 정보를 담은 파일

```bash
<.gitignore 형식>

# 모든 file.c
file.c

# 최상위 폴더의 file.c
/file.c

# 모든 .c 확장자 파일
*.c

# .c 확장자지만 무시하지 않을 파일
!not_ignore_this.c

# logs란 이름의 파일 또는 폴더와 그 내용들
logs

# logs란 이름의 폴더와 그 내용들
logs/

# logs 폴더 바로 안의 debug.log와 .c 파일들
logs/debug.log
logs/*.c

# logs 폴더 바로 안, 또는 그 안의 다른 폴더(들) 안의 debug.log
logs/**/debug.log
```

## 4. Git 버전관리하기

```bash
git status #변경사항 확인

git add "파일명" #파일 하나 담기

git add . #모든 파일 담기

git commit #Vi 입력 모드 진입

git commit -m "커밋 이름" #커밋 메시지 함께 작성

git commit -am "커밋 이름" #새로 추가된(untracked)파일이 없을 때 add와 commit을 한꺼번에

git log #커밋한 기록 확인(:q로 빠져나감)
```

## 5. 과거로 돌아가기

- reset : 원하는 시점으로 돌아간 뒤 이후 내역들을 지웁니다.
- revert : 되돌리기 원하는 시점의 커밋을 거꾸로 실행합니다.

```bash
git reset --hard (돌아갈 커밋 해시) #과거의 커밋으로 돌아간 뒤 이후 내역은 삭제

git reset --hard #현 커밋 상태로 초기화

git revert (되돌릴 커밋 해시)

git rm 파일명 #Git에서 해당 파일 삭제

git revert --continue #충돌 이후 마무리

git revert --no--commit (되돌릴 커밋해시) #커밋해버리지 않고 revert하기
```
