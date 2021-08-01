# Code in a Content Mnagement System(CMS):

What is a **content management system**?

A *content management system* is a software application that contains a variety of tools that allows the user to create, modify, manage and deliver digital content.

When talking about the structure of the **CMS**, there are typically two major parts to it:
- **Content Management Application(CMA)**, which represents the front-end user interface to allow users with any level of experience, to add, modify or remove content without needing a webmaster.

- **Content Delivery Application(CDA)**, which compiles content and updates the website.

These kind of softwares gives users so many options, one of them is the option to modify the code that it's righting for you which will give users with higher experience level more room to do things faster and as they want.

# HTML Tags, Structural and Semantic Markup:

- ***Structural markup***: elements used to describe headings and paragraphs.

- ***Semantic markup***: elements that provide extra information, such as, emphasis, quoting, the meaning of acronyms, etc....

### Headings:

|Heading|Effect|
|-------|------|
|`<h1>`|The biggest title size|
|`<h2>`|Smaller than `<h1>`|
|`<h3>`|Smaller than `<h2>`|
|`<h4>`|Smaller than `<h3>`|
|`<h5>`|Smaller than `<h4>`|
|`<h6>`|The Smallest title size|

- **Examples**:

`<h1>Header</h1>`

# Header

`<h6>Header</h6>`

###### Header

### Paragraphs:
The tag `<p>` is used to write a paragraph.

`<p>This is a paragraph</p>`

When writing paragraphs the tag `<b>` to make the text **bold**, and the tag `<i>` is used to make the text *italic*.

`<p><b>This</b> is a <i>paragraph</i></p>`

***Note***: White spaces in paragraph make no effect on the rendered text.

Also you can use `<br>` tag to break text lines, and the `<hr>` tag to make lines to separate text.

```
    <p>
        Words 
        <br>
        <hr>
        words
    </p>
```

### Semantic Markup:

The tag `<Strong>` can be used to indicate the importance of the contant, there is also `<em>` that is used to emmphasis on the contant.

```
<p><strong>Beware:</strong> Pickpockets operate in
 this area.</p>

 <p>I <em>think</em> Ivy was the first.</p>
```

# Forms:

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

# Basic JavaScript Instructions:

- ***JavaScript*** is case sensitive. 

- ***Statements*** are instructions or steps that end in a semicolon.

- ***Comments*** are non-executable text in the code used for explaining.

- ***Variables*** are a place that values get stored in, you can view it as a box that you store your valuables in for later use.

### Declaring Variables and Assigning Values to Them:
**Declaring** variables can be done in two ways:

- var varName;
- let varName;

**Assigning** values to variables can be done like this:
There are many data types such as **Strings**, **Numbers** and **Booleans**.

- Assigning a **String**:

`var firstName = 'Joe';` or `let firstName = 'Joe';`

- Assigning a **Number**:

`var teamNum = 7;` or `let teamNum = 7;`

- Assigning a **Boolean**:

`var isGood = false;` ore `let isBad = true;`

There is no need for redeclaring a variable to change it's value you can just referance it and change it's value, like this:

`firstName = 'mike';`

### Arrays:
**Arrays** are a kind of variable where you can store a list of variables you can view it as the truck that stores your valuable boxes(**variables**).

**Creating an Array**:

`let colors = [blue, pink, black, orange, red, yellow]`










