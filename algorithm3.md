# 문자열(String)
> 문자열은 immutable(변경 불가능) 자료형이다. 그러므로 문자열을 조작하기 위해서는 형변환과 조작방법을 알고 있어야 한다.


## 목차
 1) 문자열 조작
 2) 문자열 메서드
 3) 아스키(ASEII) 코드



## 학습목표
 * 문자열을 인덱스로 접근하고 슬라이싱 할 수 있다.
 * 문자열을 조작하는 유형을 알고 활용할 수 있다.
 * 문자열 메서드와 그 결과를 설명할 수 있다.






## 문자열 조작

### 문자열 슬라이싱




## 문자열 메서드

 1) `.split(기준문자)` 
 - 문자열을 일정 기준으로 나누어 리스트로 반환
 - 괄호 안에 아무것도 넣지 않으면 자동으로 공백을 기준으로 설정
    ```
    word = 'I play the piano'
    print(word.split())
    ['I', 'play', 'the', 'piano']
    ```

 2) `.strip(제거할 문자)`
 - 문자열 *양쪽 끝*에 있는 특정 문자를 모두 제거한 *새로운 문자열 반환*
 - 괄호 안에 아무것도 넣지 않으면 자동으로 공백을 제거 문자로 설정
 - 제거할 문자를 여러개 넣으면 해당하는 모든 문자들을 제거


 3) `.find(찾는 문자)`
 - 특정 문자가 처음으로 나타나는 *위치(인덱스)*를 반환
 - 찾는 문자가 없다면 *-1*을 반환


 4) `.index(찾는문자)`
 - 특정 문자가 처음으로 나타나는 위치(인덱스)를 반환 
 - 찾는 문자가 없다면 *오류* 발생

 5) `.count(개수를 셀 문자)`
 - 문자열에서 특정 문자가 몇 개인지 반환
 - 문자 뿐만 아니라, 문자열의 개수도 확인 가능 == len() ?


 6) `.replace(기존문자, 새로운문자)`
 - 문자열에서 기존 문자를 새로운 문자로 수정한 새로운 문자열 반환
 - 특정 문자를 빈 문자열('')로 수정하여 마치 해당 문자를 삭제한 것 같은 효과 가능


 7) `삽입할 문자.join(iterable)`
 - iterable의 각각 원소 사이에 특정 문자를 삽입한 새로운 문자열 반환
 - 공백 출력, 콤마 출력 등 원하는 출력 형태를 위해 사용






## 아스키(ASCII)코드

 * ord(문자)
    - 문자 -> 아스키코드로 변환하는 내장함수

 * chr(아스키코드)
    - 아스키코드 -> 문자로 변환하는 내장함수

