# Class 10 Notes

## Why This Matters

        A large part of programming is troubleshooting/debugging. Programs can be very complicated, with many interacting parts. 
        
        If you write 10 things, and each things can be combined with one other thing, that's 45 possible combinations. For example, maybe I create create 10 functions for a complicated object type. I can sum the objects, multiply them, increment them, etc. Now I want to increment an object and sum with it another. Next I multiply some some objects and then sum the products. That's two function combinations out of a possible 45.

        This shows how quickly the complexity of a system with many interacting parts can increase. It might not take me long to write 10 functions. But to check all 45 potential pairings could take a while. And it's not like we can only combine two functions. I've seend code like funcA(funcB, funcC). With 3 functions combined out of 10, we have 120 possible combinations. 

        We must write our programs in ways that make them to easy to troubleshoot, and develop methods quality assurance that are effective.

## Further Learning

## Questions and Answers:

### Troubleshooting Javascript
1. Name some key differences between a *Syntax Error* and a *Logic Error*.
        
        Syntax errors are 'grammatical' type errors. When you write code that doesn't meet the rules of the language, for example, forgetting parenthesis or misspelling a keyword, that is a syntax error. These usually produce error output that can be quickly traced.

        Logic errors are when you write syntactically correct code that can run succesfully, but it doesn't produce the result that you expected or wanted. For example, if you're returning the sum of something when you should be using the average, that's a logic error. If you're checking the string value of something in a conditional, when you should be checking the number value, that could be a logic error. These can be more difficult to trace, as no error messages may be produced. 

2. List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.

        Being new to JavaScript, I have made many *syntax* errors. Not knowing all the keywords, correct operators for things like equality or exponentiation, and format for brackets, braces, quotes; and forgetting things like semicolonss (or adding them when unnecessary), resulted in these syntax errors. Fortunately, the error messages which the browser intepreting the JS produces, as well as the errors which the VS Code IDE highlights, make these pretty easy to trace and fix.

        As my Salmon Cookies project got more complicated, I started producing many *logic* errors. Working with a lot of variables and objects, sometimes I was manipulating the wrong value, or doing the wrong thing with a value and producing the wrong result. Sometimes my conditionals were not triggering in the way I mean them to (for example, if I needed <= instead of <). 

        The first thing I did was rewrite most of my functions so that they actually return something, instead of acting through 'side effects'. This made them easier to test. Then I was able to build my functions one at a time, iteratively, testing the function until it produced the value I wanted.

        The second thing I did was seprate my tasks by purpose, and group them into two new object types. I designed a Store type to handle all the data of the store, and process calculations with it. I made a Table type to transform this data into a user readable output (HTML Tables), using the DOM.

        This division made it easier to design and analyze the program.
        
3. How will this topic continue to influence your long term goals.

        When designing and writing, I will consider how to make the program easier to troubleshoot. As programs get more complex, the potential for error, and the diffiuculty in troubleshooting them, can increase exponentially.
        
### JS Debugger
1. How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?
        
        Various browsers have a debugger tool in their "dev tools". It lets you step through the code, observe the values of various expressions while you're stepping through it, and trace the program's execution. It can be very useful for seeing exactly what is happening in your program.     

2. Define what a breakpoint is.
        
        The user of the debugger defines a breakpoint in the program which tells the debugger where to stop. Otherwise the whole program would just complete and you wouldn't see what's happening. To start out, it's useful to put a breakpoints at the returns of a function you want to check.

3. What is the call stack?
        
        It shows the program go to the point it is currently at in the code. If you're in a function, it will show what called that function. If that was in turn a function, it will show what called that function, and so on. 