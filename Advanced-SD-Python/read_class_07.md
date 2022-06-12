# Read: Class 07

## Python Scope

### ***What is Python Scope***

In programming, to access a variable or a function you should be within it's scope or space, it is a place where it is known as a variable or a function, it's a grate way to avoid name collisions.

### ***Using the LEGB Rule for Python Scope***

The letters stand for **Local**, **Enclosing**, **Global**, and **Built-in**, which are the python scope for names, but I will currently only be focussing on the **Local** and **Global**.

- **Local/function scope**: this is the body of any python function, where all the variables defined within it are only access by that scope.

**Note**: this scope is created at function call.

example on local scope:

```
def function_local():
    x = 1
    y = 3
    return x + y

function_local()
```

- **Global/module scope**: this is the top-level scope, anything defined in this scope can be access in any other scope. 

The moment a python project is started the programmer will be at the **global scope** so anything that is not inside a class or a function is considered in the **global scope**.

example:

```
names_list = ['x', 'y', 'z']  # this is a global variable
def funcation():
    # doing somthing

funcation()
```

### ***Modifying the Behavior of a Python Scope***



## Things I want to know more about

None.