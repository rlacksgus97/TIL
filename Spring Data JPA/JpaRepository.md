## @Entity

- 객체를 Entity로 선언
- PK가 필요
    - @Id : PK로 저장
    - @GeneratedValue : 순차적으로 번호 증가

## JpaRepository

```java
public interface UserRepository extends JpaRepository<User, Long>{
}
```

save()

- 저장

findAll()

- 전체 조회
- 전체를 조회하기 때문에 성능 이슈 발생 가능

flush()

- 현재 Jpa 컨텍스트에서 갖고 있는 DB 값을 DB에 반영하도록 지시

## PagingAndSortingRepository

## CrudRepository

## getOne() vs findById()

- getOne() : Lazy Fetch
- findById() : Eager Fetch
