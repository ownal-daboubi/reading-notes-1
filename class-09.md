# Read: 09 - Forms and JS Events
# Forms in HTMl:
* `<form>` element: Form controls live inside it.
* `action` attribute: Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
* `method` attribute (get or post): used to send the forms.
* `id` attribute: used to identify the form distinctly from other elements on the page.
* `<input>` element: used to create several different form controls.
* `type="text"` attribute: it creates a single-line text input.
* `name` attribute: When users enter information into a form, the server needs to know which form control each piece of data was entered into.
* `<textarea>` element: used to create a mutli-line text input.
* `<select>` element: used to create a drop down list box.
* `<option>` element: used to specify the options that the user can select from.
* `<button>` element: allow users more control over how their buttons.
* `<fieldset>` element: group related form controls together inside the form.
* `<legend>` element: come directly after the opening `<fieldset>` tag and contains a caption which helps identify the purpose of that group of form.
* Example:
``` <form action="http://www.example.com/subscribe.php"
method="get">
<p>Username:
<input type="text" name="username" size="15"
maxlength="30" />
</p>
<p>Password:
<input type="password" name="password" size="15"
maxlength="30" />
</p>
<p>Please select your favorite genre:
<br />
<input type="radio" name="genre" value="rock"
checked="checked" /> Rock
<input type="radio" name="genre" value="pop" />
Pop
<input type="radio" name="genre" value="jazz" />
Jazz
</p>
<p>Subscribe to our email list:</p>
<input type="text" name="email" />
<input type="submit" name="subscribe"
value="Subscribe" />
</form>
```

# Lists, Tables & Forms in CSS:
## Lists properties:
* `list-style-type` property allows you to control the shape or style of a bullet point.
* `list-style-image` property specify an image to act as a bullet point.
* `list-style-position` property indicates whether the marker should appear on the inside or the outside of the box containing the main  points.
* `list-style` property allows you to express the markers' style, image and position properties in any order.

## Tables properties:
* `width` to set the width of the table.
* `padding` to set the space between the border of each table cell and its content.
* `letter-spacing`, `font-size`to add additional styling to the content of the table headers 
* `border-top`, `border-bottom` to set borders above and below the table headers
* `text-align` to align the writing to the left of some table cells and to the right of the others.
* `background-color` to change the background color of the alternating table rows.
* `:hover` to highlight a table row when a user's mouse goes over it.

## Forms properties:
* Styling text input using: font-size, color, background-color, border..etc.
* Styling submit button using: border-bottom, background-color, text-shadow.
* Styling fieldsets using: border-radius, padding

![](https://uicookies.com/wp-content/uploads/2019/09/css-contact-form-1000x750.jpg)

# JavaScript Events:
* Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked).
* Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen  upon.
* When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user.
* You can use event delegation to monitor for events that happen on all of the children of an element. The most commonly used events are W3C DOM events, although there are others in the HTMLS specification as well as browser-specific events.
* Events can be used to trigger a function in your JavaScript code.
* Event Handling:
 1. Select the element node(s) you want the script to respond to.
 2. Binding: Indicate which event on the selected node(s) will trigger the response.
 3. State the code you want to run when the event occurs.
<<<<<<< HEAD
* Traditional Event Handler: `element .onevent = functionName ;`
* Event listener: `element .addEventlistener('event', functionName [, Boolean]) ;`
=======
* Traditional Event Handler: `element .onevent = functionName ;`.
* Event listener: `element .addEventlistener('event', functionName [, Boolean]) ;`.
>>>>>>> 98fffa1029cafe458feed5dde2a1f5bfe74692a1
* Changing delfault behaviour of an element:
 1. `preventDefault ()`.
 2. `stopPropagation()`.

![](https://i.stack.imgur.com/BTm1H.png)
