# HTML Book
# Chapter 7 

### Why Forms?
* In addition to enabling users to search, forms also allow users to perform other functions online. You will see forms.
* when registering as a member of a website, when shopping online, and when signing up for newsletters or mailing lists.

### Form Controls
* ADDING TEXT:Text (one line or multible),Password.
* Making Choices:Radio buttons,Checkboxes, and Drop-down boxes.
* Submitting Forms:Submit buttons and img buttons.
* Uploading Files:File upload.

### How Forms Work?
* A user fills in a form and then presses a button to submit the information to the server.
* The name of each form control is sent to the server along with the value the user enters or selects.
* The server processes the information using a programming language such as PHP, C#, VB.net, or Java. It may also store the information in a database.
* The server creates a new page to send back to the browser based on the information received.

### Form Structure

* Form controls live inside a `<form>` element. This element should always carry the action attribute and will usually have a method and id attribute too.
* `action` Every <form> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
* `method` Forms can be sent using one of two methods: get or post.

### Text input
* The <input> element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.
* `type="text"` When the type attribute has a value of text, it creates a singleline text input.
* `name`  When users enter information into a form, the server needs to know which form control each piece of data was entered into.
* `type="password"` When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.
* The `<textarea>` element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag.

* `<input>` `type="radio"` Radio buttons allow users to pick just one of a number of options.
* `name` The name attribute is sent to the server with the value of the option the user selects.
* `value` The value attribute indicates the value that is sent to the server for the selected option.
* `checked` The checked attribute can be used to indicate which value (if any) should be selected when the page loads.
* `<input>` `type="checkbox"` Checkboxes allow users to select (and unselect) one or more options in answer to a question.
* `name` The name attribute is sent to the server with the value of the option(s) the user selects.
* `value` The value attribute indicates the value sent to the server if this checkbox is checked.
* `checked` The checked attribute indicates that this box should be checked when the page loads.

### Drop Down Li st Box
* `<select>` A drop down list box (also known as a select box) allows users to select one option from a drop down list.
* `name` The name attribute indicates the name of the form control being sent to the server, along with the value the user selected.
* `<option>` The `<option>` element is used to specify the options that the user can select from.

### Multiple Select Box
* `<select>` `size` You can turn a drop down select box into a box that shows more than one option by adding the size attribute. Its value should be the number of options you want to show at once. In the example you can see that three of the four options are shown.
* `multiple` You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple.

### File Input Box
* `<input>` If you want to allow users to upload a file (for example an image, video, mp3, or a PDF), you will need to use a file input box.
* `type="file"` This type of input creates a box that looks like a text input followed by a browse button. When the user clicks on the browse button, a window opens up that allows them to select a file from their computer to be uploaded to the website.

### Submit Button
* `<input>` `type="submit"` The submit button is used to send a form to the server.
* `name` It can use a name attribute but it does not need to have one.
* `value` The value attribute is used to control the text that appears on a button. It is a good idea to specify the words you want to appear on a button because the default value of buttons on some browsers is ‘Submit query’ and this might not be appropriate for all kinds of form.

### IMG Button
* `<input>` `type="image"` If you want to use an image for the submit button, you can give the type attribute a value of image.

* Whenever you want to c XX ollect information from visitors you will need a form, which lives inside a `<form>` element.
* Information from a form is sent in name/value pairs.
* Each form control is given a name, and the text the user types in or the values of the options they select are sent to the server.
* HTML5 introduces new form elements which make it easier for visitors to fill in forms.

# Chapter 14: “Lists, Tables & Forms” (pp.330-357)

* In addition to the CSS p XX roperties covered in other chapters which work with the contents of all elements, there are several others that are specifically used to control the appearance of lists, tables, and forms.
* List markers can be given different appearances using the list-style-type and list-style image properties.
* Table cells can have different borders and spacing in different browsers, but there are properties you can use to control them and make them more consistent.
* Forms are easier to use if the form controls are vertically aligned using CSS.
* Forms benefit from styles that make them feel more interactive.

# JS Book
# Chapter 6 
### DIFFERENT EVENT TYPES
Here is a selection of the events that occur in the browser while you are
browsing the web. Any of these events can be used to trigger a function
in your JavaScript code.

![events](https://github.com/talaemad/reading-notes/blob/main/event.png)

### TERMINOLOGY
* EVENTS FIRE OR ARE RAISED When an event has occurred, it is often described as having fired or been raised. In the diagram on the right, if the user is tapping on a link, a click event would fire in the browser.
* EVENTS TRIGGER SCRIPTS Events are said to t rigger a function or script. When the click event fires on the element in this diagram, it could trigger a script that enlarges the selected item.

![events](https://github.com/talaemad/reading-notes/blob/main/events.png)

### HOW EVENTS TRIGGER JAVASCRIPT CODE
* When the user interacts with the HTML on a web page, there are three steps involved in getting it to trigger some JavaScript code. Together these steps are known as        `event handling`.

* Event handlers let you indicate which event you are waiting for on any particular element. There are three types of event handlers.

* `element .onevent functionName ;`

* Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.
* When an event occurs, the event object tells you information about the event, and the element it happened upon.
* Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.

* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon.
* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
* You can use event delegation to monitor for events that happen on all of the children of an element.
* The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.