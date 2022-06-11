# Class 06 Notes

## Why This Matters

JavaScript uses objects for many things. Objects are a fundamental structural concept for programming. They are useful way to model the world. Objects are a great way of organizing the data and functions in our code.

## Questions and Answers:

### JS Objects

1.	How would you describe an object to a non-technical friend you grew up with?
        An object represents a thing. Like real life things, an object has traits that can describe it, and actions it can do. In programming, we call these traits “properties” and the actions “methods”.  In JS an object is a structure that associates names with values. These values can be variables or literals for properties, and functions for methods. We can access these “members” with dot notation or brackets.
2.	What are some advantages to creating object literals?
        Having named members makes it more clear what you’re actually accessing or changing. You can also directly add members to an object without using something a push function; you just use the normal dot or bracket access.
3.	How do objects differ from arrays?
        Objects don’t map numbers to spots. They use named members (properties/variables and methods/functions). So instead of “car[0] = ‘Subaru’” we could use “car.make = ‘Subaru’” or “car[‘make’] = ‘Subaru’”. This is much more clear and organized way of organizing information, making the program more readable and easier to use.
4.	Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
        Using bracket notations allows us to access members in a custom, dynamic, way, perhaps using a variable. For example, what if we wanted to access a member of an object without knowing which one beforehand? Maybe a different function or a user is telling the program which property to be read. We would not want to hard code the access such as “theObject.theProperty”. Instead, our program could look at “theObject[theProperty]” where theProperty is a string variable.
5.	Evaluate the code below. What does the term this refer to and what is the advantage to using this?
        This refers to the actual instance of the object calling the method. For example, if you had many car objects, and they had a stop method, “this.speed = 0” in the method would set just the speed property for the particular object running ‘.stop()’ to zero. It’s very useful in constructor code. The constructor function can take arguments, and the this keyword lets it know to set the properties for that individual object to those arguments (rather than setting that property to the same value for all objects of that type). 

### DOM

1.	What is the DOM?
        DOM stands for Document Object Model. It is an object based way of accessing the parts of a web document. It is a programming interface for reading or changing the various elements in a web page (e.g. an HTML doc). 
2.	Briefly describe the relationship between the DOM and JavaScript.
        The DOM gives us a way with interacting with web documents from within JS. Everything is represented with objects.  