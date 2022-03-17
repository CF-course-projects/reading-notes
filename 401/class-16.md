# Spring Authentication

## Spring Security Overview

### Authentication and Access Control
- Applications security boils down to two problems:
  - Authentication: who are you?
  - Authorization: what are you allowed to do?
- Authentication
  - The main strategy for authenticaiton is AuthenticationManager, which has only one method
    - An authentication manager can do one of 3 thigns in its authenticate method
      - return an authentication to verify if the input represents a valid principal
      - throw an authentication error if it believes that the input represents an invalid principal.
      - return null if it cannot decide
- Web Security
  - Spring Security is based on Servlet filters

### Spring Auth Cheat Sheet

- Step 1: set up a user model and repo
- Step 2: Create a controller for that model
- Step 3: UserDetailsServiceImpl implements UserDetailsService
  - gets a User from the database by username (make sure your repository has the method to make this easy!)
- Step 4: ApplicationUser implements UserDetails
  - use IntelliJ to implement the methods; make the boolean ones all return true
- Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
- Step 6: registration page
  - Create it w/ a form
  - ensure it posts a route your controller is ready to handle
  - ensure it saves in DB
- Step 7: login page
  - create it w/ form
  - ensure it posts to the route you specified in the web config
  - pass data via attributes to the templates w/ data from principal p
