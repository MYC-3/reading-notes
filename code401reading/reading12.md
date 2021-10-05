# Spring RESTful Routing & Static Files

## Request Mapping
[Notes taken from this site](https://www.baeldung.com/spring-requestmapping)

- `@RequestMapping` example:
```Java
@RequestMapping(value = "/ex/foos", method = RequestMethod.GET)
@ResponseBody
public String getFoosBySimplePath() {
    return "Get some Foos";
}
```

- Request mapping is used to map web requests to Spring Controller Methods.

## Accessing Data with JPA
[Notes taken from this site](https://spring.io/guides/gs/accessing-data-jpa/)

- Spring Initializr:
    1. Dependencies = Spring Data JPA and H2 Database
    2. Generate

- Two constructors. One is just for JPA so it is protected. The other is to store objects in the database.

## Spring Data Repositories
[Notes taken from this site](https://www.baeldung.com/spring-data-repositories)

- JpaRepository extends:
- PagingAndSortingRepository which extends:
- CrudRepository.
- Downsides = Be careful not to expose internal implementations and using the *CrudRepository* it exposes a complete set of persistent methods at once.

[Back to HOME](../README.md)