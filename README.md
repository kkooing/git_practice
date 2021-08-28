# Git 연습

## git 도입
```
>git init
>git config user.name "sampleName"
>git config user.email "sample@sample.com"
```

## 커밋(commit)
```
>git add .
>git commit -m "내용"
```

## 기타

- `git log`
커밋 로그 보기
```
>git log
commit 커밋ID
Author: 이름 <이메일>
Date:   날짜

    내용
```
- `git diff <커밋ID1> <커밋ID2>`
두 커밋 비교: 커밋ID1 -> 커밋ID2로의 변경 사항
- `git reflog`
모든 커밋 로그 보기: git reset에 의한 로그 모두 보기
- `git status`
WD <-> SA 간 상태 표시

## 커밋 다시쓰기
```
>git reset --hard <ID>  // WD 까지
           --mixed      // SA 까지 ┐
           --soft       // RP 까지 ┴─> 커밋로그를 덮어쓸때 사용
```