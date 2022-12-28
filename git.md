# git (분산 버전 관리 시스템)

## 버전 관리란?
* 동일한 정보에 대한 여러 버전을 관리하는 것을 말한다.
* git은 버전 관리 소프트웨어중 하나이다.





## git이란?
* 분산버전관리시스템으로 코드의 버전을 관리하는 도구
* 리누스 토르발스(리눅스만든사람!)가 개발함.
* 컴퓨터 파일의 변경사항 추적, 협업을 하기에 용이함.




## 저장소(repository) 만들기

### *git 버전 관리의 흐름*
> 1. 작업을 하고 / directory에
> 2. 변경된 파일을 모아 (add) / 커밋할 파일 상태 목록(staging area)
> 3. 버전으로 남긴다 (commmit) 
>   >* modifed : 파일이 수정된 상태  ($ git add)
>   >* staged : 곧 커밋할 수정된 파일  ($ git commit)
>   >* committed : 커밋된 상태




### *저장소 생성(초기화)*
```
$ git init
```
> * 특정 폴더에 git 저장소를 만들고 버전 관리
>   >* .git 폴더가 생성됨
>   >* git bash에서는 (master)라는 표기를 확인할 수 있음




### *add 커밋 대상 기록*
```
$ git add
```
> * working directory상의 변경 내용을 staging area에 추가하기 위해 사용 
>   >* untracked 상태의 파일을 staged로 변경
>   >* modified 상태의 파일을 staged로 변경


### *커밋메세지 (버전 기록)*
```
$ git commit -m 
```
> * straged 상태의 파일들을 커밋을 통해 버전으로 기록
> * 커밋 메세지는 변경 사항을 나타낼 수 있도록 명확하게 작성해야 함


### *상태(파일 변경 상태)*
```
$ git status (working directory, staging area)
$ git log (Repository)
```
> * git 저장소에 있는 파일의 상태를 확인하기 위하여 활용
>   > * 파일의 상태를 알 수 있음
>   >   > * untracked files
>   >   > * changes not staged for commit
>   >   > * changes to be committed
> * status로 확인할 수 있는 파일의 상태
>   > * tracked : 이전부터 버전으로 관리되고 있는 파일 상태
>   >   > * unmodified : git status에 나타나지 않음
>   >   > * modified : changes not staged for commit
>   >   > * staged : changes to be committed
>   > * untracked : 버전으로 관리된 적 없는 파일 상태 (파일을 새로 만든 경우)


### *로그(커밋 기록 조회)*
```
$ git log
```
> * 현재 저장소에 기록된 커밋을 조회
> * 다양한 옵션을 통해 로그 조회 가능


### *파일 관리 상태 라이프 사이클*

사진 첨브

### *명령어 정리*
