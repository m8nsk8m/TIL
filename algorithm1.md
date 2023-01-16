# 코딩테스트 준비하기




## 기본 입출력

### 입력(Input) 예시

 * `a = input()`
    문자열 입력 받기
 * `b = int(input())`
    한 개 숫자 입력 받기
 * `d, e = map(int, input().split())`
    여러 개 숫자 입력 받기

 * map 함수 활용
    ```
    # 각 원소에 int를 적용
    a, b, c = map(int, ['1', '2', '3']) 
    a, b = map(int, '1 2'.split())
    a, b = map(int, ['1', '2'])
    a, b = 1, 2
    ```



### 출력 예시 (print)


 *  ```
    a = 'Hello'
    b = 'world'

    print(a, b)
    >>> Hello world
    ```

 * `sep = ' '` 의 역할 
    - separate의 줄임말 즉 각 문자열 객체 사이를 무엇으로 구분 할 것인가 이다.
    - sep은 무조건 문자열로 설정되어야 한다.
    - 기본값은 '' 공백이다. 따로 설정하지 않으면 기본값이 설정된다.

 * `end = '\n'`
    - end는 마지막에 붙는 문자열 무조건 문자열로 설정되어야 함
    - 기본값은 escape code /n 이다.

 * end 와 sep 사용하기
    ```
    a = 'Hello'
    b = 'world'

    print(a, end='@')
    print(b)
    >>> Hello@world
    
    print(a, b, sep='\n')
    >>>Hello
    >>>world
    

 * escape code \n 사용하기
    ```
    print('Hello world\nI'm Minsun\nNice to meet you')
    >>>Hello world
    >>>I'm Minsun
    >>>Nice to meet you
    ```




## 알고리즘

### 알고리즘이란?
 * 어떤 문제를 해결하기 위해 정해진 일련의 절차나 행동
 * 문제란 Input을 넣었을 때, 원하는 Output이 나오도록 하는 것



### 코딩테스트를 위한 문제풀이 연습 꿀팁
 1) 변수명 대충칫지 않기..
 2) 언어의 내장 함수, 라이브러리를 적극 활용
 3) 함수화를 통해 가독성 높이기
 4) 문제풀이를 적어보거나 코드리뷰를 통해 설명하는 연습 반드시 필요


### 데이터 구조 & 알고리즘
 * 프로그램 == 데이터 구조 + 알고리즘

 * 파이썬의 기본 데이터 구조 
   - 컨테이너
        - 시퀀스형
            - 리스트
            - 튜플
            - 레인지
        - 비시퀀스형
            - 세트
            - 딕셔너리