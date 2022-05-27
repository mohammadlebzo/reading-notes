# JavaScript
## Functions

### Getting a single value out of a function:
In order for us to get a single value out of a function we need to ***return*** it only. **ex**:

```
function calArea(width, height)
{
    let area = width * height;
    return area;
}
let wallOne = calArea(3, 5);
let wallTwo = calArea(8, 5);
```

### Getting multiple values out of a function:
In order for us to get multiple values out of a function we need to ***return*** an **array** of the values. **ex**:

```
function getSize(width, height, depth)
{
    let area = wifth * height;
    let volume = area * depth;
    return [area, volume];
}
let areaOne = getSize(3, 2, 3)[0];
let volumeOne = getSize(3, 2, 3)[1];
```
## Document Object Model(DOM)
The **Document Object Model(DOM)** controls how browsers create **models** of an *HTML* page and how can the Java Script access and update it's content while in a browser window.

**DOM** covers two primary parts:

- **Making a model of the HTML page**:
The **DOM** specifies the way in which browsers should structure the created model of the HTML page in the memory using a **DOM tree**.

A **DOM** is called an object model becuase the **DOM tree** is made out of objects, each one of them represents a differant part of the page loaded in the browser window.

- **Accessing and changing the HTML page**:
The **DOM** defines methods and prperties to access and update each object in the model, which all would be reflected to the user. 

**DOMs** are also called **Application Programming Interface(API)**.

### DOM tree node types:
**There are four node types**:

- **The Document Node**: it represents the entire *HTML* page, when adding any element, attribute or a text node, you navigate to it via the **document node**.

- **Element Nodes**: they are the *HTML* elements that describe the structure of the *HTML* page. **ex**: `<h1> - <h6>, <p>`

- **Attribute Nodes**: they are the attributes that can be carried by the opening tags.

- **Text Nodes**: they are text of the elements.

### Working with the DOM tree:
1. ***Access The Elements***:
    - **Select an Individual Element Node**: there are three ways to do this:
        1. *getElementById()*: uses the value of an element's id attribute.
        2. *querySelector()*: uses a CSS selector and returns the first matching element.
        3. Traversing from one element to another withn the DOM tree. 

    - **Select Multiple Elements(NodeLists)**: there are three ways to do this:
        1. *getElementByClassName()*: selects all elements with the same class name.
        2. *getElementByTagName()*: selectes all elements of the chosen tag.
        3. *querySelectorAll()*: Uses a CSS selector to select all matching elements.

    - **Traversing Between Element Nodes**: you can move through related elements by:
        1. *parentNode*: selects the parent of the current element node.
        2. *previousSibling / nextSibling*: selects the previous or next sibling from the DOM tree.
        3. *firstChild / lastChild*: select the first or last child of the current element.

2. ***Work With Those Elements***:
    - **Access / Update text nodes**:
        1. Select the element.
        2. Use any propety to access it. **ex**: *firstChild*.
        3. Use the property *nodeValue* to access and update the text node.

    - **Work with HTML contant**:
        1. *Accessing child elements and text content*: **innerHTML**. 
        2. *Accessing text content*: **textContent**.
        3. *Create new nodes, add or remove nodes from tree*: **createElement(), createTextNode, appendChild(), removeChild**.  

    - **Access or Update attribute values**: some properities that help with that:
        1. *className / id.*
        2. *hasAttribute()*
        3. *getAttribute()*
        4. *setAttribute()*
        5. *removeAttribute()*



