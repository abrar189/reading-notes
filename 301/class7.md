# How I explained REST to my brother

1. Who is Roy Fielding?
That guy, Roy Fielding, he talks a lot about what those things point to in that research I was talking about. The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.

2. Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?

Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

3. What is the HTTP protocol that Fielding and his friends created?

HTTP—this protocol Fielding and his friends created—is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

4. What does a GET do?
GET is used to request data from a specified resource.
GET is one of the most common HTTP methods.
(/test/demo_form.php?name1=value1&name2=value2)

Some other notes on GET requests:

- GET requests can be cached
- GET requests remain in the browser history
- GET requests can be bookmarked
- GET requests should never be used when dealing with sensitive data
- GET requests have length restrictions
- GET requests are only used to request data (not modify)

5. What does a POST do?

POST is used to send data to a server to create/update a resource.
The data sent to the server with POST is stored in the request body of the HTTP request:

POST /test/demo_form.php HTTP/1.1
Host: w3schools.com
name1=value1&name2=value2

6. What does PUT do?

PUT is used to send data to a server to create/update a resource.

The difference between POST and PUT is that PUT requests are idempotent. That is, calling the same PUT request multiple times will always produce the same result. In contrast, calling a POST request repeatedly have side effects of creating the same resource multiple times.

7. What does PATCH do?

A patch is a set of changes to a computer program or its supporting data designed to update, fix, or improve it. This includes fixing security vulnerabilities and other bugs, with such patches usually being called bugfixes or bug fixes.

## Geocoding API

Did you get your API key?
yes pk.3cebfe468fd3afa08797e890fdbafaa3	