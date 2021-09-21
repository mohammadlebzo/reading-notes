# Reading 09

## Functional Programming Concepts

1. *What is functional programming*? [source 1](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)[source 2](https://en.wikipedia.org/wiki/Functional_programming)

**Functional programming** is a **programming paradigm** — a style of building the *structure* and *elements* of **computer programs** — that treats *computation* as the *evaluation* of **mathematical functions** and *avoids* **changing-state** and **mutable data**.

2. *What is a pure function and how do we know if something is a pure function*?

A **pure function** is one of the *fundamental concepts* of **functional programming**, and we can know if the function is *pure* when:

- It *returns* the **same result** if given the **same arguments**.
- It does not *cause* any observable **side effects**.

3. *What are the benefits of a pure function*?

- **Immediatly testable**.
- **Easier maintaining, refactoring, and testing**.
- **No need for mocking anything**.

4. *What is immutability*?

**Immutability** means that it can't be changed (unchangeable)

5. *What is Referential transparency*? [source](https://en.wikipedia.org/wiki/Referential_transparency)

**Referential transparency** and *referential opacity* are *properties* of *parts* of **computer programs**. An *expression* is called **referentially transparent** if it can be *replaced* with its corresponding value (and vice-versa) without changing the program's behavior. (**pure** *+* **immutability** *=* **referential transparency**)

## Node JS: Modules and require()

1. *What is a module*? 

**Modules** in **Node.js** are a *set of functionalities* that can be *called* whenever are needed.

2. *What does the word ‘require’ do*? 

It **imports** the *data* from a **module**, *given* it's **path**.

3. *How do we bring another module into the file the we are working in*? 

We can do that by *using* the word **require** and give it the *path* of the **module**.

4. *What do we have to do to make a module available*? 

We can fo that by using `module.exports = what ever we want to make available`. Like that we can export the data which we want to make available.

## Things I want to know more about

None.
