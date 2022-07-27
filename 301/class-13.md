# Class 13

## Significance

The essential function of web servers: providing access to resources.

## Things I want to know more about

Routers (in the api sense)

## Questions:

[CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

1. Which HTTP method would you use to update a record through an API?

PUT - Good for replacing values of a target entry.

2. Which REST methods require an ID parameter?

PUT & DELETE so that they know which record to modify.

[Speed Coding: Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

1. What's the relationship between REST and CRUD?

REST is an architectual *style*, a web server can handle CRUD *Operations* and do so with the RESTful style, making it more easily usable and reliable.

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

    1. Establish basic server dependencies such as Express
    2. Build file system / configurations
    3. Create routers
    4. Connect to database
    5. handle get/post/put/delete routes for all routers 

