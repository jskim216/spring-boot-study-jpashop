- @NotEmpty 사용 관련
- implementation 'org.springframework.boot:spring-boot-starter-validation' 추가
- validation 을 통해 필수값 체크를 해줌 - @Valid 
- BindingResult 를 통해 결과값 핸들링 가능

- form 과 엔티티는 구분해서 사용하는 것이 좋음
- 실무에서는 화면에 출력시에도 엔티티를 직접 전달하기보다는 DTO 형태로 전달하는게 좋음
- API 만들때에는 엔티티를 외부로 반환하면 안됨!



- PathVariable

### 수정시의 변경 & 병합
- 