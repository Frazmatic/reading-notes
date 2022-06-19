# Class 11 Notes

## Why This Matters

Responsive design ensures that people accessing the site from a wide variety of devices, can all have a good user experience.

## Further Learning

## Questions and Answers:

### [Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.

In the past, there was no native support for video & audio. You had to use plugins. Now, video & audio support are built into HTML5. We also have more services for hosting, such as Youtube.

2. Describe the use of the `src` and `controls` attributes in the `<video>` element.

The source attribute contains the location and name of the video file. 

The controls attribute is boolean (it doesn't need to be "set", including it makes it 'true'). If the controls element is in the tag, the browser will include it's built in playback controls for the file.

3. WHy is it important to have **fallback content** inside the `<video>` element?

If the browser doesn't support the video element, the fallback content will be displayed. This can avoid confusion for the end user, and provide a backup method of access for the video.
        
### [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

1. How does Grid layout differ from Flex?

    Flex is more about adjusting the flow/wrapping of a one dimensional list of entities. Grid is more two dimensional in that it allows explicitly laying out what grid areas go in what rows and columns.

2. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

    1. Grid Container: The elmeent where grid is applied.
    2. Grid Item: The items inside a Container, the child elements of that container element.
    3. Grid Line: The lines that separate the cells of the grid; the division between rows and columns.

### [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

1. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

Responsive images can reduce bandwidth wastage, and ensure that the image displayed makes sense regardless of the resolution or orientation of the screen it's being viewed with.

2. Define the following `<img>` attributes: `srcset` and `sizes`. Write an example of how they're used.

srcset lets you provide a list of filenames, each followed by the image's actual width in pixels and the letter w, separated by commas. 

sizes lets you provide a list of media conditions (viewport sizes) paired with the slot size for that condition. It will go to the condition it finds to be true, and select the image from the srcset that matches that size. The sizes list ends with a default size in case none of them are true.

An example would be using an image with a different ratio when viewed on a vertically oriented screen versus a wide screen.

3. How is `srcset` more helpful for responsive images than CSS or JavaScript?

CSS and JS apply after the HTML and images have been loaded. Srcset ensures just the correct image is loaded. 