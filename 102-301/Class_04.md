# HTML & CSS

## Lists

### Definition lists:
To able to use a **definition list**:
- We need to start with an `<dl>` *tag* as an indicator that we are using a definition list
- Then we should use the `<dt>` *tag* to specify the **term** that will be defined(**title of the definition**)
- After that the `<dd>` *tag* is used and closed to write a definition(**element**).

ex:

```
<dl>
    <dt>1st Definition Name</dt>
    <dd>
        The Definition 
    </dd>
    <dt>2nd Definition Name</dt>
    <dd>
        The Definition 
    </dd>
    <dt>3rd Definition Name</dt>
    <dd>
        The Definition 
    </dd>
</dl>
```
**res**:

<dl>
    <dt>1st Definition Name</dt>
    <dd>
        The Definition 
    </dd>
    <dt>2nd Definition Name</dt>
    <dd>
        The Definition 
    </dd>
    <dt>3rd Definition Name</dt>
    <dd>
        The Definition 
    </dd>
</dl>

### Nested lists:
A **nested list** is a mix of previous types of lists. ex:

```
<ol>
    <li>1st Ordered Element
        <ul>
            <li>1st Unordered Element</li>
            <li>2nd Unordered Element</li>
            <li>3rd Unordered Element</li>
            <li>4th Unordered Element</li>
        </ul>
    </li>
    <li>2nd Ordered Element</li>
    <li>3rd Ordered Element</li>
    <li>4th Ordered Element
        <ul>
            <li>1st Unordered Element</li>
            <li>2nd Unordered Element</li>
            <li>3rd Unordered Element</li>
            <li>4th Unordered Element</li>
        </ul>
    </li>
</ol>
```
res:

1. 1st Ordered Element
    - 1st Unordered Element
    - 2nd Unordered Element
    - 3rd Unordered Element
    - 4th Unordered Element
2. 2nd Ordered Element
3. 3rd Ordered Element
4. 4th Ordered Element
    - 1st Unordered Element
    - 2nd Unordered Element
    - 3rd Unordered Element
    - 4th Unordered Element

## Links

**Links** are the defining feature of the web, which is going from one page or a website to another, enabling the very idea of browsing or surfing.

### Writing links:
To be able to create a link in a website we need to use the `<a>` *tag* and close it. ex:

`<a href = "http://www.example.com" target = "_blank">example</a>`

**res**:

[Cockatiel image](https://images.saymedia-content.com/.image/t_share/MTc0OTY3NzI5NDMzMDkzNTcy/information-on-the-cockatiel-and-cockatiels.jpg)

<ins>Notes</ins>: 

1. The text that is between the opening and closing tags is called the **link text**.
2. You can open a link in a new window using the keyword **target** with the value **"_blank"** inside of the opening tage.

## Layout

### Key concepts in positioning elements:
**Bulding blocks**:

When using **CSS** each **HTML** element is treated as if it has it's own box, and this box is either a **block-level box** or an **inline box**.
- **Block-Level Element**: These elements start on a new line. ex: `<p>, <h1>`

- **Inline Element**: These elements flow between surrounding text. ex: `<img>, <b>`

### Controlling the position of elements:
**CSS** has some **positioning schemes** that allows us to control the layout of the page these *schemes* are:
- **Normal Flow**
- **Relative Positioning**
- **Absolute Positioning**

These *schemes* can be specified using the **position** property, or use the **float** property to float elements.

1. **Normal Flow(position: static)**:

**Normal Flow** is the default formatting of the HTML elements, where each block-level element sets on top of the next one.

2. **Relative Positioning(position: relative)**:

When using the **relative positioning**, **CSS** layouts the elements where they should have been in **normal flow**, meaning that if you have moved an element to the top, bottom, left or right(because **relative positioning** allows you to do that), the element will be where it would be in **normal flow**.

3. **Absolute Positioning(position:absolute)**:

When using the **absolute positioning**, the element is taken out of the **normal flow** and no longer affects other elements.

4. **Fixed Positioning(position: fixed)**:

When using **fixed positioning**, the element takes place in relation to the browser, meaning if the user scroll down, the element stays in the same exact place.

### Floating Elements(float):
Using the **float** property allows you to take an element from the **noraml flow** and and place it as far to the left or right of the containing element.

**clear property**: this property is used to prevent elements from touching the left or right sides of the box.

**clear property's values**:
- **left**: it prevents elements from touching to the left.
- **right**:it prevents elements from touching to the right.
- **both**:it prevents elements from touching to the left or right.
- **none**: elements can touch either sides.

### Page Sizes: 
When thinking about the appropriate size for the page you should think of using either **Fixed Width Layouts** or **Liquid Layouts**, but you also need to think in their advantages and disadvantages.

- **Fixed Width Layouts**: it allows designs without a changing size according to the screen size.

|Advantages|Disadvantages|
|----------|-------------|
|Pixel values are accurate at controlling size and positioning of elements.|You can end up with big gaps around the edge of a page.|
|The designer has far greater control over the appearance and position of items on the page than with liquid layouts.|If a user increases font sizes, text might not fit into the allotted spaces|
|You can control the lengths of lines of text regardless of the size of the user's window.|If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read.|

- **Liquid Layouts**:it allows designs with a changing size according to the screen size.

|Advantages|Disadvantages|
|----------|-------------|
|Pages expand to fill the entire browser window so there are no spaces around the page on a large screen.|If the user has a wide window, lines of text can become very long, which makes them harder to read.|
|If the user has a small window, the page can contract to fit it without the user having to scroll to the side.|If the user has a very narrow window, words may be squashed and you can end up with few words on each line.|
|The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch).|If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together.|

# JavaScript(Functions, Methods and Objects)

1. **Finctions & Methods**: they are a group of statements that perform a specofoc task, except that methods are created inside objects.

2. **Objects**: they are elements that are created from properties and methods.

3. **Built-In Objects**: they are the objects that come with the browser that act like a toolkit for the user to benefit from.

### Declaring and Calling Functions:
- **Declaring a function**:

```
function takeInput()
{
    let input = prompt('Give input');
    console.log(input);
}
```
- **Calling a function**: `takeInput();`

