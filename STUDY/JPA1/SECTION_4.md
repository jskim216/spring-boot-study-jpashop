## 회원 리포지터리 개발

### @PersistenceContext, EntityManager
- @PersistenceContext , EntityManager 선언으로 스프링이 EntityManager 를 생성하여 주입해줌
- EntityManager 는 @PersistenceContext 가 반드시 있어야(표준어노테이션) 주입되지만 
  스프링 데이터 JPA 가 @PersistenceContext 없이도 @Autowired 로 주입 지원 


- em.createQuery() JPQL 작성시


### @Transactional
- spring 에서 제공하는 @Transactional 을 사용하는 것이 유리
- 조회, 읽기 등에는 @Transactional(readOnly = true) 를 사용하는 것이 성능 최적화에 유리함
- Class 레벨에서 @Transactional(readOnly = true) 를 적용하고 쓰기가 필요한 메소드에서 @Transactional 지정으로 처리할 수 있음
- Test 시의 @Transactional 사용시 롤백이 되므로 @Rollback(value = false) 를 통해 롤백처리를 막을 수 있음

### Test 단계의 H2 메모리 db 사용
- test 디렉토리 아래에 resources/application.yml 설정
- 