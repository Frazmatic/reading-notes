# Class 3

## Significance



## Things I want to know more about

The spread operator sounds like the unpacking operator in Python.

## Questions:

### [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

1. What does .map() return?

    A new array, where each element in the array is the returned value from the function passed to map(), with each element in the original array given as an argument to the given function.

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

    Utilize map. The function passed to map() should return an element for for each item in the array. 

    The syntax for this would be like `theNewElementArray = oldArray.map(item => <tag>{item}</tag>);`. 

    This can be done within a component function. The old array can be passed as props to the component function. The new array can be placed inside an element and returned. for example, an array of `<li>` elements could be placed inside a `<ul>` and returns, like `return <ul>{theNewElement}</ul>`.

    Now that it's a proper React component,  the component can be passed as an argument to a component's (such as root's) render method.

3. Each list item needs a unique ___.

    Key. A string identifier for every element in a list of elements. They are given as attributes (like props).

4. What is the purpose of a key?

    React uses keys unique to items in individual lists to track changes to the list, such as adding or removing items.
    

### [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

1. What is the spread operator?

It breaks up an array into its individual elements.

2. List 4 things the spread operator can do.

Pass an array as a series of indivdual arguments to a function.

Combinee arrays, or adding items to an array

Add to state in React

Combine objects

Convert a NodeList to an Array

3. Give an example of using the spread operator to combine two arrays.

`[..array1, ...array2]`

4. Give an example of using the spread operator to add a new item to an array.

`arra1 = [...array1, newItem];`

5. Give an example of using the spread operator to combine two objects into one.

`{...object1, ...object2}`
`{object1, ...object2, newKey: newValueOrFunction}`

### [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

1. In the video, what is the first step the developer does to pass functions between components?

Create a function within the parent, so that is has the same scope as the state he wishes to modify.

2. In your own words, what does the increment function do?

There is an array called 'people' in the App component's state (the app component is a class component). The increment function he wrote takes a name as argument. It maps the original people array into a new array. It looks through the people array for an object with a 'name' property that matches that name. It modifies that object's 'count' property by incrementing it by one.

It then calls setState on the App component. The argument, using curly braces to embed key value pair to be changed, is the people property with the value set to the newly created array.

3. How can you pass a method from a parent component into a child component?

Pass it in props as key value pair. The value is the function in the parent app. It can now be accessed via dot notation on props in the child component.

4. How does the child component invoke a method that was passed to it from a parent component?

Using its props, since it was passed as props. e.g. `this.props.thePassedFunction()`. It can be assigned to or used within one of the component's methods.