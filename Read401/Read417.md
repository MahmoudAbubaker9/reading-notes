# Spring Authorization

### Spring Boot and OAuth2

There are several sample that build on each other, adding new features at every step:

1. Simple: A very basic static app with only a home page and unconditional login

2. Click: Adds an explicit link that the user has to click to log in.

3. Sign Out: Adds a sign out link for authenticated users as well.

4. Two Providers: Adds a second login provider so that the user can choose on the main page which one to use.

5. Custom Error: Adds an error message for unauthenticated users and custom authentication that depends on the GitHub API.

**Note:**

* Every application can be imported into the IDE.

* All applications run on localhost:8080 because they will use OAuth 2.0 clients registered with GitHub and Google for that address.

### How to login with single sign on github

1. Create a new project
2. Add a home page
3. Secure the application with GitHub and Spring Security to make the application secure.
4. Add a new GitHub app
5. Configure application.yml
6. Run the app

## Adding an Error Page for Unauthenticated Users

1. Switching to GitHub
2. Detecting an Authentication Failure in the Client
3. Adding an Error Message
4. Generating a 401 in the Server


For more details
[Resources](https://spring.io/guides/tutorials/spring-boot-oauth2/)
