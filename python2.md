#

## 컨테이너
### 리스트(List)
 * 리스트란?
    - 변경 가능한 값들의 나열된 자료형
    - 순서를 가지며, 다른 타입의 요소 가질 수 있음
    - 변경 가능(mutable), 반복 가능(iterable)
    - 항상 대괄호 [] 로 정의 하며, 요소는 콤마 , 로 구분
    - 각 요소는 0부터 시작하는 인덱스를 사용하여 접근 할 수 있다.
 * 리스트의 생성과 접근
    - 대괄호[] 혹은 list()를 통해 생성
    ```
    myList = [1, 2, 3, 4]
    newList = myList[:]
    newList2 = list(myList)

    list = [] 빈 리스트도 생성가능
    ```
    - 순서가 있는 시퀀스로 인덱스를 통해 접근 가능

    ```
    # 값 접근
    a = [1, 2, 3]
    print(a[0])
    # 1

    # 값 변경
    a[0] = '1'
    print(a)
    # ['1', 2, 3]
    ```


 * 리스트 값 추가/삭제
    - 추가는 `.append()` 를 활용 (맨 뒤에 추가됨)
    ```
    even_numbers = [2, 4, 6, 8]
    even_numbers.append(10)
    even_numbers
    # [2, 4, 6, 8, 10]
    ```

    - 삭제는 `.pop()` 과 `remove()`를 활용
     ```
    even_numbers = [2, 4, 6, 8]
    even_numbers.pop(0)  --> 원하는 위치의 값 삭제
    even_numbers.remove('2')  --> 요소
    print(even_numbers)
    # [4, 6, 8]
    ```

    
    








### 레인지(Range)
 * range(n=0, m, s=1)
    
    * 숫자의 시퀀스를 나타내기 위해 사용
        
        `기본형 : range(n)`
        * 0부터 n-1까지

        `범위지정 : range(n, m)` 
        * n부터 m-1까지

        `범위 및 스템 지정 : range(n, m, s)`
        * n부터 m-1까지 s만큼 증가시킴

    * 변경 불가능하며(immutable), 반복 가능함(iterable)



 * for 와 range
    
    * for 구문과 range의 특성을 이용해 오름차순과 내림차순을 지정할 수 있다.
   
         ```
        for i in range(0, 10) =>  오름차순

        for i in range(9, -1 or 0 - 1, -1) => 내림차순
        for i in reversed(range(0, 10)) => 내림차순
         ```


### 반복문(Loop Statement)
     특정 조건을 도달할 때까지, 계속 반복되는 일련의 문장

 * 반복문의 종류

    1) while 문
        * 종료조건에 의해 반복문이 종료됨
    
    2) for 문
        * 반복가능한 객체를 모두 순회하면 종료 (별도의 종료조건 필요없음)
    
    3) 반복 제어
        * break, countiue, for-else


### while문
 * while문은 조건식이 참인 경우 반복적으로 코드를 실행
    
    ```
     while <expression>:
        # Code block
    ```
    
    * 조건이 참인경우
        - 들여쓰기 되어 있는 코드 블럭이 실행 됨
        - 코드 블럭이 모두 실행되고, 다시 조건식을 검사하며 반복적으로 실행
        - while문은 무한 루프를 하지 않도록 종료조건이 반드시 필요

 

 * 실습 


### for문
 * for문은 시퀀스(문자열, 튜플, 리스트, 레인지)를 포함한 객체요소를 모두 순회함
     
    
    ```
     for <변수명> in <iterable>:
        # Code block
    ```
    
    
    
     * 처음부터 끝까지 모두 순회함으로 **종료조건 필요 없음**
     * 순회 가능한 객체 : 컨테이너형(문자열, 리스트, 튜플, 레인지, 딕셔너리)등


 * 문자열 순회
     * 사용자가 입력한 문자를 한글자씩 세로로 출력




    