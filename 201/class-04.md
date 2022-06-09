# Class 04 Notes

## Why This Matters

Functions are a fundamental concept in making reusable, clear, code.

Layout is an important UX consideration.

Pair Programming is a useful techique, and can even be fun.

## Summary / Analogy

Functions are similar, but not the same, as the concept in math. I still think of them as a black box.

The military is big on the buddy system. You don't get the organization friciton of a larger unit, but it's easier both to spot problems and think of solutions.

## Things I Want To Know More About

1. arrow/lambda functions in js
2. objects

## Real Time Thoughts

### Ch 4 of HTML & CSS: Links

`<a href="url"> content </a>` : link to other sites
relative url: directory_name/file.ext

`<a href="mailto:email@addrress.com"> name </a>` : email link

attribute **target="_blank"**  to open in a new window.

`<a href="#anElementID"> stuff </a>` : link to element on same page by its id attribute. Can be added to end  of url for other pages.

### Ch 15 of HTML & CSS: Layout (pp. 358 - 364, skim rest)

`position: relative;` : can be used to adjust position relative where element normally  would have bee; for example, can be followed by left: 100px; to move it 100 pixels away from where the left would have been (i.e. 100 pixes to the right)

does not affect other elements

`position: absolute;` : can give position relative to the parent/containing element

does not affect other elements

`position: fixed`: position relative to the browser window; e.g. keep a nav bar at top of screen when scrolling

does not affect other elements

`z-index:` : for determining which elements are on top when overlapping. higher numbers cover lower numbers.

`float:` : move to left or right side of container element. other items in that element will "flow" around it. Should use width property so that the floating element doesn't take up whole width anyway.

**does** affect other elements. 

### Ch 3 of Javascript & JQuery: Functions, Methods, and Objects (pp. 86 - 99)

function: resuable block of code that can take arguments and return a result. arguments called 'paramters' in definition of function.

```
function name(parms) {
    //do stuff
    return value;
}

let x = name(args);
```

anonymous function:
```
let funcVar = functions(parms) {
    //do stuff
    return value;
}
```
can then use the variable name like a function e.g. let x = funcVar(args).

immediately called (IIFE):

let x = (function(parms) {

}(args))

### Article: [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

Two programmers work together on the same (single) screen/workstations. Collaborative effort between a 'Driver and a Navigator'.