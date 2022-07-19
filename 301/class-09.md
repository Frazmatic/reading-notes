# Class 9

## Significance

Functional programming is a useful paradigm for modelling many types of problem domains.



## Things I want to know more about



## Questions:

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

I'm out of my two free Medium articles, and when I viewing in incognito mode all of the exmaple code was missing, making the article difficult to understand. For instance:

![Screenshot of the Medium article](./MediumArticle.png)


I used this instead: https://opensource.com/article/17/6/functional-javascript

1. What is functional programming?

Functional programming depends on using and composing pure functions, values are obtained by evaluating expressions (i.e. looking at the return of a function) rather than assigning/changing them in "state".  Values are "mapped" to each other with functions, just like in math class: "f(g) -> y".

2. What is a pure function and how do we know if something is a pure function?

A pure function must always have the same result for the same input. This is called referential transparency. It must not change anything outside of the function; e.g. it shouldn't change values inside an object or variable passed to it, or send any data anywhere except the return value of the function. That is, it should not have "side effects".

Pure functions are more like the functions we learn in math class.

3. What are the benefits of a pure function?

I learned this from experience: debugging is easier! You only need to worry about the input producing the correct output. You don't need to worry about a bunch of changing state conditions adding complexity and making it hard to troubleshoot, or giving you weird results because something else changed. Similarly, building a program by composing pure functions is easier; you just do one particular, discrete, thing at a time.

Testing: Related to above, if you have predictable results (expected value for given input) without worry about a bunch of environmental variables, you can more easily and effectively write tests.

Memoization: I've done this in Python. Input values can be saved as keys in a hashable data structure (e.g. Object, Map, Dictionary). The return values can be stored as each key's value. This can be checked before running the function to avoid running it again if the value has already been computed.

4. What is immutability?

Immutable data structures can't have their values changed. For example, you can't change a character in a string without making a new string. If using an object in an immutable way you would always create a new instance of that object type instead of modifying the object directly.

5. What is Referential transparency?

It means you could replace the expression with its resulting value and it wouldn't change the program. Because it always returns the same value for the same input (no state changes / side effects), we can use the expected values. This allows for the memoization I mentioned before.

[Node JS Tutorial - Modules and Require](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?



2. What does the word ‘require’ do?
3. How do we bring another module into the file the we are working in?
4. What do we have to do to make a module available?


