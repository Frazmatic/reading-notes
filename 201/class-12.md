# Class 12 Notes

## Why This Matters

The canvas element and charts allow for versatile visual communication with the users. 

## Further Learning

## Questions and Answers:

### [JavaScript Canvas](https://www.javascripttutorial.net/web-apis/javascript-canvas/)

1. What does the `<canvas>` allow a developer to achieve?

    The canvas provides an area the program can draw on.

2. What is the importance of closing the `<canvas>` tag?

    The content between the opening and closing canvas tags is fallback content, similar to videos.

3. Explain what the `.getContext()` method does. 

    getContext() returns an object, which is an interface, that allows the program to draw on the canvas. If the argument passed to getContext is "2d" (e.g. `canvas.getObject('2d')`;) it return a rendering context object that allows one to draw lines, shapes, and text. It can provide styling elements such different colors, shading, and rotation.


### [Chart.js Documentation](http://www.chartjs.org/docs/)

1. What is Chart.js and how can it be brought into your project?

    Chart.js is a javascript package that makes it easier to draw a variety of chart types on a Canvas element.

    Chart js can be added to a project with a project with the npm installation or a link directly to the website. Either way a script src link must point to the chart.js file befre your custom script. 

2. List 3 different Chart types you can create using Chart.js. 

    1. Line
    2. Bar
    3. Pie/Donut
    4. Scatter
    5. Bubble
        Two examples of bubble chart use (used for 3 dimensional information):
        1. Comparing populatoin density, unvaccinated rate, and COVID-19 per capita cases
        2. Comparing time, cost, & revenue



### [Easily Create Stunning Animated Charts with Chart.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

1. What are some advantages to displaying data via charts over tables?

    Humans aren't really meant to process spreadsheets. Visual representations are more intuitively understandable. Data can be conveyed faster with a chart.

2. How could Chart.js aid your previously created applications visually?

    A bar chart would be an excellent way of representing hourly sales or staffing in the salmon cookie project. 