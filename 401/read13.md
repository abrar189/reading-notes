# Working with Relationships in Spring Data REST

1. Overview
how to work with relationships between entities in Spring Data REST. association resources that Spring Data REST exposes for a repository

2. One-to-One Relationship

- The Data Model:

- The @RestResource annotation is optional and can be used to customize the endpoint.
- We must be careful to have different names for each association resource.
- The association name defaults to the property name and can be customized using the rel attribute of @RestResource annotation
- If we were to add the secondaryAddress property above to the Library class, we would have two resources named address, and we would encounter a conflict.

@JoinColumn(name = "secondary_address_id")
@RestResource(path = "libraryAddress", rel="address")
private Address secondaryAddress;

- The Repositories:

- In order to expose these entities as resources, let's create two repository interfaces for each of them, by extending the CrudRepository interface: public interface LibraryRepository extends CrudRepository<Library, Long> {} public interface AddressRepository extends CrudRepository<Address, Long> {}

- Creating the Resources:

- Note that if you're using curl on Windows, you have to escape the double-quote character inside the String that represents the JSON body: -d "{\"name\":\"My Library\"}"

- Creating the Associations:

- After persisting both instances, we can establish the relationship by using one of the association resources.
- This is done using the HTTP method PUT

3. One-to-Many Relationship

- A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.

4. Many-to-Many Relationship

- A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.

# Baeldung: Spring Integration Testing

## Enable Spring in Tests with JUnit 5

JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.

We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.

We also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.

@ExtendWith(SpringExtension.class)
@ContextConfiguration(classes = { ApplicationConfig.class })
@WebAppConfiguration
public class GreetControllerIntegrationTest {
    ....
}

We use a Java configuration class here to specify the context configuration. Similarly, we can use the XML-based configuration:

@ContextConfiguration(locations={""})

Finally, we also annotate the test with @WebAppConfiguration, which will load the web application context.

By default, it looks for the root web application at path src/main/webapp. We can override this location by simply passing the value attribute:

@WebAppConfiguration(value = "")

## The WebApplicationContext Object

WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.

We'll now be able to wire the web application context right into the test:

@Autowired
private WebApplicationContext webApplicationContext;

## Mocking Web Context Beans

MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

Let's see how to use it:

private MockMvc mockMvc;
@BeforeEach
public void setup() throws Exception {
    this.mockMvc = MockMvcBuilders.webAppContextSetup(this.webApplicationContext).build();
}