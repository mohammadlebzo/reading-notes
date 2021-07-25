# Expressions, Operators and Functions:
### Control Flow:

Before talking about any of the above we need to understand how does JavaScript read codelines.<br>
The **control flow** is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

### Expressions:
**Expressions** are any valid unit of code that resolves to a value.<br>

There are two types of expressions, the expression **x = 7** is an example of the ***first type***. This expression uses the **= operator** to assign the value seven to the variable x. The expression itself evaluates to seven.
<br>
**To learn more about operators visit**: [Read_05](https://mohammadlebzo.github.io/reading-notes/Read_05)

The code **3 + 4** is an example of the second expression type. This expression uses the **+ operator** to add three and four together without assigning the result, seven, to a variable.

**JavaScript has the following expression categories**:

- **Arithmetic**: evaluates to a number, for example 3.14159.
- **String**: evaluates to a character string, for example, "Fred" or "234".
- **Logical**: evaluates to true or false.
- **Primary expressions**: Basic keywords and general expressions in JavaScript.
- **Left-hand-side expressions**: Left values are the destination of an assignment.

#### ***Primary Expressions***:
- **"this"** keyword is used to refer to the current object. In general, this refers to the calling object in a method. Use this either with the dot or the bracket notation:
```
this['propertyName']
this.propertyName

```

- **Grouping operator**:
The grouping operator ( ) controls the precedence of evaluation in expressions. For example, you can override multiplication and division first, then addition and subtraction to evaluate addition first.

```
var a = 1;
var b = 2;
var c = 3;

// default precedence
a + b * c     // 7
// evaluated by default like this
a + (b * c)   // 7

// now overriding precedence
// addition before multiplication
(a + b) * c   // 9

// which is equivalent to
a * c + b * c // 9
```

#### ***Left-hand-side expressions***:
Left values are the destination of an assignment.

- **new** operator:
You can use the new operator to create an instance of a user-defined object type or of one of the built-in object types. Use new as follows:
```
var objectName = new objectType([param1, param2, ..., paramN]);
```

- **super** keyword:
The super keyword is used to call functions on an object's parent. It is useful with classes to call the parent constructor, for example.
```
super([arguments]); // calls the parent constructor.
super.functionOnParent([arguments]);
```

### Functions:
**Functions** are one of the ***fundamental building blocks in JavaScript***.<br> A **function** in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

#### ***Defining functions***:>>

**Function declarations**:
A function declaration consists of the function keyword, followed by:
- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

**Example**:
```
function square(number) {
  return number * number;
}
```

#### ***Calling functions***:>>
Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:
```
square(5);
```
The preceding statement calls the function with an argument of 5. The function executes its statements and returns the value 25.
