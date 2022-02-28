# Spring

## Serving Web Content with Spring MVC

- Creating a web controller 
  - In Spring's approach to building web sites, HTTP requests are handled by a controller.
  - You can tell a controller by the @Controller annotation
  - The @GetMapping annotation links the HTTP GET requests to the specified route are mapped to the greeting method.
  - @RequestParam binds the query string param to the callback param
  - Thymeleaf performs server-side rendering of html
    - Make sure to have Thymeleaf on your classpath
    - org.springframework.boot:spring-boot-starter-thymeleaf
  - Building an executable JAR file
    - You can run the app from the command line with Gradle or Maven
    - Building an executable app as a JAR file will contain all the necessary dependencies, classes, and resources to run the app properly.
    - You can build the JAR file by using ./gradlew build
    - Add a home page:
      - Staic resources, like HTML, CSS, and JS are served from your Spring Boot app.
      - You need to create a file at src/main/resources/static/index.html

## Spring MVC and Thymeleaf: how to access data from templates
- In Spring MVC, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered. The model map allows for the webpage to be abstacted into a Thymeleaf context object. <br>
1. Spring model attributes
  - Spring MVC calls the pieces of data that can be accessed during the execution of views 'model attributes'. There are several ways to add attributes to a view in Spring MVC:
    - Add attribute to model via addAttribute method
    - Return ModelAndView with model attributes included
    - Expose common attributes via methods annothed with @ModelAttribute

2. Request Params
- In order to access params, use the <b>param</b> prefix
  - Ex. String paramVal = param.someParamName
  - Note: If you access a multivalued param you will get a serialized/hydrated array as a value.
3. Session attributes
  - Use the session prefix to add session attributes
4. ServletContext attributes
  - SerlvetContext attributes are shared between requests and session.
  - To access them, use the #servletContext prefix.


