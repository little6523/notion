# Mybatis에서 foreach 사용 시 SQL 구문 오류 발생

- 문제 상황
    - where절에서 foreach를 사용할 때 구문 오류가 발생

- 관련 코드(실무 코드이므로 공개 x)
    
    ```jsx
    
    ```
    

- 해결 방법
    - foreach에서 사용하는 파라미터값(리스트 등)이 비어있으면 foreach가 동작하지 않으므로 쿼리가 제대로 완성되지 않아 오류발생
    ⇒ 서비스 클래스에서 null 및 값이 비어있는지 확인하는 로직 추가
