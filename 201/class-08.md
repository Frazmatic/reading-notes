# Class 08 Notes

## Why This Matters

        W

## Questions and Answers:

### CSS - Flexbox
1. Flexbox is designed for one-dimensional content. Explain what this means.
        A series of content. The type of content that can be laid out vertically ***or*** horizontally without losing meaning. 
2. Explain the difference between the main axis and cross axis.
        Main axis is set by flex-direction property. If, for exaple, flex direction is set to row; the main axis is horizontal and the cross axis is vertical. 
3. How can using certain properties of flexbox negatively impact accessibility?
        The order in which things appear on screen may not math the order in which they appear in HTML. Screen readers will read in the order they appear in HTML. If understanding the content depends on the order of appearance, users of devices such as screen readers will have trouble understanding it. Similarly input such as using the keyboard to navigate will follow the structure of the document, not the visual structure generated by flexbox.

### Layout - Flexbox
1. What are some advantages of using flexbox over float?
        Flex allows you to make all the rows and columns take up the same height or width; easily vertically center content inside its parent, control which way things flow and wrap, and other things which better control layout then just having inline elements wrap around a box. 
2. How does this topic connect with your long term goals?
        This is a more modern, dynamic, and powerful method of controlling the layout of content. I want to display data in a way that's easy for people to understand and use. This will be very handy for that.