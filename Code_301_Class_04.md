# React

## Forms

1. *What is a ‘Controlled Component’?*

A **controlled component** is a **component** that **works on rendering the form elements** and **controls them by keeping the data in the component's state**.

2. *Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.*

I think that we do need to **wait**, because the user *might* **change their mind about one of the inputs**, so i think it would be better to wait until the user **submits the responses**, to get all the data and **store** it, plus it would be better for the *application*.

3. *How do we target what the user is entering if we have an event handler on an input field?*

We can **target the user input** by using the **value attribute** for the form or the input field.

## The Conditional (Ternary) Operator

1. *Why would we use a ternary operator?*

We **use** the **ternary operator** because it **allows us to assgin one value** to a variable that will **return either true or false**, also because it **makes assigning values to variables easier to see and work with**, because it's all on one line.

2. *Rewrite the following statement using a ternary statement:*

**ex**:
```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

**ternary statement**:

`console.log(x===y ? 'true' : 'false');`
