# Class 7

## Significance

This describes the ideas of REST architecture and use of HTTP to exchange representations of resources on the internet.

## Things I want to know more about

"I couldn't use the word "get" universally, but instead had to think up a new word for each verb/noun combination. "shmet the bottle", "mandle the magazine", "zorp the book""

Some of English does work like that ('eat the food' vs 'drink the water') and some spoken languages work more like that, heh.

## Questions:

### [How I explained REST to my brother](https://gist.github.com/brookr/5977550)

1. Who is Roy Fielding?

  One of the main people who helped create HTTP.

2. Why don't the techniques that we use today work well when we need to be able to talk to all of the machines in the world?

  They weren't designed to communicate with a potentially massive number of systems accross a massive network.

3. What is the HTTP protocol that Fielding and his friends created?

  A protocol that allows machines to make requests for resources via a network, and uses URLs to provide "location" data for the resources.

4. What does a `GET` do?

  *Requests* a resource from a web server.

5. What does a `POST` do?

  (Tries to) *Add* a resource to a web server.

6. What does `PUT` do?

  For *replacing* something in another system

7. What does `PATCH` do

  For *modifying/updating* something in another system.