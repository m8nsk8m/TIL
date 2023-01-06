
# 모듈과 예외처리



## 컬렉션



### 딕셔너리
 * 키 - 값 (key - value) 쌍으로 이뤄진 모음(collection)
    
    * 키(key)
        * 불변 자료형만 가능(리스트, 딕셔너리 X)

    * 값(values)
        * 어떠한 형태든 관계 없음


 * 키와 값은 `:`로 구분 된다. 개별 요소는 `,` 로 구분된다.
 * `{}` 중괄호 안에 키와 값을 넣는다.
        
        
     `sutdents = {'홍길동' : 30, '김철수' : 25}`

 * 변경 가능하며, 반복 가능함
    * 딕셔너리는 반복하면 키가 반환 됨



 

### 딕셔너리의 생성
 * 키와 값이 쌍으로 이뤄진 자료구조
    * 키는 별경 불가능한 데이터만 활용가능
    * 값은 모든 값으로 설정 가능 (리스트 딕셔너리도)
    ```
     dict_c = {[1, 2, 3]: 'hi'} (x)
     dict_c = {'hi': [1, 2, 3]} (o)
    ```


### 딕셔너리의 접근
 * `딕셔너리명[key값]` 의 형태로 사용함
 *  하나의 딕셔너리에 같은 key 값이 동시에 저장될 수는 없다.
  ```
  dic = {1: 'MY', 2: 'Name', 3: 'Is'. 4: 'python'}


  print(dic[1])
  print(dic[2])
  print(dic[3])
  print(dic[4])

  MY
  Name
  Is
  python
  ```




### 딕셔너리의 키-값 추가 및 변경
 * 키와 값의 쌍을 추가할 수 있음
 * 이미 해당하는 키가 있다면 기존 값이 변경
    ```
    

