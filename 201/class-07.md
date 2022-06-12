# Class 07 Notes

## Why This Matters

        We are learning a particular 'paradigm' used in programming, object oriented. When approaching a problem, we need to know what exactly the problem is in order to solve it. We 'model' things and their behaviors as data, in a way that we can understand and implement in a programming language. This is a useful way of breaking down complex issues into actual instructions & information that can be written in a programming language, and keeping it organized in a manner that we can understand and work on effectively.

## Questions and Answers:

### Domain Modeling

1. Explain why we need domain modeling.

        Well thought out domain modelling allows to to determine what information and behavior needs to be represented. It allows us to figure out the actual problems being solved, and exactly what needs to be created to solve them.

### HTML Table Basics

1. Why should tables not be used for page layouts?

        Tables are not "automatically responsove"; that is, they are static, not dynamic. Using them for layout obfuscates the actal content of the page, lacking semantic or contextual meaning, and overcomplicating the HTML structure. They are meant to contain tabular data, not structural information.

2. List and describe 3 different semantic HTML elements used in an HTML `<table>`.

        `<th>` : marks the header/title for a column/field in the table
        `<tr>` : marks every new row/record in the table
        `<td>` : marks the indiviual cell/entry in a row.

### Introducing Constructors

1. What is a constructor and what are some advantages to using it?
        
        Constructors are functions used to create a new object (with the new keyword). The are generaly a function named after the "type" that is being created. They allow us to create an indefinate number of the new object type in a generalizable, programatic, encapsulated, way. 

2. How does the term this differ when used in an object literal versus when used in a constructor?
        
        In a a constructor,  'this' refers to the property being set for the new instance of an object being created. In methods other than constructors, this will refer to the property of an already extant instance.

### Object Prototypes Using A Constructor

1. Explain prototypes and inheritance via an analogy from your previous work experience. NOTE: This is a very common front end developer interview question
        
        In object oriented programming, we are organizing our model by defining categegories, or in other words, creating specifications for classifications. 'Classes' are a common word for programmer defined object types in OOP; although, you don't need to use `class` to create your own type/category/class of object in JS.

        Consider how categories work. We might define a "mammal" class/category as having the properties 'warm blooded', 'has hair', 'nourishes young with milk'. We have other categories of mammal which "inherit" all those properties from the "mammal" class. A "Person" object also has those properties, as well as properties and behavior specific to people. It's the same for camels, dogs, and elephants. The "mammaL" class, in turn, inherits from the "vertebrate" class properties that all vertebrates, not just animals, have, and "vertebrates" inherits from the "animal" class. "Camel" is a subclass of "Mammal". "Animal" is a superclass of "Vertebrate". Sublclasses inherit from superclasses.

        'protoype' is a property which all JS objects have. It indicates the object from which a JS object inherits shared properties. If we assign a method or property to an object's protope, all objects of that type inherit that method or property. If we set the protype field to an object, that assigned object becomes the superclass. We might think of setting the protype as assigning a template, and adding properties/methods to the prototype as changing the template.







