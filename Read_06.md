# CSS: definition and examples
**CSS (Cascading Style Sheets)** is a language for specifying how documents are presented to users — how they are styled, laid out, etc.

**CSS** can be used for very basic document text styling — for example changing the **color** and **size of headings** and **links**, also it can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as **animation**.

## CSS syntax

* ### External CSS
```
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="style.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
**"style.css"**
```
body 
{
  background-color: lightblue;
}

h1 
{
    color: red;
    font-size: 5em;
}

p 
{
    color: black;
}
```

* ### Internal CSS
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

* ### Inline CSS
```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```
