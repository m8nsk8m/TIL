# Git Branch

## Branch(브랜치)란?
```
프로젝트를 공유하고 같이 작업할 수 있도록 해주는 기능이다.
각자 로컬에서 독립적으로 작업이 가능하며, 각각의 브랜치는 다른 브랜치의
영향을 받지 않기 때문에 여러 작업을 동시에 진행할 수 있다.
즉, 브랜치 기능을 활용해 하나의 작업을 여러시점에서 개발 할 수 있다.
```

## Branch 주요 명령어

- ### 브랜치 생성
`$ git branch (branch name)`
> master브랜치에서 복사된 새로운 브랜치가 생성된다. 브랜치를 생성하지 않으면 master브랜치에서 작업하고 있는것이다.


- ### 브랜치 이동
`$ git checkout (branch name)`
> 브랜치 생성 후, 반드시 checkout을 해줘야 master에서 전환이 된다.
전환된 상태로 파일을 add commit 헤준다.

- ### 브랜치 생성 및 이동
`$ git checkout -b (branch name)`
> 브랜치를 만들면서 동시에 이동할 수 있다.

- ### 브랜치 목록 
`$ git branch`


- ### 브랜치 삭제
`$ git branch -d (branch name)`


## Merge란?
```
각 브랜치에서 작업 한 후 합치는 것을 말한다
merge를 할 때 commit 끼리 conflict 될 수 있다. 
conflict에는 두가지 경우가 있다.
- 동일한 파일을 수정한 경우
    이경우에는 해당 파일을 확인하고 수정한 이후에 직접 commit 할 것
- 다른 파일을 수정한 경우
    conflict 없이 자동으로 merge commit이 생성됨.
```


## Merge 주요 명령어

`$ git merge (branch name)`

- ### merge - fast foward
> * 기존 master 브랜치에 변경사항이 없어 단순히 브랜치 이동 후 commit
> 1) 이동한 브랜치 commit
> 2) master 변경 없음
> 3) master 브랜치로 merge



- ### merge - merge commit
> * 기존 master 브랜치에 변경사항이 있어 merge commit 발생
> 1) 이동한 브랜치 commit
> 2) master 브랜치 commit
> 3) master 브랜치 merge







