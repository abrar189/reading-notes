# API Design Best Practices

1. What does REST stand for?

REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP

2. REST APIs are designed around a resources.

3. What is an identifer of a resource? Give an example.

 a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: https://adventure-works.com/orders/1

4. What are the most common HTTP verbs?
The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently.

5. What should the URIs be based on?
URIs should be based on nouns

6. Give an example of a good URI.
https://eu1.locationiq.com/v1/search.php?key=YOUR_ACCESS_TOKEN&q=SEARCH_STRING&format=json

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
A web API that have more requests, which is bad as it lower the performance.

8. What status code does a successful GET request return?
A successful GET method typically returns HTTP status code 200 (OK).

9. What status code does an unsuccessful GET request return?
If the resource cannot be found, the method should return 404 (Not Found).

10. What status code does a successful POST request return?
If a POST method creates a new resource, it returns HTTP status code 201 (Created).

11. What status code does a successful DELETE request return?
indicating that the process has been successfully handled, but that the response body contains no further information.