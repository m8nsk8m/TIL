# 파일 입출력


## 학습 목표

 * 파이썬 활용하여 파일을 읽고 쓸 수 있다.
 * JSON 형식의 파일을 읽고 활용할 수 있다.



### 파일 입력
 * `open(file, mode='r', encoding=None)` -> 괄호안의 요소를 인자라고 한다
    - file : 파일명
    - mode : 텍스트 모드
    - encoding : 인코딩 방식 (일반적으로 utf-8 활용)
        
        
         Character|Meaning
        ------|-----
        'r'|읽기 모드(기본)
        'w'|쓰기 모드
        'a'|이어쓰기모드
        

        ** Character : 컴퓨터가 기억하거나 송출 할 수 있는 숫자나 알파벳
    
 * 파일 객체 활용
    -  ```
        f = open('workfile', 'w')
       ``` 

 * with 키워드 활용 (강사님이 추천하는 방식)
    - ```
       with open('workfile') as f:
            read_data = f.read()

       f.closed
       ```
    - with 키워드를 사용하지 않으면, f.close()를 반드시 호출하여 종료시켜야함.


### JSON
 * json은 자바스크립트 객체 표기법으로 개발활경에서 많이 활용되는 데이터 양식
 * 웹 에서 데이터를 전송할 때 사용
 * 문자기반(텍스트) 데이터 포멧으로 다수의 프로그래밍 환경에서 쉽게 활용 가능


#### JSON 파일의 활용
 * 객체(리스트, 딕셔너리 등)를 jSON으로 변환
    ```
    import json
    x = [1, 'simple', 'list']
    json.dumps(x)
    ```

 * JSON을 객체(리스트, 딕셔너리 등)로 변환
    ```
    X = json.load(f)
    ```



 * pprint
    - 임의의 파이썬 데이터 구조를 예쁘게 인쇄 할 수 있는 기능을 제공 
     ```
    import json
    from pprint import pprint
    with open( , , , ) as f:
    movie = json.load(f)  --> '파싱' 한다고 함
    pprint(movie)  --> 예쁘게 개행해서 보여줌 ㅎㅎ
    ```