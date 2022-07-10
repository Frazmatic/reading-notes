# Class 5

## Significance

Use of these concepts results in readable, maintainable, design with functionality broken down into basic parts. This facilitates implementing the desired behavior.

## Things I want to know more about

The principles for decomposition and identifying heirarchy, state, and where state should exist, seem to follow good general OOP design principles. I'd like to know more about applying this in other frameworks. 

I've written higher order functions in Python. For example, I created GameBoard object that needed a search() method for GamePiece objects. I needed a way to compare and look through these new classes, so my search method took a function as argument. Then I created functions for each object which compared them, and return an appropiate value for the search method to use. Doing it this way, I was also able to write functions for comparing different classes, which I would not have been able to do if each type only had its own comparison method.

## Questions:

### [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

1. What is the "single responsibility principle" and how does it apply to components?

The basic idea fo the single responsibility principle is that a function, or component, should only do one thing. One way to break things down is using the "information architecture"; that is, the type of data each thing represents. Look at what each part represents, and break it down into the smallest discrete concepts that make sense. 

In the example, they have concepts such as category, individual products, the table of products which contains the categories as well as the individual products), the search bar, and the filterable (searchable) table as a whole that combines the products table with the search bar. They broke it down into five basic ideas, from which they can make five components.

As you can see, some of the component types make sense as "part" ('has a' relationship) of the other components. This is a heirarchical relationship, identifying which comonents are "children" of other components.

2. What does it mean to build a 'static' version of your application?

A static version of a site is stateless and non-interactive. It defines the basic structure of the application without needing to think too much about the behavior and logic.

In react, the only methods that components will have are their render() methods. This is because the static version only needs the elements to display, it doesn't need to manipulate data.

It will use props to pass data to child elements so that their elements are created correctly.

3. Once you have a static application, what do you need to add?

To turn it into an interatice, dynamic, app, state must be added.

The types of data that actually needs to be mutable, and not just computed (i.e. calculated with a method) needs to be considered. The following questions can help decide which of this data needs to be state. 

4. What are the three questions you can ask to determine if something is state?

  1. Is passed from parent via props? Since props is used for one directional data that isn't supposed to be changed, it's probably not state if it's in props.
  2. Does it remain unchanged over time? If it doesn't need to be mutated by the application, it's probably not state.
  3. Can you compute it based on other state or props in the component? If it can be calculated on the fly, it probably doesn't need to be its own state property.

5. How can you identify where state needs to live?

Look at what all components need the state. Find the lowest component in the heirachy that contains all those components. This is similar to a 'lowest common denominator' idea. That component (or one higher up, if necessary) should own the state.

If none make sense, create container component at a high enough level in the heirachy for the purpose of owning the state.

In the example, ProductTable needs the state from SearchBar. Both are children of FilterableProductTable, so the state lives there and is passed as props to those child components.

To modify the state in FilterableProductTable, it can pass a callback function to SearchBar via props. The callback function will use FilterableProductTables' setState() method. Then Searchbar can implement an onChange event handler using that callback function to modify FilterableProductTable's state.

### [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

1. What is a "higher-order function"?

A higher-order function takes a function as an argument and/or returns a function. It's a function that works on functions.

2. Explore the greaterThan() function as defined in the reading. In your own words, what is line 2 of this function doing?

The greaterThan function creates (returns) a function. Line 2 returns a function using arrow function syntax. It is equivalent to `return function(m){return m > n}`. n is the argument to greaterThan. 

In line 2, whatever is passed as n is substituted in the new function, then returned as a function which takes m as an argument and compared it to the subtituted n. 

For example, calling greaterThan with the argument '10' returns a function equivalent to `function(m){return m > 10}`, which will return true if the argument is greater than 10.

3. Explain how either map() or reduce() operates, with regards to higher-order functions.

Map and reduce are methods for arrays which both *take* functions as arguments. They are higher-order functions because they both use a function as their argument, changing their behavior based on the function received.

Map takes the function recieved as input, and applies to each element in the array sequentially. Each element in the array is passed as an argument to the received function, and the return value of the received function as pushed to a new array.

Similarly, reduce takes a function and applies it to all the elements in the array to produce a single value representing (summarizing) the array. The function received tells it how to combine each value with the prior value produced. For example, if given a function that takes two arguments and returns their sum, it's equivalent to looping through the array and peformaing a += with all the array's elements.

By using higher-order functions, these functions can be more simlpy combined (composed) with other functions, such as calling reduce in a function that returns a function to map, to modify a data set based on a query dependant on that data set.