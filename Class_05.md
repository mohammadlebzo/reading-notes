# HTML & CSS

## Images
Using **images** in websites is very important, because some times using an **images** would do the job of lines of text more effectively, and it would give the reader a *visual representation* of the topic.

**Note**: it is ***recommended*** to make a folder for all the used **images** in the website.

### Adding images:
In order to add an **image**, you need to use a `<img>` *tag* that is an empty element, meaning that there is no **closing tag** for the `<img>` *tag*.

The `<img>` *tag* must carry the following two attributes:

- **src**: it tells the browser the source or place of the image file. The source can be either in **another website** or on a **local file** in the website.
- **alt**: it provides a text description of the image if it's not available.
- **title**: it is used to give more information about the image.

Optional `<img>` *tag* values:

- **height**: it specifies the hight of the image.
- **width**: it specifies the width of the image.

### Rules of creating images:
- **Save images in the right format**: mainly websites use jpeg, gif or png formats, because using the wrong format might cause a problem, where images might not look as sharp as it should.

When to use **jpeg**, **png** or **gif**:
1. **jpeg**: it is used when the image contains a natural scene or photograph, where variation is colour and intensity is smooth.

2. **png**: it is used when the image needs transparency, or when the image's with text and objects with sharp contrast edges.

3. **gif**: it is used when there is animations.

- **Save images at the right size**: the images should be saved in the same hight and width that will appear on the website, because we might pace a problem, where the image might get distorted or stretched.

- **Use the correct resolution**: because images are made of pixels we should use the right resolution, because if we use a high resolution image, the image would take longer to load.

## Color
### Foreground color:
In order to add **color** to websites we need to use the **color** property, which can be specified by using the values:
- **RGB values**: it will express colors according to how much **red**, **green** and **blue** are used to make it up.

- **HEX codes**: they are six-digit codes that represent the amount of **red**, **green** and **blue** in color.

- **Color names**: they are the predefined color names that are recognized by the browsers, and they are 147 colors.

**Some properties that change color**:
- **color**: mentioned above.
- **background-color**: it is used to change the background color of the selected element.

## Text
### Typeface Terminology:
- **Serif**:Serif fonts have extra details on the ends of the main strokes of the letters. These details are known as serifs.

- **Sans-Serif**: Sans-serif fonts have straight ends to letters, and therefore have a much cleaner design.

- **Monospace**:Every letter in a monospace (or fixed-width) font is the same width. (Non-monospace fonts have different widths.)

**Values for the chageing the font**:
- ***weight***
    - **Light**: gives a light font.
    - **Medium**: gives a medium font.
    - **Bold**: gives a bold font.
    - **Black**: gives a black font(not in color but in weight).

- ***style***
    - **Normal**
    - **Italic**
    - **Oblique**

- ***stretch***
    - **Condensed**
    - **Regular**
    - **Extended**

 ### Specifying Typefaces:
 **Typefaces** can be specified using the **font-family** *property*, the *value* of the property is the name of the **typeface**.

 **Note**: the property **@font-face** allows you to use a font, even if it's not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.

 ### Changing the size of the text:
 In order to change the size of the text we can use the **font-size** *property*, the value can be in **pixels**, **percentages** and by using **ems**.

 ### Some more text properties:
 - **font-weight**: allows you to change two values:
    - **normal**: text appear in normal weight.
    - **bold**: text appear **bold**.

- **font-style**: allows you to change three values:
    - **normal**: text appear in normal style.
    - **italic**:text appear *italic*.
    - **oblique**:text appear oblique.

- **text-transform**: allows you to change three values:
    - **uppercase**: TEXT APPER IN UPPERCASE.
    - **lowercase**: text appear in lowercase.
    - **capitalize**: Each Word Apper With A Capitalized First Letter.

- **text-decoration**: allows you to change five values:
    - **none**: removes text decoration.
    - **underline**: adds an underline to the text.
    - **overline**: adds a line on top of the text.
    - **line-through**: adds a line through the text.
    - **blink**: animates the text to flash on and off.

- **line-height**: sets the hight of an entire line of text.

- **letter-spacing**: used to set the space size between letters.

- **word-spacing**: used to set the space size between words.

- **text-align**: allows you to change three values:
    - **left**: aligns text to the left.
    - **right**: aligns text to the right.
    - **center**: aligns text to the center.
    - **justify**: indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box.

- **text-indent**: used to indent the first line of text within and element, the values can be **pixels**, and **ems**.


