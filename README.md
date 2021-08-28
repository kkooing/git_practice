# Git 연습

## 깃(git) 최초 설정
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

## 커밋 다시쓰기
```
>git reset --hard <ID>  // WD 까지
           --mixed      // SA 까지 ┐
           --soft       // RP 까지 ┴─> 커밋로그를 덮어쓸때 사용
```

## 깃허브에 업로드
- 처음 업로드
```
git remote add origin "repo_url"
git branch -M main
git push -u origin main
```
- 업로드
```
git push
```

## 깃허브 다운로드
- 처음 다운로드
```
git clone "repo_url"
```
- 다운로드
```
git pull
```
:`git clone`이후에는 `git remote` 생략 가능