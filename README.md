# QueryDSL 학습을 위한 리포지토리
1. QueryDSL
   - 자바 코드로 부터 DB 쿼리를 생성해주는 도구
   - 타입 세이프가 지켜지지 않는 HQL의 가독성이 떨어지는 Criteria 대체제
   - Type-Safety하지 않아 불안정한 JPQL, em을 직접 사용 해야하고 어려운 Criteria Query
2. Q클래스
   - QueryDSL이 자동으로 생성해주는 클래스
   - Q클래스를 이용해 가독성 좋은 쿼리 작성 가능
   - 편리한 Join과 스프링이 제공해주는 Pagealbe 등 스프링과의 연동성 보장
   - 다이내믹하게 where절을 추가 가능
   - fetchCount()를 이용해 쉽게 카운트 쿼리 호출 가능
   - QueryDsl 인스턴스를 가져와 에러처리 가능하고 쉽게 조인과 페이징이 가능
     - 복잡한 페이징을 구현할 때에도 Pageable만 잘 만들어두면 쉽게 페이징 가능
3. Jooq
   - DB 스키마를 자바 클래스로 바꿔주는 도구
   - ORM 프레임워크가 아니며 SQL을 잘 활용하기 위한 도구로 JPA 함께 사용하면 좋다.
   -