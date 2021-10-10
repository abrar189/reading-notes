# Spring

The Spring Framework is an application framework and inversion of control container for the Java platform. The framework's core features can be used by any Java application, but there are extensions for building web applications.

## Spring model attributes :

- SMVCpring calls the pieces of data that can be accessed during the execution of views model attributes.

- There are several ways of adding model attributes to a view in Spring MVC.

- Below you will find some common cases:

1. Add attribute to Model via its addAttribute method
2. Return ModelAndView with model attributes included
3. Expose common attributes via methods annotated with @ModelAttribute.

// Example
    @RequestMapping(value = "message", method = RequestMethod.GET)
        public String messages(Model model) {
            model.addAttribute("messages", messageRepository.findAll());
            return "message/list";
        }


## Request parameters

Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server like:

https://example.com/query?q=Thymeleaf+Is+Great!


## Session attributes

- Similarly to the request parameters, session attributes can be accessed by using the session. prefix
- Or by using #session, that gives you direct access to the javax.servlet.http.HttpSession object: ${#session.getAttribute('mySessionAttribute')}

    @RequestMapping({"/"})
        String index(HttpSession session) {
            session.setAttribute("mySessionAttribute", "someValue");
            return "index";
        }


## ServletContext attributes

The ServletContext attributes are shared between requests and sessions. In order to access ServletContext attributes in Thymeleaf you can use the #servletContext. prefix

## Spring beans

Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax

< div th:text="${@urlService.getApplicationUrl()}">...< /div >

