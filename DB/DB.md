# DB 설계 Tips!

---

<h3>Table을 선정할 떄 고려해야 할 점</h3>

- 정확하고 모호하지 않은 이름   
- 전체 조직이 이해가능한 서술적 이름(명사 -> 동사화)
- 단수형을 사용
- 이름을 짧게
- 약어는 사용 X
- 물리적 특성 사용 X

<h3>Relation</h3>

- 두 개 테이블의 관계 = 데이터를 공유하는 방법
- 1:1 (1 대 1) = 한 개의 테이블의 상세내용
  ```
  ex) Product <=> ProductDetails
  Product (ProductID, name, description, quantity, unitprice, ... )
  ProductDetails (ProductID, moreDescription, image, ... )
  ```
- 1:m (1 대 다)= 한 개 테이블과 관련된 m개의 instance정보를 다른 테이블이 가짐
- m:n (다 대 다)= Linking table
  
<h3>Attribute</h3>

- 속성은 특징 한개의 집합 = 다중특징 X
- 반드시 Primary Key를 지정해야함
- 기본키는 Stirng? Autoincrement?
- 이후에 변경이 생겼을때 대처할 수 있는가?
- 필요한 경우 Compound Key(복합키)를 사용함
- 중복되어 저장되는 속성이 없도록 함 (정규화)
- 계산 속성은 View를 통해서 업데이트 해서 제공
- 계산 속성은 테이블의 변경, 삭제 등 떄마다 업데이트 필요
- 모든 테이블을 다 찾아서 업데이트 하는 건 어려울 수 있음