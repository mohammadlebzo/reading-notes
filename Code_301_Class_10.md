# Reading 10: JavaScript

## Call Stack

1. *What is a ‘call’*?

**Invoking** a *routine* which *consists* of a **name** and **parameters**.

2. *How many ‘calls’ can happen at once*? 

Only *one* at a time, becuase *calls* happen in a **single function(s) execution**, from *top* to *bottom*.

3. *What does LIFO mean*? 

It means **Last in first out**, which means that the **last element** to get into the **stack** is going to be the **first element** to *pop* out of the *stack*.
*
4. *Draw an example of a call stack and the functions that would need to be invoked to generate that call stack*. [source](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```

![Stack Image](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)

5. *What causes a Stack Overflow*? [source](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

**Stack overflow** *occurs* when there is a **recursive function** (a **function that calls itself**) *without* an **exit point**.

## Error Messages

1. *What is a ‘refrence error’*? 

This *error* happens when you try to **use a variable that isn't declared**.

2. *What is a ‘syntax error’*?

This *error* is self explanatory, it happens when you **use the wrong syntax for declaring something or doing something**.

3. *What is a ‘range error’*?

This *error* happens when **trying to manipulate an object** that has a **length** and you gave it an **invalid length** or it **got out the range of the length**.

4. *What is a ‘tyep error’*?

This *error* happens when the **data types are incompatible**.

5. *What is a breakpoint*?

A **breakpoint** is a **debugging tool** that is in the **IDEs**, used to *specify* the *line* that the **program will stop running at(break)**.

6. *What does the word ‘debugger’ do in your code*?

It *specifies* the *line* at which the **program will stop running(break)**.
