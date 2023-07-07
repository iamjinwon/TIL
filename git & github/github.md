## Github

: Git으로 관리되는 프로젝트의 원격 저장소

## 명령어

```bash
git remote add origin (원격저장소 주소) #로컬의 Git 저장소에 원격 저장소로의 연결 추가

git branch -M main #기본 브랜치명을 main으로

git push -u origin main #로컬 저장소의 커밋 내역들 원격으로 push(업로드)

git remote #원격 목록 보기

git remote remove (원격 이름) #원격 지우기

git clone (원격 저장소 주소) #github에서 프로젝트 다운
-> 터미널이나 Git Bash에서 대상 폴더 이동 후 실행

git push #원격으로 커밋 밀어올리기

git pull #원격으로 커밋 당겨오기

git push --force #강제 push

git fetch #원격의 변경사항들을 확인

git push (원격 이름) --delete (원격의 브랜치명) #원격의 브랜치 삭제
```
