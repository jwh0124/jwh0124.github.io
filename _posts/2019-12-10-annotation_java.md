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

## Used Java Annotation ##

### Lombok ###

> 멤버 변수에 대한 Getter/Setter Method, Equals(), hashCode(), toString() 과 멤버 변수에 값을 설정하는 생성자 등을 자동으로 생성해주는 라이브러리

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@Data` | @Getter, @Setter, @ToString, @EqualsAndHashCode 등 자동 생성 |
| `@Builder` | Builder API 처럼 사용할 수 있도록 지원 |
| `@AllArgsConstructor` | 모든 인자를 가진 생성자를 생성 |
| `@NoArgsConstructor` | 인자 없는 생성자를 생성 |
| `@Slf4j` | Simple Logging Facade For JAVA ,로깅에 대한 인터페이스 모음 |
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
| `@OneToOne` | 1:1 Relationship Annotation |
| `@OneToMany` | 1:N Relationship Annotation |
| `@ManyToOne` | N:1 Relationship Annotation |
| `@ManyToMany` | M:N Relationship Annotation |
| `@JoinColumn` | Foreign key Mapping Annotation |
| `@Temporal` | 날짜 타입(Date, Calendar) Mapping 시 사용 |

### Spring-Web ###

> Web Application 개발에 필요한 Web Application Context와 Multipart Request등의 기능을 지원

| Annotation | Description |
| :--- | :--------------------------------------------------------- |
| `@RestController` | @Controller 와 @ResponseBody를 합쳐놓은 Annotation |
| `@RequestMapping` | 요청에 대해 어떤 Controller, 어떤 메소드가 처리할지를 맵핑하기 위한 Annotation |
| `@GetMapping` | @RequestMapping(method = RequestMethod.GET) 의 축약형 |
| `@PostMapping` | @RequestMapping(method = RequestMethod.POST) 의 축약형 |
| `@PutMapping` | @RequestMapping(method = RequestMethod.PUT) 의 축약형 |
| `@DeleteMapping` | @RequestMapping(method = RequestMethod.DELETE) 의 축약형 |
| `@ExceptionHandler` | Controller 기반 Exception Handle 시 사용하는 Annotation |
| `@RestControllerAdvice` | 예외 발생 시 json형태로 결과를 Return 하는 Annotation |

### Spring-context ###

| Annotation | Description |
| :--- | :--------------------------------------------------- |
| `@Configuration` | 클래스가 JavaConfig용 클래스임을 컴파일러에 알리는 Annotation |
| `@Bean` | DI 컨테이너가 관리할 Bean을 생성하는 메서드, 메서드 이름이 Bean 이름 |
| `@Import` | JavaConfig를 읽어들이기 위한 Annotation으로 @Configuration 이 붙은 클래스를 지정 |
| `@Controller` | 웹 MVC 프레임워크인 스프링 MVC의 컨트롤러를 나타내는 Annotation |
| `@Service` | Service Class 를 나타내는 Annotation |
| `@Repository` | Repository class를 나타내는 Annotation |
| `@Validated` | 폼에서 입력되어 들어온 값을 검사 |

### Spring Boot ###

> 실행만 하면 스프링 기반의 상용화가 가능한 애플리케이션을 쉽게 만들 수 있도록 만든 스프링 프레임워크.

| Annotation | Description |
| :--- | :---------------------------------------------------- |
| `@EnableAutoConfiguration` | 다양한 설정이 자동으로 수행되고 기존의 스프링 애플리케이션에 필요했던 설정 파일들이 필요 없게 되는 Annotation |

### Spring Beens ###

| Annotation | Description |
| :--- | :----------------------------------------|
| `@Autowired` | DI Container 가 주입해야 할 필드를 의미하는 Annotation |

### Javax ###

| Annotation | Description |
| :--- | :----------------------------------------|
| `@NotNull` | 입력 값을 검사하기 위한 Annotation, 필수 요소 |
| `@Size` | 길이를 제한 하는 Annotation |

### Spring-cores ###

| Annotation | Description |
| :--- | :----------------------------------------|
| `@Order` | 입력 값을 검사하기 위한 Annotation, 필수 요소 |
