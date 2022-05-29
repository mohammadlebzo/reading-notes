# React

## Lists and keys

1. *What does **.map()** return?* ***.map()* returns a new array.**

2. *If I want to **loop through** an array and display each value in JSX, how do I do that in **React**?*

**Ex** on displaying each element in react using **map() javascript function**: (*ex* [source](https://reactjs.org/docs/lists-and-keys.html))

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);

ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
```

3. *Each list item needs a unique ____.*

**Each list item needs a unique key.**

4. *What is the purpose of a key?*

**Keys** are used by **React** to **identify changed, added or remobed items**.

## The Spread Operator

1. *What is the spread operator?*

It's an operator that is used for adding items to arrays, combining arrays or objects, and spreading an array out into a function's arguments. [source](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

2. *List 4 things that the spread operator can do.* [source](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

- Copying an array.

- Combining arrays.

- Using an array as a function.

- Adding an item to a list.

3. *Give an example of using the spread operator to combine two arrays.*

```
const array1 = ['a',`ab`,`abc`]
const array2 = [`d`,`de`,`def`]
const arrayconcat = [...array1,...array2]
console.log(...arrayconcat) 
```

4. *Give an example of using the spread operator to add a new item to an array.*

```
const names = ['nathan', 'ahmad', 'john'];
const moreNames = ['mike', ...names];
console.log(moreNames);
```

5. *Give an example of using the spread operator to combine two objects into one.*

```
const objectOne = {p1: 'Hello Im object 1'};
const objectTwo = {p2: 'Hellow Im object 2'};
const objectThree = {...objectOne, ...objectTwo, p3: 'Hellow Im object 3'};
console.log(objectThree);
const objectFour = {...objectOne, ...objectTwo, p4: () => {console.log("Hellow Im object 4".repeat(5))}};
objectFour.p4();
```

## Passing Functions Between Components

1. *In the video, what is the first step that the developer does to pass functions between components?*

He used the **map() function** to loop over the array of objects.

2. *In your own words, what does the **increment** function do?*

This function **loops over the array of objects** to **find the passed name** to be able to **update/increment the count**.

3. *How can you pass a method from a parent component into a child component?*

In order to **pass a method** from a **parent** to a **child** you basically need to use **props**.

4. *How does the child component invoke a method that was passed to it from a parent component?*

The **child** can **invoke** a **method** that was **passed to it from the parent** by **making a prop out of it** and then **using the prop to access the method and invoke it**. **ex**: `this.props.methodName();`

## Things I want to know more about

**None**.
