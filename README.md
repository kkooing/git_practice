# Git 연습

## 기초

### 깃(git) 최초 설정
```
git init
git config user.name "sampleName"
git config user.email "sample@sample.com"
```

### 커밋(commit)
```
git add .
git commit -m "내용"
```

### 커밋 로그 관련

- `git log` 커밋 로그 보기
```
>git log
commit 커밋ID
Author: 이름 <이메일>
Date:   날짜

    내용
```
- `git diff <커밋ID1> <커밋ID2>` 두 커밋 비교: 커밋ID1 -> 커밋ID2로의 변경 사항
- `git reflog` 모든 커밋 로그 보기: git reset에 의한 로그 모두 보기
- `git status` WD <-> SA 간 상태 표시

### 커밋 다시쓰기(커밋 이동)
```
git reset --hard <ID>   // WD 까지
          --mixed       // SA 까지 ┐
          --soft        // RP 까지 ┴─> 커밋로그를 덮어쓸때 사용
```

### 깃허브에 push/pull
처음 설정
```
git remote add origin "repo_url"    // 대상 repo 설정
git branch -M main                  // 브랜치 만들기
git push -u origin main             // 브랜치로 push
```
:이후 `git push`, `git pull` 만으로 push/pull 가능


### 제 2 유저
repo 다운로드
```
git clone "repo_url"
```
`git init`, `git remote`, `git branch` 등 생략가능

## 브랜치
- `git branch <branch>` 브랜치 생성
- `git checkout <branch>` 브랜치 이동
- `git log --all --graph` 모든 브랜지 커밋 로그 표시 (+그래프)
- `git merge <branch>` (상위 브랜치에서 실행)  
Fast-forward: 충돌 없음, 커밋 이동  
conflict    : 충돌 발생, 수정 후 커밋 필요

##