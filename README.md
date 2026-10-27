# ** 2026-10-27 TUE 오늘의 TIL : Git 명령어와 Git commint 하는 방법 + 내 GitHub에 push하는 방법 **
### **1. 명령어**

rm 은 파일 삭제

-rf  강제로 삭제

echo, >(리다이액션), cat(보기)

code . → vscode로 넘어감

vscode로 넘어가서 git 터미널로 만드는 방법

→ ctrl+`하면 터미널 오픈, ctrl + shift + p → Terminal: Select Default Profile 검색 → git bash로 변경

명령어 정리 → ctrl + l

줄임말에는 - 한개, 풀네임 시에 — 2개

git config —list 파일들 확인

git log 해왔던 상태 확인

git log —oneline 한 줄로 표현

git log —oneline —all 모든 commit한거 한 줄로 보여주기

브랜치 바꾸는 방법은 git branch -M 브렌치명

---

### 2.  Vs에서 Git 설정

이름 설정 —global(전체로 바꾸는거)—local

→ git config global user.email(name) 이메일, 이름 변경

git config —list하면 확인할 수 있음

---

### 3. Vs에서 Git commit 하는 방법

git add + 파일명

이때, 항상 git status를 활용해서 상태를 확인한다.

그 후, git commit -m(수정 사항 코멘트 옵션) “수정 사항”  하면 커밋까지 완료

만약, 전으로 돌아가고 싶다면, checkout 명령어를 사용하면 된다.

git log를 확인한 뒤에, 돌아가고 싶은 곳의 대쉬값을 가져와서,

git checkout 대쉬값 하면 돌아가고 싶은 곳으로 돌아간다.

다시 원상복구를 희망한다면, 원래의 대쉬값, 브런치명을 checkout 뒤에 써주면 돌아갈 수 있다.

---

### 4. Vs에서 원격으로 GitHub 리포에 올리는 방법

이제 github에 원격으로 올리는 방법을 알아보자

현재 리포와 연결이 되어있는지를 확인해보자

git remote -v  연결이 안되어있을 경우 아무것도 안뜸

그러면 연결해보자

git remote -v origin URL 이렇게 하면 연결이 됨.

다시 확인해보면 

fetch,push 가 나올텐데 여기서 fetch는 새로운 무언가가 있다는 뜻

push는 올리는 용도

이제 브렌치에 올려보자 

git push origin(별명) main(브렌치)

---
