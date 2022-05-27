# JavaScript
## Error Handling & Debugging

The **JavaScript interpreter** uses the concept of ***execution contexts***, which include three contexts that correspond to variable scope. 

- ***Execution Context***:
    - **Global Context**: statements that are not inside a function.
    - **Function Context**: statements that are inside a function.
    - **Eval Context(Not Shown)**: text that is executed in an internal function.

- ***Variable Scope***: first two contexts work with the notion of scope:
    - **Global Scope**: when variables are not inside a function they can be used anywhere in the code because they are in the globle scope.

    - **Function-Level Scope**: When variables are inside a function they can only be used in that function because it has a function-level scope.

***Each time a script enters a new execution context, there are two phases of activity***:

1. **Prepare**: 
    - New scope is created.
    - Variables, functions and arguments are created.
    - The value of `this` keyword is determined.

2. **Execute**: 
    - Assigning values to variables.
    - Reference functions and run them.
    - Execute statments.

***Functions in javascript are said to have lexical scope.***. They are linked to the object they were defined within. So,  each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object. 

### Error Objects: 
**Error objects** are used to help understand where the mistakes are, and they contain the following properties:

|Property|Description|
|--------|-----------|
|name|Type of execution|
|message|Description|
|fileNumber|Name of the JavaScript file|
|lineNumber|Line number of error|

**There are seven types of built-in error objects in javascript**: 

|Object|Description|
|------|-----------|
|Error|Generic error, which is the error that all other are based on|
|SyntaxError|Syntax has not been followed|
|ReferenceError|Tried to reference an undeclared variable within the scope|
|TypeError|An unexpected data type that cannot be coerced|
|RangeError|Number not in acceptable range|
|URIError|encodeURI(), decodeURI() and similar methods used incorrectly|
|EvalError|eval() function used incorrectly|

### Dealing With Errors:
There are two things need to be done to handle **errors**:

1. **Debuging the script to fix errors**: this can be done by tracking down the source of the error and fixing it.
2. **Handling errors gracefully**: this can be done using `try`, `catch`, `throw` and `finally` statements.

**Note**: errors can be monitored using the console tool that is available in all modern browsers.

**Note**: errors can be also handled using **breakpoints**.