---
title: Java Annotation

categories:
    - Dev
tags:
    - Java
    - JPA
late_modified_at: 2019-12-10T23:00:00
---

##  Used Java Annotation ##

### Lombok ###
> 멤버 변수에 대한 Getter/Setter Method, Equals(), hashCode(), toString() 과 멤버 변수에 값을 설정하는 생성자 등을 자동으로 생성해주는 라이브러리

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@Data` | @Getter, @Setter, @ToString, @EqualsAndHashCode 등 자동 생성 |
| `@Builder` | Builder API 처럼 사용할 수 있도록 지원 |
| `@AllArgsConstructor` | 모든 인자를 가진 생성자를 생성 |
| `@NoArgsConstructor` | 인자 없는 생성자를 생성 |
| `@Slf4j` | Simple Logging Facade For JAVA <br> 로깅에 대한 인터페이스 모음 |
| `@Getter` | Getter 메소드를 생성해준다. |
| `@Setter` | Setter 메소드를 생성해준다. |
| `@ToString` | ToString 메소드를 생성해준다. |
| `@EqualsAndHashCode` | Equals(두 객체의 내용이 같은지)메소드와 Hashcode(두 객체가 같은 객체인지)메소드를 생성해준다.  |


### JPA ###
* Java Persistent API
* 자바 진영의 ORM 표준 기술
* 자바를 이용해서 데이터를 관리(유지)하는 기법을 하나의 스펙으로 정리한 표준

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@Entity` | JPA를 사용해서 테이블과 Mapping할 클래스에 부여하는 Annotation (파라미터가 없는 기본 생성자 필수) |
| `@Table` | Entity가 Mapping 할 테이블을 지정하는 Annotation(테이블 명칭 등과 같은 속성 제공) |
| `@Id` | 기본키 지정 Annotation |
| `@GeneratedValue` | 식별자 자동 생성 Annotation |
| `@Column` | Database의 Column과 Mapping되는 Annotation(Column명, Constraints 등 속성 제공, 생략 가능) |
| `@OneToOne` |  |
| `@OneToMany` |  |
| `@ManyToOne` |  |
| `@JoinColumn` |  |
| `@EntityListeners` |  |
| `@Temporal` |  |


### Spring-Web ###

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@RestController` |  |
| `@RequestMapping` |  |
| `@GetMapping` |  |
| `@PostMapping` |  |
| `@PutMapping` |  |
| `@DeleteMapping` |  |
| `@ExceptionHandler` |  |
| `@RestControllerAdvice` |  |


### Spring-data-commons ###

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@CreatedDate` |  |
| `@CreatedBy` |  |
| `@LastModifiedDate` |  |
| `@LastModifiedBy` |  |
