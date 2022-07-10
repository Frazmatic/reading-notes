# Class 3

## Significance

Controlled components ensure that our element state matches our React state, making them easier and more consistent to use within React. Ternary operators add a way of modifying elements 'on the fly' in a way that doesn't defeat the purpose of jsx (matching the html structural syntax) as much.

## Things I want to know more about

I would like to know more about how we will use the form component's state in React. For example, accessing it from another component.

## Questions:

### [React Docs - Forms](https://reactjs.org/docs/forms.html)

1. What is a 'Controlled Component'?

Input forms intrinsically have their own state (the values whish users can affect); however, if the form component controls the values with React, it is a "controlled component". This makes it so the React state is the only state.

2. Should we wait to store the user's responses from the form into state when they submit the form OR should we update the state with their responses as soon as we enter them? Why?

The component's state is updated as it is changed. This is so that the react state always matches the form state.

3. How do we target what the user is entering if we have an event handler on the an input field?

The event handler function receives an event object for that component, as an argument. `event.target.value` will have the value being entered by the user in that form component. We can use this.setState() to update that component's state with the changing value; however, since the event handler uses a call back function, the callback function must be bound to the component to access the component's `this`. 

### [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

1. Why should we use a ternary operator?

When we need to return or show something in an either/or situation, ternary operators are simple, single line way of doing so.

In React with jsx, we might use it to affect the struc returned element, causing it to render differently based on conditions.

This is an example from the text, returned from a component's render() method:

```
return (
    <div>
        The user is <strong>{isLoggedIn ? 'currently' : 'not'}</strong> logged in.
    </div>
)
```

In that example, the expression in curly braces is evaluated. If isLoggedIn is true, 'currently' is substituted for the curly brace expression. If not, 'not' is substituted. Then the element is returned with the appropriate word filled in. 

2. Rewrite the following statement using a ternary statement:
```
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

`x === y ? console.log(true) : console.log(false);`