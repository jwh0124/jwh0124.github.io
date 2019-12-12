---
title: Java Annotation

categories:
    - Dev
tags:
    - Java
    - JPA

toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"

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
| `@EqualsAndHashCode` |  |


### JPA ###
* Java Persistent API
* 자바 진영의 ORM 표준 기술
* 자바를 이용해서 데이터를 관리(유지)하는 기법을 하나의 스펙으로 정리한 표준

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@Entity` |  |
| `@Table` |  |
| `@Id` |  |
| `@GeneratedValue` |  |
| `@Column` |  |
| `@Version` |  |
| `@MapperSuperclass` |  |
| `@EntityListeners` |  |
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
