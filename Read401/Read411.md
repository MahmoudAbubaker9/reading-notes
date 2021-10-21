# Spring

### Serving Web Content with Spring MVC

A Spring MVC is a Java framework which is used to build web applications. It follows the Model-View-Controller design pattern. It implements all the basic features of a core spring framework like Inversion of Control, Dependency Injection.

**Create a Web Controller**

@Controller : used for marks a class as Controller and for handling the HTTP requests(controls the flow of the data).

GetMapping : used to map the class with the specified URL name. It ensures the specific HTTP GET requests are maped to specific method.

@RequestParam : used to read the form data and bind it automatically to the parameter present in the provided method.

**Run the Application**

@SpringBootApplication : it is convenience annotation that use to auto-configuration, component scan and be able to define extra configuration on application class.

@EnableAutoConfiguration : Tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.

@Configuration : allow to register extra beans in the context or import additional configuration classes

### Spring MVC and Thymeleaf

Thymeleaf is a Java library . It is template engine for processing and creating HTML, XML, JavaScript, CSS, and text.

**Spring model attributes**

The @ModelAttribute is an annotation that binds a method parameter or method return value to a named model attribute and then exposes it to a web view.

**Session attributes**

The @SessionAttributes annotation is used to store the model attribute in the session


For more information :

[Spring App Basics](https://spring.io/guides/gs/serving-web-content/)

[Spring MVC and Thymeleaf](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)
