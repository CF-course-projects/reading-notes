# Related Resources and Integration Testing

### Integration Testing in Spring

1. Prep
- Dependencies:
  - We need sveral Maven dependencies for running integration tests
    - junit jupiter engine
    - junit jupiter api
    - Spring test

2. Spring MVC Test Configuration
- Enalble Spring in Test with JUnit 5
  - add the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class
  - we'll also need the @ContextConfiguration annotation to lead the context configuration and bootstrap the context that the test will use
    - within the params of ContextConfiguration(classes = {ApplicationConfig.class}) we include the thte config class which loads the config we need for the class.
  - The WebApplicationContextObject
    - The WebApplicationContextObject provides a web application configuration

3. Writing Integration Tests:
- Verify View Name
  - We can invoke the /homePage endpoint from our test as: http://localhost:8080/spring-mvc-test/
  - the perform method will call a GET request method which returns the ResultActions
  - .andDo(print()) will print the response
  - .andExpect() will expect the provided argument
- Verify Response Body
  - andExpect(MockMvcResultMatcherd.status()isOk()) verifies that the response HTTP status is ok (200)
  - andExpect(MOckMvcResultMatchers.jsonPath"$.message").value("Hello World")) will verify that the response content matches with the argument "Hello World" Here we used jsonPath, which extracts the response content and provides te request value
- Sending GET Request with Path Var
  - We invoke the GET request request with a path var as: http://localhost:8080/spring-mvc-test/greetWithPathVariable/John

4. MockMvc Limitations
- We cannot test the whole network stack while using MockMvc
- Bc Spring prepares a fake web app context to mock the HTTP requests and responses, it may not support all hte fratures of a full-blown Spring applicaton


