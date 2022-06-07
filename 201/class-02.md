# Class 02 Notes

## Why This Matters

These are the fundamentals of web development. With what we have learned in this lesson, we can now accomplish flow control and customize the site's presentation.

## Summary / Analogy

Conditional statements are making simple decisions. An if statement is a yes/no decision, but can result in a complex set of possible outcomes. If I'm driving somewhere, depending on what left/right decisions I make at each intersection, I can arrive at many different places.

A variable is just a label for a specific location in memory. If I want to know what's in a mailbox, I don't need to know the specific GPS coordinates. I can refer to the label, like "my home mailbox" or "the mailbox at 123 Main Street". 

Similarly, if I'm asking for the contents of a mailbox but give a label that refers to a garage, I won't get the right results. Data types can have the same issue.

## Things I Want To Know More About

1. Other data structures besides arrays.
2. More about designing objects and their methods and properties.
3. Storing variables for long term access (e.g. in a database or on a hard drive).

## Real Time Thoughts

### Ch 2 of HTML & CSS: "Text"

Structural Markup:
1. `<h1>` through `<h6>`
2. `<p>`
3. `<sup>`
4. `<sub>`
5. `<br />`
6. `<hr />`

Semantic Markup:
1. `<strong>`
2. `<em>`
3. `<blockquote>`
4. `<q>`
5. `<abbr>`
6. `<cite>`
7. `<dfn>`
8. `<address>`

Changes to Text:
1. `<ins>`
2. `<del>`
3. `<s>` 

### Ch 10 of HTML & CSS: "Intoducing CSS"

CSS uses selectors and declarations.

Selectors select various HTMLS elements. Declarations determine how they're styled.

CSS can be linked externally, contained in a style element, or done in line with the style attribute.

There are various selectors that allow for the selection of one or more elements, by type, class, descendency, etc.

Child elements inherit their parents style. CSS rules cascade from least to most specific (rules under more specific selectors takes precendence)

### Ch 2 of Javascript & JQuery: "Basic Javascript Instructions"

A statement is an individual instruction in a script / program. Each one should start on a new line an they are ended with semicolons. Curly braces can be used to delineate code blocks.

Coments can be added to code with /* */ or //.

A variable stores a value. It is essentially a label for a location in memory. A variable is assigned a value with the equal sign (called the assignment operator in this context).

Arrays are list-like variables.

JS has numeric, string, and boolean data types.

Expressions evaluate into a single value.

Operators "operate" on literals or variables to create an expression.

### Ch 4 of Javascript & JQuery: "Decisions and Loops" (pp. 145 - 162)

Decicision making allows for flow control within a program. Comparison operators return true or false and can be used with a conditional statement such as an if statement.

Logical operators: `&&` AND, `||` OR, `!` NOT. "AND" returns true if both expressions are true. OR returns true if eitehr expression is true. NOT returns true if the expression is false.

`if (expression) {
    statement1;
}
else {
    statement2;
}`

Executes statemetn1 if expression is true, otherwise executes expression2.
