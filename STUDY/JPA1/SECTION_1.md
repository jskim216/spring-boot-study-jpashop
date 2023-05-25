### 커넥션 풀과 hikariCP
https://code-lab1.tistory.com/209

### thymeleaf
- 장점
  - 마크업을 깨지않고 그대로 사용함 (웹 브라우져에서도 열어서 볼 수 있음)
- 단점
  - 3.0 으로 업데이트 되면서 많이 개선됨
  - 매뉴얼 학습필요
- viewName 매핑
  - resources:templates/ +{ViewName}+ .html

### spring ui Model
- data 를 가지고 view 단으로 넘길 수 있음

### spring-boot-devtools
- view 화면 등을 서버 재시작없이 갱신해주는 라이브러리

### DB 연결 설정
- show_sql: true 은 시스템상에서 찍는거므로 안씀 logging 을 사용

### @PersistenceContext
- 스프링 부트가 해당 @PersistenceContext 애노테이션을 읽고 엔티티 매니져를 생성하여 주입해줌

### EntityManager
- EntityManager 를 포함한 모든 데이터 변경은 반드시 트랜잭션 안에서 수행해야함
- @Transactional 이 @Test 안에 있을 시 수행 후 롤백함
- 같은 트랜잭션 안에서는 같은 영속성 컨텍스트 안에서는 식별자가 같으니 같은 개채로 봄

### 쿼리 파라미터 로그 남기기
- org.hibernate.type: trace

### p6spy
- https://github.com/gavlyukovskiy/spring-boot-data-source-decorator
- 개발간 활용 / 운영단계는 검토 필요