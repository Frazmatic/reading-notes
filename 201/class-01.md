#Class 01 Notes

## Why This Matters

This material covers how HTML, CSS, and JS work together and what they're purposes are. It is important to have an understanding of the fundamental reasoning behind each to build a well designed page. The sections on HTML explain how to use to properly structure the *information* being shared with the page. The sections on layout & design explain how to make the page more useful for its users. The section on JS explains how programming works with web pages to provide dynamic behavior.

## Summarize and Explain Via Analogy

In the military we have organizational plans & mission plans which provide a basic structure based on a desired function. We have regulations & communication systems which affect their presentation. We have standard operating procedures, orders, and documented instructions which affect behavior. 

Other systems can be thought of similarly. Rules govern structure, rules govern behavior, and rules govern observation. 

## Things I want to know more about

1. Best practices for HTML5 semantic tagging (e.g when to use sections, when to call something an article or an aside)
2. Accessibility features besides just screenreaders (e.g. assistive technology for mobility or cogntively impaired) and how to support them.
3. Best design practices for conveying information based on cogntive science, pedagology, and taking into account cultural factors.

## Real Time Thoughts

### Ch 1 of HTML & CSS: Structure (pp. 12 - 39)

HTML provides structure for the information within documents. This aids understanding. Each HTML tag describes the structural meaning (what type of part it is) for an 'element' of the document. It's a markup language used to provide annotations for the document. 

Structural elements such as headings and subheadings help defined and identify the "heirarchy" of information within the document. For example, a headline describes the major theme of the information in that document; subheadlines describe the constituent themes of the subcomponents within. Simililarly, each paragraph addresses a particular topic within that theme. An article describing a complex concept might have a single heading describing the overall subject, be divided into multiple sections each with their own subheading, and even have further division under those in sub-sub-headings. Each sub-sub-heading would cover multiple paragraphs of content.

Tags mark elements. They are like containers. In HTML the overall document is delineated with `<HTML></HTML>` tags. Within that document the `<body>` tag describes where the actual informational content will go. The body can be broken down into header, main, and footer. Headings are marked with `<h1></h1>` tags, with subheadings using h2 though h6 depending on level. Paragraphs are at the lowest level, and marked with `<p></p>`. Overall, every tag describes the information between the tags.

These tags create a sort of tree (heirarchical) structure.

Technically a single element would consit of the the opening and closing tags as well as the information contained within.

Attributes provide further information about an element. They consist of name (describing which property of the element is being set), a value (the actual info/setting for that property), and assignment operator `=` setting the property to that value. Attributes are set within the opening tag following its identifier. Different types of elements have differents sets of attributes to adjust. Each type of attribute has different valid values.

The head element, located before the body, contains information about the page itself, not the information within. For example, the title element in the head element sets the title which is displayed for that page in the browser (in the title bar or tab). 

Content management systems can create some of this code for you, using templates. Sometimes they let you directly edit the code they generate.

### CH 8 of HTML & CSS: Extra Markup (p 176 - 199)

The !DOCTYPE tag indicates to the browser which version of HTML is being used . `<!DOCTYPE html>` indicates HTML5. 

`<!-- -->` is used to add comments to HTML documents where the comment is written between these tags. Comments are not visible to the end user but can be seen in the source.

Global attributes are attributes which all elements have. 

The 'id' attribute is a global attribute used to identify particular elements. It acts as a unique identifier on that page which can referred to by CSS or JS. 

The 'class' attribute is used to identify a set of elements. It can be used to create a category of element, and referred to by CSS or JS. An element can also belong to multiple classes.

Two categories of element are block & inline. Block elements always start on a new line. For example, `<p>` and `<h1>` are block elements. Inline elements will continue on the same line. For example, `<a>` (an anchor element, used for things like links) and `<img>` are inline elements.

The `<div>` element can used to group elements into a block level grouping. This element can then be assigned an id and/or class attribute allowing it to be adjusted with CSS or JS. Similarly, the `<span>` element can be used to create inline groupings.

The `<iframe>` element allows one to embed a page within another page. It uses src, height, and width attributes. The seamless attribute can also be used to get rid of scrollbars.

`<meta>` elements go in the `<head>` element and contain information about *the page itself*. It uses attributes for that information. The "name" and "content" attributes are the most commonly used, with names such as "author", "description", and "keywords" used to provide information about the site (often used by things such as search engines).

Escape characters allow one to display characters which would normally be interpreted as code. For example, the left angled bracket (less than sign), normally used to delineate tags, can be displayed with `&lt;`. 

### CH 17 of HTML & CSS: HTML5 Layout (pp. 428 - 451)

HTML5 layout elements are more specific alternatives to just grouping things with divs. They are more semantically meaningfull. They have names which actually indicate the type of content inside.

`<header>` and `<footer>` elements are used within the body or individual articles. They have the same meaning as with normal writing; for example, they might contain contact information or copyright information. 

`<nav>` elements contain a collection of navigational links for the site.

`<aside>` elements are used like pullquotes or a related content section.

`<article>` elements contain a section that could be seen as a stand alone article.

`<hgroup>` elements group related headings together, such as an article title & subtitle.

`<section>` groups related content, e.g. a cooking section might have several recipe articles, or a single articel might have several sections with several paragraphs each. Generally suitable for something that would get its own heading.

`<figure>` elements are for content referenced by an article, such as an image of a diagram or a section of another text. The `<figcaption`> is used within them to provide a description of the figure content.

Div elements can still be used to group things that don't fit these categories.

Older browsers may have trouble understanding some of these new HTML5 elements. They will all be treated as inline elements.

### CH 18 of HTML & CSS: Process & Design (pp. 452 - 475)

Like other forms of communication, you should understand your target audience. Factors to consider include demographics such as age marital status, what sort of technology they will be using to access the site, and background knowledge. The type of information you include and its presentation can be adjusted to better fit this audience.

Consider the purpose of your site, why people visit it. What are their motivations and goals (in regards to using the site). What are the use cases? What will visitors achieve via the site?

Use this to figure what information they need and how to prioritize it. Make sure the relevance of the site is immediately apparent.

Consider the frequency of visitation to the site.

Site maps are conceptual tools for organizing the pages of the site. Pieces of information are grouped and related to pages. Multiple pages by be grouped together as well. A diagram is created that show how the different sections/groups are connected. 

A wireframe is a sketch of how information is layed out on a page. It is functional in focus rather than appearance based. It helps you know what information needs to be where. 

Prioritize information using a visual heirarchy. Organize it into related chunks. Make the purpose of each part of a page clear at first glance.

### CH 1 of Javascript & JQuery: The ABC of Programming (pp. 11 - 52)

A script is a series of instructions.

The instructions must be very explicit, computers can't figure things out on their own.

Think of a goal. Break down what is necessary to achieve the goal into tasks & decisions. Break down the tasks into steps.

Flowcharts describe program flow.

We use data to model the world. In OOP we think of things as objects with properties.

In event based programming we used computer generated events to trigger certain actions.

Methods are functions within an object. An object can have multiple methods.

Document objects represent an HTML page. An event (sent from the browser) can trigger an object's method.

Content -> Presentation -> Behavior = HTML -> CSS -> JS

extern link, script tag