# 6. Git/GitHub

## ■ Git

- 컴퓨터 파일의 변경사항을 추적하고 여러 사용자들 간에 해당 파일 작업을 조율하기 위한 버전 관리 시스템(VCS)
- = SCM(Source Code Management) < SCM(Software Configuration Management)

## ■ Git Init

![6%20Git%20GitHub%200578602efc254aaeac5bb0cc5f239d1d/Untitled.png](6%20Git%20GitHub%200578602efc254aaeac5bb0cc5f239d1d/Untitled.png)

- 삭제 → git config —global —unset user.email

## ■ Git 저장소 추가

1. git init
2. git remote add origin [https://github.com/jkpark-104/starbucks.git](https://github.com/jkpark-104/starbucks.git)
    - origin이란 별칭으로 원격 저장소를 연결
    - git remote / git remote get-url origin / git remote -v
3. git add . → 변경사항을 추적할 특정 파일 지정( '.' ← 모든 파일로 설정) 
    - 새 파일 추가 시 다시 해줘야 함
4. git status
5. git commit -m 'Start Project' → 메시지(-m)와 함께 버전을 생성
    - git commit -m 'main.js 추가' → 메시지와 함께 추가된 버전을 생성
    - git commit → vim이 뜸
6. git log
7. git branch -M main : 브랜치 이름 바꿈
    - git branch
8. git push origin main
    - git push -u origin main → Branch 'main' set up to track remote branch 'main' from 'origin'.
    - origin이란 별칭의 원격 저장소로 버전 내역('main') 전송

## ■ Git Branch 추가

1. git branch '브랜치 이름' → 브랜치 생성
2. git checkout '브랜치 이름' → 브랜치 이동

## ■ Git Clone

1. 터미널에서 디렉토리 이동
2. git clone 깃주소 → 폴더도 자동으로 생김
3. code . → 새 창에 VS CODE 실행
    - code . -r → 현재 창에 VS CODE 실행

## ■ Git 버전 되돌리기

1. git reset —hard HEAD~1 → 버전 하나 되돌리기
2. git reset —hard ORIG_HEAD → 기존 최신 버전으로 되돌리기

## ■ 다른 환경에서 Git 시작하기

1. git clone 깃주소
2. code . -r
3. git branch -r (master 外 다른 브랜치 가지고오기)
4. git checkout -t origin/브랜치이름
    - git checkout -b 브랜치이름 → 브랜치 생성하고 로그인
5. git branch -d 브랜치이름 → 브랜치 삭제

## ■ 충돌, 로컬 병합

### 1. 충돌 전 상태로 리셋함

- git reset —hard HEAD~1

### 2. Git Hub에서 최신 상태를 가지고 옴

1. git pull origin master
2. 코드 정리
3. git add .
4. git commit -m '변경 내용'
5. git push origin master

## ■ CLI (Command Line Interface, CUI)

- Linux : 리누스 토발즈가 작성한 커널 혹은 GNU 프로젝트의 라이브러리와 도구가 포함된 운영체제
    - Bash (GNU Bourne Again SHell)
- Kernel : 하드웨어와 응용프로그램을 이어주는 운영체제의 핵심 시스템소프트웨어
    - 이미지

        ![6%20Git%20GitHub%200578602efc254aaeac5bb0cc5f239d1d/Untitled%201.png](6%20Git%20GitHub%200578602efc254aaeac5bb0cc5f239d1d/Untitled%201.png)

- Shell
    - sh : AT&T Bell 연구소의 Steve Bourne이 작성한 유닉스 쉘
    - csh : AT&T Bell 연구소의 Steve Bourne이 작성한 유닉스 쉘
    - bash : Brian Fox가 작성한 유닉스 쉘, 다양한 운영체제에서 기본 쉘로 채택
    - zsh : Paul Falstad가 작성한 유닉스 쉘, sh 확장형 쉘, 현재까지 가장 완벽한 쉘

    ```bash

    ```

- Vim ()
- Emacs