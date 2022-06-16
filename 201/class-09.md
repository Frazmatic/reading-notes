# Class 08 Notes

## Why This Matters

        Forms and events allow us to capture input from users in a programmatic, generalizable manner which allows for validation. Their use and design is an important part of the User Experience (UX).

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


Provide a name attribute to every form element for use by the client & server computers.

### JavaScript Events
1. How would you describe events to a non-technical friend?
        Computers use 'events' to communicate with programs. They're a way of letting the program know that something has happened. When something happens, such as a button being pressed, the computer creates an event object which the program can "handle".
2. When using the addEventListener() method, what 2 arguments will you need to provide?
        
3. Describe the event object. Why is the target within the event object useful?
        .
4. What is the difference between event bubbling and event capturing?
        .