# HTML & CSS

### Adding author details:
- `<address>` **Tag**: this element is specifically used to contain the author's contact information.

### Changing inline contant:
- `<ins>` **tag**: shows inserted content, 
**ex**: `<p>This is the <ins>best</ins> game i played</p>`

 **res**: This is the <ins>best</ins> game i played
- `<del>` **tag**: shows deleted contant, 
**ex**: `<p>This is the <del>worst</del> best movie i've seen</p>`

**res**: This is the <del>worst</del> best movie i've seen
- `<s>` **tag**: indicates elements that is no longer relevent or accurate, **ex**:

```
    <p>Laptop computer:</p>
    <p><s>Was $995</s></p>
    <p>Now only $375</p>
```
**res**:

Laptop computer:
<s>Was $995</s>
Now only $375

## Lists

|List Type|Indicator Tag|Element Tag(s)|
|---------|-------------|--------------|
|Ordered|`<ol>`|`<il>`|
|Unordered|`<ul>`|`<il>`|
|Definition|`<ol>`|`<dt>`, `<dd>`|

**Notes**:
1. After uesing the definition indicator we use the `<dt>` *tag* to specify the **term** that will be defined(**title of the definition**), after that the `<dd>` *tag* is used and closed to write a definition(**element**).
2. There is also a **list type** called ***Nested List***, which is just a mix of the previous types.

**Examples**:

- **Ordered List**:

```
<ol>
    <li>1st Element</li>
    <li>2nd Element</li>
    <li>3rd Element</li>
    <li>4th Element</li>
</ol>
```
**res**:

1. 1st Element
2. 2nd Element
3. 3rd Element
4. 4th Element

- **Unordered List**:

```
<ul>
    <li>1st Element</li>
    <li>2nd Element</li>
    <li>3rd Element</li>
    <li>4th Element</li>
</ul>
```

**res**:

- 1st Element
- 2nd Element
- 3rd Element
- 4th Element

- **Definition List**:

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
## Boxes

### Box dimensions(width, height):
The **box size** of the element depends on the content of it by **default**, in order for us to be able to change the size, we need to change the **hight** and **width** properties. 

You can change the **width** and **hight** by using:
- Pixels. ex: `p{width: 110px};`
- Percentages. ex: `h1{hight: 40%};`

*Sizing with percentages is flexible because it depends on the screen size*

- Limiting width using **min-width / max-width**:

ex: `p{min-width: 350px; max-width: 605px};`

- Limiting hight using **min-hight / max-hight**:

ex: `p{min-hight: 350px; max-hight: 605px};`

### Overflowing content:
The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
- **hidden**: hides extra contant that does't fit in the box.
- **scroll**: allows the user to scroll down to see the hidden content.

### Border, Margin and Padding:
![BMP](https://s1.o7planning.com/en/12495/images/51081143.gif)

- **Border**: separates the edges of boxes.
- **Margin**: is outside the edge of the border.
- **Padding**: the space between the border and the content.

Each of these can be increased in size, whether it is in a specific direction of from all of them, also they can be colored.

### Changing inline / block:
Using the ***display*** property we can turn inline element into a block-level element and vice versa, also we can hide elements from pages.

The ***display*** property can take the valus:
- **inline**: it makes a block-level element to act like an inline element.
- **block**: it makes an inline element act like a block-level element.
- **inline-block**: it makes a block-level element to flow like an inline element, while sustainable some of its features.
- **none**: it hides elements in the page, and it acts like it's not on the page at all.

### Hiding boxes:
To hide and show boxes there is a property called ***visibility***, when it's used to hide boxes, the place of the contant remain empty.

The values of the ***visibility*** property:
- **hidden**: hides the element.
- **visible**: shows the element.

# JavaScript(Decisions & Loops)

### Logical operators:
**Comparison operators** are used to return a single value of **true** or **false**.
**Logical operators** are used to compare the results of more than one **comparison operator**.

The ***logical operators***:
- **&& (logical AND)**: always returns false, except when both conditions happen.

- **|| (logical OR)**: always returns ture, except when neither of the conditions happen.

- **! (logical NOT)**: takes a boolean value and inverse it.

### If Statements:
**If statements** are used to check or evaluate conditions, if it's ture code executes otherwise it doesn't. **ex**: `if(ture){let i = 0;}`

There is also **if...else statements**, the only difference is that if it's false the code jumps to the next block.

### Switch statement:
A **switch statement** takes first a switch value, which decides if the code will execute or continue, then comes the cases, which is the code that needs to be executed. **ex**:

```
    switch (level) 
    {
        case 'One ':
        title = 'Level 1 ';
        break;
        case 'Two':
        tit 1 e = ' Level 2 ';
        break;
        case ' Three':
        title = 'Level 3';
        break;
        default:
        title = 'Test';
        break;
    }
```

### Loops:
**Loops** checks a condition set by the user, if it's *true* the code runs and the ***condition will be checked again afterwords***, if it's *false* the code doesn't run.

**Loop types**:
- For
- While
- Do While

