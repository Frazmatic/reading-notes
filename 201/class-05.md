# Class 05 Notes

## Why This Matters

The tools HTML5 provides allow us to make accessible websites that present information in a comprehensible format that effectively conveys information. Similarly, with CSS formatting we can shape our formatting in such a way to make the website more usable and enjoyable.

### What is a real world use case for the alt attribute being used in a website?

The alt text provides a text alternative to images. It can be read by screen readers, or used when bandwidth or technological limitations prevent viewing the image. It helps ensure accessibility of the website regardless of technological or physical limitations. Two realworld situtions for use of alt text are visually impaired users reading the site and people in remote areas utilizing lightweight browsers and devices.

### How can you improve accessibility of images in an HTML document?

Utilize detailed alt text to provide a textual alternative to pictures. Utilize captions to provide *additional* information. Don't use images alone for navigation.

### Provide an example of when the figure element would be useful in an HTML document.

Figures are used to provide supportive, additional, meaning in a concise way; for example, charts or illustrations of a subject, or even a section of another text or an audio recording. An example would be a chart in an article about the stock market.

### Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community

A fig stores an image line by line, or dot by dot. It can support simple animations. Therefore, it may have more detail, but it is larger. An svg stores an image with a set of instructions. It tells the computer what to draw. It can be more efficient and scalable, but is not necessarily a good way to show something like a photograph.

### What image type would you use to display a screenshot on your website and why?

It is compressed, but lossless, so things like text won't lose clarity.

### Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

The foreground color is the color of the actual content. For example, the text. The background color is the color around/behind that content. A normal book is black 'foreground' with white 'background'.

### Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

I would find a suitable color scheme (several sitesh help identify matching color schemes) and assign various foreground and background colors to different elements depending on the site's theme, content, and purpose. Perhaps a dark theme would make sense, or a floral theme. I might make the header have a background color that contrasts highly with the main articles.

### What should you consider when choosing fonts for an HTML document?

Availability on different devices, readability in different contexts, and suitability for the theme of the site (e.g. no comic sans or cursive on a serious accounting site)

### What do font-size, font-weight, and font-style do to HTML text elements?

font-size allows you to set the actual size of the text; e.g. a fontsize of 2000px would make a single character larger than the screen. font-weight adjusts the **boldness** of the text. font-style let's you set the text to *italic*, oblique, or noramal.

## Describe two ways you could add spacing around the characters displayed in an h1 element.

letter-spacing increases the space between letters. word-spacing increases the space between words.

```
h1{
    letter-spacing: 10px;
    word-spacing: 3em;
}
```