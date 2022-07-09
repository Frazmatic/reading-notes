# Class 2

## Significance

Props and state are how React handles data within and between components.

## Things I want to know more about

Exactly when does props get seen by a component? 

## Questions:

### [React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. Based off the diagram, what happens first, the 'render' or the 'componentDidMount'?

    `render` occurs before `componentDidMount` in the Mountaing phase.

2. What is the very first thing to happen in the lifecycle of React?

    The first phase is Mounting, which initially calls the `constructor` to create the component instance.

3. Put the following things in the order they happen:
    1. `componentDidMount`
    2. `render`
    3. `constructor`
    4. `componentWillUnmount`
    5. `React Updates`

    I. `constructor`. II. `render`. III. `componentDidMount`. IV. `React Updates`. V. `componentWillUnmount`.

4. What does `componentDidMount` do?

    It's called automatically after the component mounts succesfully. It's a good place for network requests.

### [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

1. What types of things can you pass in the props?

    Information for the component to use (without being changed) by component. For example, text to be displayed in an element can be passed to the component.

2. What is the big difference between props and state?

    State is handled inside a component. It can be changed inside the component. Props are handled outside the component and *passed* to the component. Props must be changed outside the component.

3. When do we re-render our application?

    When the state is changed inside a component. When the component needs to be recreated with new props.

4. What are some examples of things we could store in state?

    Anything requiring the internal (to the component) changes to the data, i.e. things the component needs to update. For example, form data, counters. 