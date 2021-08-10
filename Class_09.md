# HTML & CSS
## Forms
A **Form** is a way of collecting information from users of the product, and it widely used in websites.

**Forms** work by asking the user to fill information and then press a button to submit to the server. the name of each and values of each form get sent to the server, then these values get processed by the server using programming language, after that the server creates a new page where the information is sent to be viewed.  

### Form Controls Types:

- Adding text using:
    - Text input
    - Password input
    - Text Area

- Making choices using:
    - Radio buttons
    - Checkboxes
    - Drop-down boxes

- Submitting forms using:
    - Submit buttons
    - Image buttons

- Uploading files using file upload.

### Form Structure:
In order to make a **form** you should use the `<form>` element. This element should always carry the action attribute and will usually have a method and id attribute.

- **action** attribute: it is a required attribute that has a value of the *URL* for the page on the server that will receive the subbitted information by the user.

- **method**: it is the method of sending the forms, and it can be sent by two ways:

    1. Using **get** method: the values of the form are added to the end of the *URL*. This method is ideal for:
        - Short forms.
        - When retrieving data from the web server.

    2. Using **post** method: the values are sent as a *HTTP* header. This method should be used when your form:
        - Allows users to upload a file.
        - Is very long.
        - Contains sensitive data.
        - adds or removes information from a database.

- **id**: it is used to be able to distinguish the **form** from others.

### Input types:
Using the `<input>` element you can create several form controls, and using the **type** attribute you can choose the input type you are creating.

1. ***Text input attributes***:

    - **type="text"**: it creates a single-line text input.
    - **name**: it is the form name that is sent along with the information to the server.

    - **maxlength**: it limits the allowed number of characters in the field.

2. ***Password input attributes***:
    - **type="password"**: it creates a single-line text input with blocked-out characters.

    - **name**: it is the name of the password input, which is sent to the server.

    - **maxlength**: it limits the allowed number of characters in the field.

3. ***Text area***: using a `<textarea>` element you can create a multi-line text input.

**Note**: this element isn't an empty element, meaning it has an opening and a closing tag.

**Attributes**: 
- **cols**: it indicates how wide the text area should be.
- **rows**: it indicates how many rows the text area should take vertically.

4. ***Radio button attributes***:
    - **type="radio"**: allows the user to pick one of many options.
    - **name**: it is sent name with the value of the option to the server.

    - **value**: it indicates the sent value to the server.
    - **checked**: it indicates the value that should be selected when the page loads.

5. ***Checkbox attributes***: 
    - **type="checkbox"**: allows users to select and unselect a set of different options.

    - **name**: it is sent to the server with the value of the options.

    - **value**: it indicates the sent value(s) to the server.
    - **checked**: it indicates the value(s) that should be selected when the page loads.

6. ***Drop down list box***: in order to use the **drop down list box** you need to use the `<select>` element, which allows the user to choose an option from a drop down list using the `<Option>` element.

`<Option>`element attributes:

- **value**:it indicates the sent value(s) to the server.
- **selected**: it indicates the option that should be selected when the page loads.

7. ***multiple select box attributes***:
    - **size**: it's value is the number of the options to be displayed.
    - **multiple**: it allows the users to select multiple options.

8. ***File input box***:
    By using the **type="file"** attribute you can allow the user to upload a file.

9. ***submit button***: 
The **type="submit"** attribute is used to send a form to the server.

## Lists, Tables and Forms

### List styles: 
1. ***Bullet point styles***: 
In order to make a **Bullet point style list** for the  `<ol>`, `<ul>` and `<li>` elements, you chould use the **list-style-type** property with one of these values:
- For **unordered lists**:
    - **disc**
    - **circle**
    - **square**
    - Or **none** for no list type.

- For **ordered lists**:
    - **decimal**
    - **decimal-leading-zero**
    - **lower-alpha**
    - **upper-alpha**
    - **lower-roman**
    - **upper-roman**

2. ***Images for bullets(list-style-image)***: it can be used on unorderd lists.

3. ***Positioning the marker(list-style-position)***.

### Table properties:
- **width**: to set the width of the table.
- **padding**: to set the space between the border of each table cell and its content.

- **text-transform**: to convert the content of the table headers to uppercase.

- **letter-spacing, font-size**: to add additional styling to the content of the table headers.

- **border-top, border-bottom**: to set borders above and below the table headers.

- **text-align**: to align the writing to the left of some table cells and to the right of the others.

- **background-color**: to change the background color of the alternating table rows.

- **:hover**: to highlight a table row when a user's mouse goes over it.

# JavaScript
## Events

### Event Types:
1. **UI Events**: Occur when a user interacts with the browser's user interface (UI) rather than the web pag. **ex**: 

**load**: web page has finished loading.

2. **Keyboard Events**: occur when a user interacts with the keyboard. **ex**:

**keydown**: user first presses a key (repeats while key is depressed).

3. **Mouse Events**: occur when a user interacts with a mouse. trackpad, or touchscreen. **ex**:

**click**: user presses and releases a button over the same element

4. **Focus Events**: occur when a user interacts with a form element. **ex**: 

**focus / focus in**: Element gains focus.

5. **Form Evants**: occur when a user interacts with a form element. **ex**: 

**input**: Value in any `<input>` or `<textarea>` element has changed (I +) or any element with the contented i table attribute.

6. **Mutation Events**: occur when the DOM structure has been changed by a script. To be replaced by mutation observers. **ex**:

**DOMSubtreeModified**: change hc;is been made to document.

### How events trigger javascript code:

1. Select the element node(s) you want the script to respond to(**select element**).
2. Indicate which event on the selectd node(s) will trigger the response(**specify event**).
3. State the code you want to run when the event occurs(**call code**).

### Ways of binding events to elements:
1. **HTML Event Handlers**: a bad practice that isn't used anymore.
2. **Traditional DOM Events Handelers**: [read more about DOM](https://mohammadlebzo.github.io/reading-notes/Class_06)

3. **DOM Level 2 Event listeners**.



