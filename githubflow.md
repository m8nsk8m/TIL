# GitHub Flow

## GitHub Flow란?
```
여러 개발자가 git을 활용하여 branch의 생성, 삭제, 병합을 통해 협업하는
브랜치 전략이다.
git flow에 정해진 답이 있는 것은 아니다. 각자의 프로젝트/회사에서 알맞게 변형되어 활용되고 있다.
가장 대표적으로 활용되는 전략은 다음과 같다.
```






### GitHub flow Branch Name 
* `master` : 배포 가능한 상태의 브랜치 (main)
* `develop` : 다음 패치를 대비하여 개발하는 브랜치 (main)
* `featre branches` : 추가 기능 개발 브랜치
* `realse branches` : 개발 완료 후 QA/Test 후 master 브랜치로 merge
* `hotfixes` : 긴급하게 반영 해야하는 버그 수정용 브랜치

![gitflow](https://images.velog.io/images/seongwon97/post/5994c1a6-cdfd-4c73-84ea-842f9f7b001e/image.png)








### GitHub Flow 기본 원칙

1. master branch는 반드시 배포 가능한 상태여야 한다.
2. feature branch는 각 기능의 의도를 알 수 있도록 작성한다.
3. 커밋 메세지는 매우 중요하며, 명확하게 작성한다.
4. **Pull Request**를 통해 협업을 진행한다.
5. 변경사항을 반영하고 싶다면, master branch에 병합한다.






