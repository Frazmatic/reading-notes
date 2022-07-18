# Class 8

## Significance



## Things I want to know more about



## Questions:

[API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. What does REST stand for?

Representational State Transfer

2. REST APIs are designs around a ___.

Resources (a.k.a. data, services, objects)

3. What is an indentifier of a resource? Give an example. The example in this article is "https://adventure-works.com/orders/1"; a hypothetical URI for an individual order.

A URI, the web address for the resource. 

4. What the most common HTTP verbs?

"GET, POST, PUT, PATCH, and DELETE" for retrieving, sending, replacing, updating, and removing respectively.

5. What should the URIs be based on?

URIs should be based on resources, not operations. On the nouns, not the verbs. A URI identifies the location of a resource, then different types of requests (the verbs) are applied to it.

6. Give an example of a good URI.

The text identifies "https://adventure-works.com/orders" as a good example of a URI, because it identifies a particular type of resource (based on the business entity it represents; orders). A client could get orders from or post orders to this URI. 

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

If resources are divided up into many small parts, they will require a large number of requests to obtain them all. This will put a high load of requests on the web server, which is bad.

8. What status code does a successful GET request return?

200

9. What status code does an unsuccessful GET request return?

404

10.   What status code does a successful POST request return?

201

11. What status code does a successful DELETE request return?

204
