# basic command
> git 기본 문법 정리

## 초기 설정
- git을 설치 후 한번만 실행
```bash
git config --global user.email <이메일>
git config --global user.name <이름>
```

## git 저장소 만들기
- `git init` 
    - `.git directory`를 생성해주는 명령어
    - 관리하고 싶은 최상위 위치에서 실행함.  

## GIT 상태 체크
- status
    - 현재 git으로 관리되고 있는 파일/폴더 상태를 출력

## 코드 수정하고 저장소에 저장하기
-`add`  
    -  `git add <파일/폴더이름>`  
    - `working directory` 에서 `staging area`로 추가  
    - 일반적으로 모든 파일, 폴더를 추가하기 위해 아래의 코드를 사용  
        - `git add .`
- `commit`
    - `git commit -m `메세지``
    - `staging area` 에 올라간 파일들의 스냅샷을 찍어서 `.git dicertory`에 저장. 
    - 일반적으로 `-m` 옵션을 넣어서 메세지를 추가하여 등록


## 원격저장소에 업로드하기

- `remote add`
    - `git remote add <원격저장소이름>origin <URL>`
    - 원격 저장소 주소를 origin이라는 이름으로 저장
-`push`
    - `git push <원격저장소이름><브랜치이름>`
    - 원격저장소에 브랜치를 업로드