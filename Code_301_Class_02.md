# React

## React lifecycle

**What happens first, the ‘render’ or the ‘componentDidMount’?** Render happens first.

**What is the very first thing to happen in the lifecycle of React?**

The first thing is **mounting**, which happens when an instance of a component is being created and inserted into the DOM. And there is a sequance of operations will happen in the mounting phase, this secuance goes like this: constructor, static, getDerivedStateFormProps, render, componentDidMount then finally UNSAFE_componentWillMount.

**Put the following things in the order that they happen**: ***componentDidMount***, ***render***, ***constructor***, ***componentWillUnmount***, ***React Updates***

1. constructor.

2. render.

3. componentDidMount

4. React Updates

5. componentWillUnmount.

**What does componentDidMount do?**

**componentDidMount** is used to lead anything using a network request or initialize the DOM [source](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093).

## React State Vs Props

**What types of things can you pass in the props?**

We can pass values of any data type to propes.

**What is the big difference between props and state?**

The big difference between them is that **props** are things that are ***passed into*** a component (***handeled outside***) but **state** is a thing that is ***handeled inside*** of a component.

**When do we re-render our application?**

We re-render our application when we change the state of it.

**What are some examples of things that we could store in state?**

We store changes in state meaning that when a user entered values or changed a value, it will be stored in a state, so that the application can re-render with the new values.

## Things I want to know more about

- *React-Bootstrap*
