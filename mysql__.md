# 관계형 데이터베이스 용어 정리




### Table (aka Relation)​
      테이블은 이름을 가지고 있으며, 행(row)과 열(column) 그리고 거기에 대응하는 값을 가짐.
      관계형 데이터베이스는 위와 같이 구성된 테이블이 다른 테이블들과 관계를 맺고 모여있는 집합체임
     
### Field (aka Column, Attribute)​
      각각의 열은 유일한 이름을 가지고 있으며, 자신만의 타입을 가지고 있음.
      이러한 열은 필드(field) 또는 속성(attribute)이라고도 불림


### Record (aka Row, Tuple)​
      값의 나열(리스트) 즉, 테이블의 행 (때로는, 레코드 라고도 함)


### Database (aka Schema)
```
 데이터 베이스의 구조를 전반적으로 기술한 것. 구체적으로 데이터베이스를 구성하는 데이터 개체(Entity), 속성(Attribute), 관계(Relationship) 등을 정의 한 것을 말한다. 사용자의 관점에 따라 외부 스키마, 개념 스키마, 내부 스키마로 구분한다. DBMS는 외부 스키마에 명세된 사용자의 요구를 개념 스키마 형태로 변환하고, 이를 다시 내부 스키마 형태로 반환한다. 
```


### Primary Key(PK)
     릴레이션 내 투플을 식별할 수 있는 고유한 값을 가져야 한다.
     NULL 값은 허용하지 않는다.


### Foreign Key(FK)
     관계 데이터 모델의 릴레이션 간의 관계를 표현한다.
     참조되는 값이 변경되면 참조하는 값도 변경된다.
     NULL 값과 중복 값 등이 허용된다.