# Spring Security Architecture

Spring security is framework used for securing Spring applications. It stands between client and application and gives possibility of configuring what data and functionalities are exposed to which users

### Authentication and Access Control

1. Authentication : is any process by which a system verifies the identity of a user who wishes to access the system.

```
An AuthenticationManager can do one of 3 things in its authenticate() method:

1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

2. Throw an AuthenticationException if it believes that the input represents an invalid principal.

3. Return null if it cannot decide.
```
2. Access control mechanisms determine which operations the user can or cannot do by comparing the user's identity to an access control list (ACL).

**Access controls encompass:**
1. File permissions, such as the right to create, read, edit or delete a file.
2. Program permissions, such as the right to execute a program.
3. Data permissions, such as the right to retrieve or update information in a database.

### Web Security

the protective measures and protocols that organizations adopt to protect the organization from, cyber criminals and threats that use the web channel.

**The typical layering of the handlers for a single HTTP request:**

1. The client sends a request to the application, and the container decides which filters and which servlet apply to it based on the path of the request URI.

2. At most, one servlet can handle a single request, but filters form a chain, so they are ordered.

3. The order of the filter chain is very important, and Spring Boot manages it through two mechanisms: @Beans of type Filter can have an @Order or implement Ordered, and they can be part of a FilterRegistrationBean that itself has an order as part of its API.

4. In a Spring Boot application, the security filter is a @Bean in the ApplicationContext, and it is installed by default so that it is applied to every request.

### Method Security

1. Method-level security is implemented by placing the @PreAuthorize annotation on controller methods (actually one of a set of annotations available, but the most commonly used).

2. This annotation contains a Spring Expression Language (SpEL) snippet that is assessed to determine if the request should be authenticated

```
@EnableGlobalMethodSecurity(securedEnabled = true)
public class SampleSecureApplication {
}

then :

public class MyService {

  @Secured("ROLE_USER")
  public String secure() {
    return "Hello Security";
  }

}
```

### Working with Threads

If you need access to the currently authenticated user in a web endpoint, you can use a method parameter in a @RequestMapping


Resource Site :

[Spring Security overview](https://spring.io/guides/topicals/spring-security-architecture/)
[Spring Auth cheat sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)