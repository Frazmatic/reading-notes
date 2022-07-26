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