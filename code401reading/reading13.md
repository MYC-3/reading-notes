# Related Resources and Integration Testing

## Spring Data Rest

[Notes taken from this site](https://www.baeldung.com/spring-data-rest-relationships)

- *Library* and *Address* have a one-to-one relationship.
- The @RestResource annotation is optional and can be used to customize the endpoint.
- Be careful to have different names for each association resource.
- Before creating an association, sending a GET request to this endpoint will return an empty object.
- A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.
- A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.

## Integration Testing

[Notes taken from this site](https://www.baeldung.com/integration-testing-in-spring)

- Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.
- Dependencies: junit-jupiter-engine, junit-jupiter-api, and Spring test.

>We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.

>We also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.

- Code Example:

```Java
@ExtendWith(SpringExtension.class)
@ContextConfiguration(classes = { ApplicationConfig.class })
@WebAppConfiguration
public class GreetControllerIntegrationTest {
    ....
}
```

- 

[Back to HOME](../README.md)