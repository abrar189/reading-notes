# Spring Boot and OAuth2

It starts with a simple, single-provider single-sign on, and works up to a client with a choice of authentication providers: GitHub or Google.

The samples are all single-page apps using Spring Boot and Spring Security on the back end. They also all use plain jQuery on the front end. But, the changes needed to convert to a different JavaScript framework or to use server-side rendering would be minimal.

All samples are implemented using the native OAuth 2.0 support in Spring Boot.

There are several samples building on each other, adding new features at each step:

- simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

- click: adds an explicit link that the user has to click to login.

- logout: adds a logout link as well for authenticated users.

- two-providers: adds a second login provider so the user can choose on the home page which one to use.

- custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.

Each app can be imported into an IDE. You can run the main method in SocialApplication to start an app. They all come up with a home page on http://localhost:8080 (and all require that you have at least a GitHub and Google account if you want to log in and see the content).

You can also run all the apps on the command line using mvn spring-boot:run or by building the jar file and running it with mvn package and java -jar target/*.jar (per the Spring Boot docs and other available documentation). There is no need to install Maven if you use the wrapper at the top level, e.g.

$ cd simple
$ ../mvnw package
$ java -jar target/*.jar

## Single Sign On With GitHub

1. Creating a New Project
First, you need to create a Spring Boot application, which can be done in a number of ways. The easiest is to go to https://start.spring.io and generate an empty project (choosing the "Web" dependency as a starting point). Equivalently, do this on the command line:

$ mkdir ui && cd ui
$ curl https://start.spring.io/starter.tgz -d style=web -d name=simple | tar -xzvf -

2. Add a Home Page
In your new project, create index.html in the src/main/resources/static folder. You should add some stylesheets and JavaScript links so the result looks like this:

index.html
< !doctype html>
 < html lang="en">
< head >
    < meta charset="utf-8"/>
    < meta http-equiv="X-UA-Compatible" content="IE=edge"/>
    < title>Demo</title>
    < meta name="description" content=""/>
    < meta name="viewport" content="width=device-width"/>
    < base href="/"/>
    < link rel="stylesheet" type="text/css" href="/webjars/bootstrap/css/bootstrap.min.css"/>
    < script type="text/javascript" src="/webjars/jquery/jquery.min.js"></script>
    < script type="text/javascript" src="/webjars/bootstrap/js/bootstrap.min.js">< /script>
< /head>
<  body>
	<h1>Demo</h1>
	<div class="container"></div>
< /body>
< /html>

3. Securing the Application with GitHub and Spring Security
To make the application secure, you can simply add Spring Security as a dependency. Since you’re wanting to do a "social" login (delegate to GitHub), you should include the Spring Security OAuth 2.0 Client starter:

pom.xml
< ependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-oauth2-client</artifactId>
< /dependency>

# you can learn more and more by visite [Spring Boot and OAuth2](https://spring.io/guides/tutorials/spring-boot-oauth2/)
