## Cmd에서 경로지정

```bash
cd \ #C드라이브로 경로변경

mkdir workspace #workspace라는 폴더(디렉토리) 생성

cd workspace #workspace로 경로 지정

mkdir git_test #git_test라는 폴더 생성

cd git_test #git_test로 경로 지정
```

---

## Git 프로젝트 시작

```bash
git init

git add git_test.txt

git commit git_test.txt -m "First commit"

mv .gitignore.txt .gitignore -> .gitignore 파일형식변경

git rm test_abc.txt

git mv git_test.txt test.txt -> 파일이름변경
```

---

## Git log 명령어들

```bash
git log --stat #통계 정보를 조회 가능

git log --pretty=oneline #한줄에 이쁘게 정보를 출력

git log --pretty=format:"%h - %an, %at :%s " #날짜 정보 출력

git log --pretty=format:"%h - %an, %at :%s " --graph

git checkout bfc1425(예시) #돌아가기
```

---

## Git

1. 형상 관리 도구
2. 코드 공유 도구

- 코드 공유를 위해서는 Remote Repository가 필요

- Working Directory
  안의 Local Repository
  <-> Remote Repository

---

## 코드릍 통해서 push하는 방법

```bash
echo "# CS50_Web_test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/iamjinwon/CS50_Web_test.git
git push -u origin main
```

---

## Git 원격저장소 관리

```bash
git remote

git remote -v

git remote add origin 주소

git remote add test 주소

git remote rm test
```

---

## Git remote 저장소에 commit 올리기

```bash
git add 파일명

git commit 파일명 -m"커밋명"

git push origin main
```

---

## remote -> Local 가져오기

1. Clone - 전체를 다 가져오는 명령
2. Pull - 가져와서 같은 Branch를 합쳐 버리는 명령어
3. Fetch - 변경 내용만 가져오고 안 합치는 명령어

## Fork & Pull Request (PR)

- Fork - 남의 Githhub Repository를 내 걸로 가져오는 거

- PR - Fork로 가져온 남의 코드를 수정한 다음 가져가 달라고 요청하는것

- Fork -> Clone -> Add -> Commit -> Push -> PR

- Permission Setting
  : 아예 작업 권한을 공동 작업자에게 넘기는 방식
