# 컴퓨터 프로그래밍 언어


## 사용자 정의 함수


### 학습 목표
 1) 함수를 직접 정의하고 활용 할 수 있다.
 2) 함수 정의에 맞게 호출하고 실행시킬 수 있다.
 3) 스코프를 이해하고 설명할 수 있다.
 4) 파이썬의 이름 검색 규칙을 설명할 수 있다. 



### 함수 기본 구조
 * 선언과 호출(define & call)
 * 입력(Input)
 * 범위(Scope)
 * 결과값(Output)



### 선언과 호출 
`def`

 * 함수의 선언은 **def** 키워드 활용
 * 들여쓰기를 통해 Fuction body(실행될 코드 블록)를 작성함
 * 함수는  parameter를 넘겨줄 수 있음
 * 함수는 동작 후에 return을 통해 결과값을 전달함
 * 함수는 `함수명()` 의 형식으로 호출
    - parameter가 있는 경우, 함수명(값1, 값2, **)로 호출
    
    ```
    * foo()/foo=함수이름
    def foo():
        return True
    
    * add(2, 3)
    def add(x, y):
        return x + y
    ```


### 함수의 결과값 (Output) 
`return`

 * 함수는 반드시 값을 하나만 return한다.
     - 명시적인 return이 없는 경우에도 None을 반환함
 * 함수는 return과 동시에 실행이 종료된다.
    ```
    def foo():
        return 1  -> 얘만 출력되고
        return 2    -> 얘는 출력안댐 위에서 종료되었기 때문
                    
    print(foo()) # 1
    ```
 * 여러 값을 return 하는 경우 : tuple   
    ```
    def foo():
        return 1, 2, 3
    print(foo()) # (1, 2, 3)
    print(type(foo())) # <class 'tuple'>
    ```
 * return vs print
     - return은 함수 안에서 값을 반환하기 위해 사용되는 키워드
     - print는 출력을 위해 사용되는 함수


### 함수의 입력 (Input) 
 * Parameter : 함수를 실행할 때, 함수 내부에서 사용됨
 * Argument : 함수를 호출 할 때, 넣어주는 값
    ```
    def function(ham): # parameter : ham
        return ham
  
    function('spam')  #argument: 'spam'
    ```
 * positional arguments
    - 위치에 맞게 함수에 전달됨
    ```
    def add(x, y):       add(2, 3) -> 2 == x, 3 == y
        return x + y
    ```
 * keyword arguments
    - 직접 변수의 이름으로 특정 argu를 전달


 * Defult Arguments Values
    - 기본값을 지정하여 함수 호출 시 argument 값을 설정하지 않도록 함


 *  정해지지 않은 개수의 argu
    - argument들은 튜플로 묶여 처리되며, parameter에 *를 붙여 표현
    
    ```
    def add(*numbers):
        print(type(numbers)) # <class 'tuple'>
    ```    
 
 * 정해지지 않은 개수의 keywork argu
    - 딕셔너리로 묶여 처리, parameter에 **을 붙여 표현

    ```
    def movie(**kwargs):
        return kwargs
    
    print(movie(name='더 글로리', writer='김은숙))
    # {'name': '더 글로리', 'writer': '김은숙}
    ```



 * 함수의 범위 (Scope)
    
    