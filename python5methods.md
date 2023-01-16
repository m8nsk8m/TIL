

# 타입과 메서드

## 학습목표
 1) 메서드와 함수의 차이점은?

 2) 파이썬의 주요 객체(타입)의 메서드를 비교

 3) 메서드별 필수 인자와 결과값 에측
    ```
    타입.메서드()
    input().split()
    [1, 2, 3].append()
    ```
 
## 시퀀스 (string, list, tuple, range) 메서드
### 문자열(String)
 * 문자열의 특징
    - 모든 문자는 str 타입
    - 문자열은 작은 따옴표(')나 큰 따옴표(")를 활용
    - 문자열을 묶을 때 동일한 문장부호 사용

 * 메서드
   - `{} + format()`
      - print('{} {}'.format['hi', 'python'])
   
   - `f-string`
      - print(f'어쩌구 저쩌구 {hi}, {python})
   
   - `s.find(x)`
      - x의 첫 번째 위치를 반환, 없으면 -1을 반환
   
   - `s.index(x)`
      - x의 첫 번째 위치를 반환, 없으면 오류 발생

 > is~~로 시작하는 메서드는 Boolean 형식이다.
   
   - `s.isalpha()`
      - 알파벳 문자 여부

   - `s.isupper()`
      - 대문자 여부
   
   - `s.islower()`
      - 소문자 여부
   
   - `s.istitle()`
      - 타이틀 형식 여부

   - `s.replace(old, new[count])`
      - 바꿀 대상 글자를 새로운 글자로 바꿔서 반환
      - count를 지정하면, 해당 개수만큼만 시행
         ```
         print('coone'.replace('o', 'a'))
         # caane
         print('wooooowoo'.replace('o', '!', 2))
         # w!!ooowooo
         ```  
   
   - `s.strip([chars])`
      - 공백이나 특정 문자를 제거
   
   - `s.split( , )`
      - 문자열을 특정한 단위로 나눠 *리스트로 반환*
         ```
         print('a,b,c'.split('_'))
         # [a,b,c]
         print('a b c'.split()) # 공백으로 나누기
         # ['a', 'b', 'c']



   - `'separator'.join([iterable])
      - 구분자를 기준으로 iterable을 합침
      - 반복가능한 컨테이너 요소들을 seperator(구분자)합쳐 문자열 반환
         - iterable에는 문자열만 가능 아니면 TypeError 남
         ```
         print(''.join(['3', '5']))
         # 35
         ```
         ```
         (1) join메서드 이용
         result = ['1', '5', '3']
         print(''.join(result))
         # 153
         result = ['1', '5', '3']
         print(' '.join(result))
         # 1 5 3
         ```
         ```
         (2) 반복하면서 문자열 만들기
         result = ['1', '5', '3']
         text = ''
         for elem in result:
         text = text + elem
         print(text)   #153
         print(type(text)) # str
         ```

### 리스트(List)

 * 리스트의 특징
   - 변경가능, 반복가능
   - 순서를 가짐, 서로 다른 타입의 요소
   - 항상 대괄호 형태로 정의 요소는 콤마로 구분
 
 * 메서드
   - `l.append(x)`
      - 리스트 마지막에 항목x 를 추가

   - `l.insert(i, x)`
      - 리스트 인덱스 i에 항목x를 삽입

   - `l.remove(x)`
      - 리스트 가장 왼쪽에 있는 항목(첫번째) x를 제거
      - 항목이 존재하지 않을 경우, ValueError
   
   - `l.pop()`
      - 리스트 가장 오른쪽에 있는 항목(마지막)을 반환 후 제거
   
   - `l.pop(i)`
      - 리스트의 인덱스 i에 있는 항목을 반환 후 제거

   - `l.extend(m)` 
      - 순회형 m의 모든 항목들의 리스트 끝에 추가(+=과 같은 기능!!)
   
   - `l.index(x, start, end)`
      - 리스트에 있는 항목 중 가장 왼쪽이 엤는 항목 x의 인덱스를 반환

   - `l.reverse()` 
      - 리스트를 거꾸로 정렬
      - 정렬아님, None 반환  
         ```
         문자열 거꾸로 하는법?
         text = 'hello!'
         print(type(text[::-1]))
         # !olleh
         ```
         ```
         리스트도 동일하다
         numbers = [3, 2, 10]
         print(numbers[::-1])
         [10, 2, 3]
         ```

   - `l.sort()`
      - 원본 리스트를 정렬. None 반환
      - sorted 함수와 비교할 것
         ```
         .sort()인 경우
         numbers = [3, 2, 5, 1]
         result = numbers.sort()
         print(numbers, result)
         # [1, 2, 3, 5] None  
         ```
         ```
         sorted 함수 일 경우
         numbers = [3, 2, 5, 1]
         result = sorted(nubers)
         print(numbers, result)
         # [3, 2, 5, 1] [1, 2, 3, 5] -> 변경 없음

   
   - `l.count(x)`
      - 리스트에서 항목 x가 몇 개 존재하는지 갯수를 반환
   
   - `l.clear()`
      - 모든 항목을 삭제함

   - `l.index(x)`
      - x값을 갗아 해당 index 값을 반환 


> reverse 나 sort 는 원본 자체가 바뀐다는것...


### 세트(set)
 * 세트의 특징
   - 유일한 값들의 모음
   - 순서 없음, 중복된 값 없음
   
 * 메서드
   - `s.add(x)`
      - 가 세트 s 에 없다면 추가
   
   - `s.pop()`
      - 세트s에서 랜덤하게 항목을 반환하고, 해당 항목을 제거

   - 세트 연산자 공부하기..


### 딕셔너리(dict)
 * 특징
   - 키-값 쌍으로 이뤄짐
   - 변경 가능, 반복 가능
      - 반복시에 키가 반환됨

   
 * 메서드
   
   - `d.keys()`
      - 키만 반환
   
   - `d.values()`
      - 값만 반환

   - `d.items()`
      - 키-값을 쌍으로 반환

   - `d.get(k)`
      - 키 k의 값을 반환, 없을 경우 None
         ```
         drama = {'name' : '더 글로리', 'writer' : '김은숙'}
         print(drama['director'])
         # KeyError 
         print(drama.get('director')) 기본값이 none임
         # None
         print(drama.get('director', 0)) 0은 초기값으로 설정됨
         # 0

   - `d.update()`
   


   - `.pop(key, )`
      - key가 딕셔너리에 있으면 제거하고 해당 값을 반환
      - 그렇지 않으면 default 반환
      - default값이 없으면 KeyError
         ```
         a = {'apple' : '사과', 'banana' : '바나나'}
         data = a.pop('apple')
         print(data, a)
         # 사과 {'banana': '바나나'}
         ```



