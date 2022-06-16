# Class 08 Notes

## Why This Matters

        Forms and events allow us to capture input from users in a programmatic, generalizable manner which allows for validation. Their use and design is an important part of the User Experience (UX).

## Further Learning

        How to save this input locally and on a web server.

        Validation

        More about propogation

## Questions and Answers:

### HTML Forms
1. Why are forms so important in web development?
        They allow for user controls or capturing user input. Forms a common component of useful websites. A common use case for websites is capturing data via a form to process and/or store on a server.
2. When designing a form, what are some key things to keep in mind when it comes to user experience?
        Don't make it too big; that's confusing, tiresome, and error prone. KISS. Make sure it matches user expectations (mental models). Visually group related fields. Try to stick to a single column layout. Consider tab order. The form should be easy to read and navigate.
3. List 5 form elements and explain their importance. 
        I. `<form>`: Contains the form as a whole. action attribute tells where to send/receive data. method attribute can be set to 'get' or 'post'.
        II. `<input>`: Various types available as attributes; e.g. radio, text, email
        III. `<label>`: takes attribute with id of form control being labelled; describest the form control.
        IV. `<textarea>`: larger text input; has a closing tag. Default value contained within.
        V. `<button>`: A button possible types submit, reset, or button. Can be used to send form values with submit, reset form to default values with reset, or to call custom JS with 'button'.
        VI. `<fieldset>`: Group together related elements for semantic and styling purposes
        VII. `<legend>`: label a fieldset


        Note: Provide a name attribute to every form element for use by the client & server computers.

### JavaScript Events
1. How would you describe events to a non-technical friend?
        Computers use 'events' to communicate with programs. They're a way of letting the program know that something has happened. When something happens, such as a button being pressed, the computer creates an event object which the program can "handle".
2. When using the addEventListener() method, what 2 arguments will you need to provide?
        The event being handled, and a function to handle it with.
3. Describe the event object. Why is the target within the event object useful?
        The event object is passed to the function given in addEventListener(). The function can use the event object to get information about the event. The target will represent the object that generated the event; for example, the form, field, or button that generated the event, or the mouse that was clicked.

        For example, if a form generates a submit event, the event.target object will contain the various elements in the form and their values.
4. What is the difference between event bubbling and event capturing?
        Capture checks the "outermost" elements for event handlers first. If an input field is in a form, and the form is inside a section, and the section is inside the body; input is the 'innermost' element. If you have listeners for the same event (e.g. click) assigned to input, form, section, and body; "capturing" will look at the body one first. It checks the body first to see if it has a listern, if it does not, it checks the section and so on.

        If the 'bubbles' property for an event is true, it does 'bubbling'. This goes the opposite order of capturing. It will run that handler for the innermost element first, and continue outward. 

        Modern browsers will do capturing first, than bubbling. If you want only the innermost handler for same event to go off, wihtout bubbling back out, you can use the .stopPropogation() method on the event object.