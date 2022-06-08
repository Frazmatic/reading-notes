# Class 02 Notes

## Why This Matters

    Lists and the box model are important in presenting an easy to read, usable, site. Loops allow logic to be conditionally repeated, greatly expanding the possible behavior of a script. Arrays are very handly data structures for handling lists of related values/objects.

## Summary / Analogy

Truthy basically checks for existence. Loops happen with people too; "do this until...". Arrays can be thought of like a bookshelf, skyscraper, etc. Position is measured from the bottom "0" and they are limited in size.

## Things I Want To Know More About

1. Other types of built-in objects, for each loops, etc
2. Performance issues with JS arrays.

## Real Time Thoughts

### Ch 3 of HTML & CSS: "Lists"

There are three types of lists in HTML, ordered, unordered, and definition lists.

The `<ol>` tag is used for ordered lists. These have numbered items. The `<ul>` tag is used for unordered lists. These have bullet points. Both types of lists use the `<li>` tag for invdividual items in the lists.

Definition lists use the `<dl>` tag. The terms being defined within the list are marked with the `<dt>` tag. DT tags are followed by `<dd>` tags which contain the definition for that term.

Lists can be nested within other lists.

### Ch 13 of HTML & CSS: "Boxes"

CSS treats every element as having a "box". The properties of these boxes can be adjusted with CSS. The width and height properties can set to a desired size. Percentages, pixels(px), and em are CSS measurement units. Width and height can be limited with the properties: min-width, max-width, min-height, and max-height. 

The overlow property determines what happens if the content within a box is too large for the given size. The property's potential values are hidden and scroll.

Boxes have a border, although it may be invisible by default. Width and style can be adjusted with border-width and border-style. Style values include solid, dotted, dashed, etc. Width can be adjusted with measurement units or thin, medium, thick. The top, bottom, right, and left sides can be set separately. The color can be chanegd with border-color. The shorthand 'border' property can be used to set several values at once; eg "border: 10px solid lightgray".

"Padding" is the space between the content and the border (within the box). Padding can be adjusted with the 'padding' property, also all four sides can be set separately. Margin is the space between boxes (outside the border). Similarly, it can be set as a whole using units or the sides can be set separately.

Setting left & right margins to auto can help center content. A width needs to be set or it will take up the whole screen. "text-alight: center" can be used to center text within a box.

Elements can be manually set to hehave as 'inline' or 'block' with the 'dispalay property'. 'inline-block' retains some behavior of block elements but makes them flow like an inline element. The none property in display hides an element (as if it's not on the page at all). The visibility property can be set to hidden; this hides the element but it still takes up space on the page. It can also be used to manually set the element to visible.

The border-image property can use a referneced image for the border. The box-shadow property ceates a shadow. 

Border corners can be rounded by assigning a measurement to the border-radius property. Elliptical shapes can be achieved with two measurements. The corners can be set separately as well.

### Ch 2 of Javascript & JQuery: "Basic JavaScript Instructions" (pp. 70 - 73)

Arrays are list-like structures. Can be created with arrayName = [item1, item2, item3] or with the Array() constructor. arrayName[index] accesses a particular item in the array. 

### Ch 4 of Javascript & JQuery: "Decisions and Loops" (pp. 162 - 182) 

switch case - handy alternative to if when deciding among a series of enumerated values

type coercion - js automatically tries to convert type in non-strict checks; e.g. 1 == '1' is true. There are 'truthy' and 'falsy' values. For example 0, empty strings, & NaN are false. Non zero numbers and strings are true. therefore if you want to check if a string is not empty `if (string)` is enough; you don't need to do something like `if (string.length > 0)`. However, this can unintentionally cause expressions to be interpreted as true or false. For example `'0'` is a non empty string and would return true. Be careful.