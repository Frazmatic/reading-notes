# Learning Operators and Loops

## Navigation

[Introduction](https://frazmatic.github.io/reading-notes/) | [Growth Mindset](https://frazmatic.github.io/reading-notes/growth-mindset) | [Learning Markdown](https://frazmatic.github.io/reading-notes/learning-markdown) | [Text Editors](https://frazmatic.github.io/reading-notes/text-editor) | [Using Git](https://frazmatic.github.io/reading-notes/using-git) | [Learning HTML](https://frazmatic.github.io/reading-notes/learning-html) | [Learning CSS](https://frazmatic.github.io/reading-notes/learning-css) | [Learning Javascript](https://frazmatic.github.io/reading-notes/learning-javascript) | [Learning Functions](https://frazmatic.github.io/reading-notes/learning-functions) | [Learning Operators and Loops](https://frazmatic.github.io/reading-notes/learning-operators-and-loops)

## Operators

Operators are, as they sound, symbols that perform "operations". Generally they will performa an operation on values; these values can be a literal like '2' or variable identifiers. The values which the operation is occuring with are the 'operands'. 

The assignment operator `=` assigns the value on the right to the given variable on the left. For example, `a = 5;` would give the value of the number 5 to the variable named a. There are shorthand assignment operators such as `+=`. Following `a = 5` with `a += 2` would be equivalent to `a = a + 2`. In this case it would result in a having a value of 7.

Comparison operators return a logical (i.e. boolean true or false) value. For example, if a = 7, `a < 5` would return false and `a > 6` would return true. They can be used for conditional expressions such as if statements. `==` checks if the two operands are equal to each other, `<=` is "less than or equal to", `===` is a "strict equal" (no automatic type conversion), `!=` is "not equal to".

## Loops

Loops will repeat a given set of expressions. They will generally use some sort of conditional statement, otherwise they'd run forever. The general format for a "for" loop is as follows:

`for ([initialExpression]; [conditionExpression]; [incrementExpression])`
    `{`
        `//expressions`
    `}`

"initial expression" is a starting value, "conditional expression" determines when the loop will be exited, and "increment expression" changes the initial expression value every loop.

Example:

`for (let step = 0; step < 100; step++)`
    `{`
        `console.log(step);`
    `}`

This loop will start with the variable 'step' set to 0. It will output "step" to the console every loop. The first iteration of the loop would output "0". It then increments the value of "step" by one. Every loop it checks if "step < 100". 99 would be the last value outputted, because when step == 100, it wold no longer meet the conditional requirement of "step < 100", and the loop wil be exited.

A while loop has the following format:

`while (conditionalExpression)`
    `{`
        `//expressions`
    `}`

The loop will repeat until the given conditional expression is false. It is good for a loop where the number of iterations required is not known beforehand. A variable will need to exist and intialized before the loop is entered, otherwise the conditional expression will have nothing to check the first iteration. Something in the loop must be able to change the variable, or else it will run forever.