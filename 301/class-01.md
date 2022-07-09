# Class 1

## Significance

    Component Based Architecture and Props flow are the fundamental design philosophy of React.

## Things I want to know more about

    I'm still not 100% on creating and using React components and using this weird hybrid syntax (jsx?).

## Questions:

    In systems thinking, a system is defined by its components, their interfaces, and functionality. The elements (components) of a system have stocks (states/properties) and flows (as in data). I like that this paradigm seems to follow good systems thinking principles. 

    Who wrote this Tutorials Point article? It contains so much over-elaborate, yet vague, language. For example, "Unit of composition" can be anything from a paragraph (writing) to a squad (military). They could have said "building block". "Depend on abstractions component do not depend on other concrete components, which increase difficulty in expendability" is barely even English. There are also tons of sentence fragments (missing subjects) and seems like they need to put down the thesaurus. There's no author listed; I wouldn't put my name on this either. 

    We probably should have talked (or at least read) about interfaces and abstract classes before this. I'm familiar from courses I've taken in the past, but I'm we haven't talked about this much at Code Fellows; it may confuse students.

### [Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

1. What is a "component"?

    A modular software object, organized logically or functionally, which encapsulates a related set of functionality. It provides an interface and behavioral expectations, making it easier to use, and can interact with other components. It is a basic building block, with clear preconditions and predictable behavior. Consists of Logic + Structures + Interface. Types include: UI, utility, JIT.

2. What are the characteristics of a component?

    Reusability, Replacability, Context Agnostic, Extensible, Encapsulated, Independant. All the basic elements of good OOP design.

3. What are the advantages of using component-based architecture?

    Reusing components increases development speed and reduces the chance of error. Component based systems are easier to maintain and deploy (due to independance and encapsulation), reduce reinventing the wheel, and are highly reusable.

### [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

1. What is "props" short for?

    Properties.

2. How are props used in React?

    A React component creates and returns an element. 
    
    Using jsx style syntax, attributes can be assigned to the component (e.g. "something="). The attribute *value* is placed within {} (similar to template literals; it's interpolation). 
    
    For example: `<SomeComponent anAttribute={aValue}>`. This attribute:value pair (or pairs) will be passed to the child object as an Object accessible via the `props` keyword with dot notation.

    React components are functions (or a Class with a `render()` method) that return React elements. Therefore, the props can be passed as an argument to the function.

3. What is the flow of props?

    One direction, read-only, from parent to child. The property attributes are assigned to the child component in the parent component, passed to the child component as an object argument.