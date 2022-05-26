# Learning CSS

## Navigation

[Introduction](https://frazmatic.github.io/reading-notes/) | [Growth Mindset](https://frazmatic.github.io/reading-notes/growth-mindset) | [Learning Markdown](https://frazmatic.github.io/reading-notes/learning-markdown) | [Text Editors](https://frazmatic.github.io/reading-notes/text-editor) | [Using Git](https://frazmatic.github.io/reading-notes/using-git) | [Learning HTML](https://frazmatic.github.io/reading-notes/learning-html) | [Learning CSS](https://frazmatic.github.io/reading-notes/learning-css) | [Learning Javascript](https://frazmatic.github.io/reading-notes/learning-javascript) | [Learning Functions](https://frazmatic.github.io/reading-notes/learning-functions)

## CSS

CSS is a language designed to control the presentation of web documents. HTML structures the meaning of the page's content. CSS control's the page's style. 

CSS is used by creating rules for one or more elements. For example:

`h1 {`
    `color: red;`
`}`

This establishes a rule for h1 (headline) elements, making the color of text in them red. Each rule is a property paired with a value, and has a semicolon terminating it. Multiple rules can be enclosed in the braces for a particular element selector.

CSS consists of multiple modules. Similar properties will be defined in the same module.

CSS can be added with an external file, an internal (to the HTML file) element, or with inline (to an HTML tag) arguments. 

A linked css document can be added to an HTML file by including the following in the head element:

`<link rel="stylesheet" href="mystyle.css">`

An internal CSS section can be added with the style tag, as follows:

`<style>`
`elem_name {`
    `property:value`
`}`

Inline CSS can be added with the "style" attribute for an element.

