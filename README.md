# Git 연습

## 깃(git) 최초 설정
```
git init
git config user.name "sampleName"
git config user.email "sample@sample.com"
```

## 커밋(commit)
```
git add .
git commit -m "내용"
```

## 커밋 로그 관련

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

## 커밋 다시쓰기(커밋 이동)
```
git reset --hard <ID>   // WD 까지
          --mixed       // SA 까지 ┐
          --soft        // RP 까지 ┴─> 커밋로그를 덮어쓸때 사용
```

## 깃허브에 push/pull
처음 설정
```
git remote add origin "repo_url"    // 대상 repo 설정
git branch -M main                  // 브랜치 만들기
git push -u origin main             // 브랜치로 push
```
:이후 `git push`, `git pull` 만으로 push/pull 가능


## 제 2 유저
repo 다운로드
```
git clone "repo_url"
```
`git init`, `git remote`, `git branch` 등 생략가능


# 긴급 컴활
## 피벗 테이블
생략
## 데이터 유효성 검사
[데이터]-[데이터 도구]-[데이터 유효성 검사]
## 중복된 항목 제거
[데이터]-[데이터 도구]-[중복된 항목 제거]
데이터 영역내에 커서 위치
## 데이터 표
- 표 꼭지점에 수식 위치
- 표 전체 선택
- [데이터]-[예측]-[데이터 표]
- 행, 열에 해당하는 데이터 지정
## 목표값 찾기
[데이터]-[예측]-[목표값 찾기]
## (데이터) 찾기
대상 영역 헤더 포함 선택
[데이터]-[데이터 도구]-[통합]
## (데이터) 정렬
[데이터]-[정렬 및 필터]-[정렬]
## 부분합
- 정렬 먼저 실행
- [데이터]-[윤곽선]-[부분합]
- 그룹화할 항목은 정렬한 항목으로 설정
## 시나리오
- 셀 이름 정의(결과창을 위해)[\*[수식]-[정의된 이름]]
- [데이터]-[예측]-[시나리오 관리자]
- [요약]
## 차트
