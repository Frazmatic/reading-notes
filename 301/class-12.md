# Class 12

## Significance

These subjects are part of proper API design.

## Things I want to know more about

RESTful design patterns

## Questions:

[Status Codes Based on Rest Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

1. In your own words, describe what each group of status codes represents:

    - 100s = literally 'status', information about the HTTP request.
    - 200s = Success, but not necessarily completion
    - 300s = rediction (new location for resource)
    - 400s = Something's wrong! Errors (client side).
    - 500s = Something's wrong! Errors (server Side)

2. What is a status code of 202?

async processing, i.e. 'in process'. 

3. What is a status code of 308?

permanent relocation, client should start using new URL

4. What code would you use if an update didn't return data to a client?

204 (no content)

5. What code would you use if a resource used to exist but no longer does?

410 (Gone)

6. What is the 'Forbidden' status code? 

Client authorized but does not have permissions for that particular resource.

[Build A REST API With Node.js, Express, & MongoDB - Quick ](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

So that others can't see it when the code is hosted publicly.

2. What is middleware?

Code that runs when the server gets a request but before it passed to a route.

3. What does `app.use(express.json())` do?

App .use uses 'middleware', in this case express.json() which allows interpretation of JSON, for exmaple, in the body of a post request.

4. What does the `/:id` mean in a route?

It identifies 'id' as a parameter on that route.

5. What is the difference between `PUT` and and `PATCH`?

Patch is a partial update, allowing to change only select fields

6. How do you make a default value in a schema?

In the value object part of the schema defintion (paired with the field name, where type, required, etc are), include the `default: <value>` kv pair where value is the default value for that field.

7. What does a 500 error status code mean?

Server side error

8. What is the difference between a status 200 and a status 201?

201 more specifically means that something was created.