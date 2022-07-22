# Class 10

## Significance


## Things I want to know more about



## Questions:

[Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a 'call'?

Generally a function call, which goes on the stack

2. How many 'calls' can happen at once?

Calls are processed one at a time.

3. WHat does LIFO mean?

Last In, First Out. The last call into the stack is the first one to pop out; an analogy to a stack is a stack of plates. The last one to be placed on top is the first one removed.

4. Draw an example of a call stack and the functions would need to be invoked to generate that call stack.

5. What causes a stack overflow?

When a function calls itself too many times it will eventually exceed the stack limit. This is an overflow condition. I did a simple recursive function with a print for testing and it always exceeded the max stack size at 997 iterations.

[JavaScript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a 'reference error'?

This happens when the program tries to access a variable that hasn't been declared yet.

2. What is a 'syntax error'?

This occurs when the code doesn't follow the rules of the language (the syntax), resulting in an invalid "meaning".

3. What is a 'range error'?

Occurrs when value passed is not allowed, e.g. invalid length for an Array constructor

4. What is a 'type error'?

Occurrs when actual type does not support attempted operation E.g. trying to assign a new value to a const or trying to use a method that doesn't exist on that object type throws a TypeError

5. What is a breakpoint?

Tells the debugger where to stop at so you can check the values at that point in execution.

6. What does the word 'debugger' do in your code?

Adds a breakpoint at that location. Depends on a debugger existing in whatever is executing the code, as it also invokes that debugger.

