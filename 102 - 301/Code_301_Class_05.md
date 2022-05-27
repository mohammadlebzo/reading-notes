# React

## Thinking in React

1. *How would you break a mock into a component heirarchy?*

In order to **breack a mock into a component heirarchy**, you need to first know what **needs to be a component** what **needs to a part of a component**. To do that you need to *think of creating components like you think of creating functions*, you need to use the **single reponsibility principle**.

2. *What is the single responsibility principle and how does it apply to components?*

It is that each **component should be responsible of one thing and one thing only**.

3. *What does it mean to build a ‘static’ version of your application?*

Building a ***static version*** of your application means **building a version of your app that only renders your data using props**. And in this version there will be **no interactivity meaning there will be no state**.

4. *Once you have a static application, what do you need to add?*

Once we have a ***static application*** we need to **start adding interactivity**, but first we need to **identify the minimal set of mutable state that the app needs**.

5. *What are the three questions you can ask to determine if something is state?* [source](https://reactjs.org/docs/thinking-in-react.html)

- **Is it passed in from a parent via props**? If so, *it probably isn’t state*.

- **Does it remain unchanged over time**? If so, *it probably isn’t state*.

- **Can you compute it based on any other state or props in your component**? If so, *it isn’t state*.

6. *How can you identify where state needs to live?*

*In order to determine where the state needs to live, we need to*:

- **Identify every component that renders something based on that state**.

- **Find a common owner component (a single component above all the components that need the state in the hierarchy)**.

- **Either the common owner or another component higher up in the hierarchy should own the state.**

- **If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component**.

## Higher-Order Functions

1. What is a **“higher-order function”**? [source](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

A **higher-order functions** is a *functions* that operate on other *functions*, either by taking them as an **arguments** or by **returning them**.

2. Explore the **greaterThan** function as defined in the reading. In your own words, what is line 2 of this function doing?

In **line 2** the function is **returning an arrow function that compares** the **arrow function passed variable 'm'** to the **main function passed variable 'n'**.

3. Explain how either **map** or **reduce** operates, with regards to higher-order functions.

**Reduce function** takes 3 parameters, an array, a function, and a starting point, in this example the array is [1, 2, 3, 4] and the function works on taking the starting point and each element from the array and combine them together, then returns it to the starting point again to change it. All of this means that this reduce function takes an array and a starting point and makes some operations on them using the passed function.

*ex*: [source](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

```
function reduce(array, combine, start) {
  let current = start;
  for (let element of array) {
    current = combine(current, element);
  }
  return current;
}

console.log(reduce([1, 2, 3, 4], (a, b) => a + b, 0));
// → 10
```

## Things I want to know more about

None.
