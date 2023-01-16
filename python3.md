# 함수



## 함수란?

 > 함수란 특정 값 x를 인수(arguments)로 전달받으면,
 > 반드시 특정 값 y라는 결과로 반환(return)하는 일죵의 계산기와 같다고 볼 수 있다.
 > 파이썬에는 다양한 내장 함수 가 있고, 이러한 함수를 사용하는 이유는
 > 중복적인 코드의 작성을 최소화, 코드의 재사용성을 높여주기 때문이다.


 1) 함수를 사용하지 않고 평균을 구할 경우 (사용자 함수)
    ```
    numbers = [1, 10, 100]
    result = 0
    cnt = 0
    for number in numbers:
        result += number
        cnt += 1
    print(result/cnt)
    ```

 2) 함수를 사용하여 평균을 구할 경우 (내장함수 활용)
    ```
    numbers = [1, 10, 100]
    print(sum(numbers)/len(numbers))
    ```

 > 이처럼 코드 중복 방지, 재사용이 용이하기 때문에 함수를 사용해야 한다.


## 내장 함수

### 자주 사용하는 함수



#### 수학 관련 함수
* `len()`  
        - 객제의 길이를 반환

     
     
* `sum()`   


* `max()`


* `min()`


* `abs()`
 

* `divmod(a, b)`
    - 두 수를 받아 몫과 나머지를 반환


* pow(base, exp, mod=None)
    - base의 exp거듭제곱을 반환
    


]
#### 논리 관련 함수

* all()
    - 모든 요소가 참이면 (또는 비어있으면) True 반환

* any()
    - 요소중 어느 하나라도 참이면 True 반환
    - 비어있으면 False

