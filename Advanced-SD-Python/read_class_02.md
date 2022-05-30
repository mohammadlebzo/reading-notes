# Read: class 02

### **TDD - Test-Driven Development**
<br>

**Test-Driven Development** or **TDD** has couple of steps
1- Write a test for the thing you want to achieve.
2- Write the function that would pass the test you just wrote. 
3- Refactor your code to make it better.

You might say, wait! are we going to write the test before making the function ?

Well yes, when we make the test before the function we are forced to think about the design and structure of the software, which would really inhace it.

<br>

### **What does the if \_\_name\_\_ == “\_\_main\_\_”: do?**
<br>

First what does **\_\_name\_\_ == “\_\_main\_\_”** mean ?
It means that whenever the python interpreter runs a module it sets __name__ to __main__ indicating that its the main module, but if a module was imported into another module, the interpreter will set it's __name__ variable to the module name to indicate that this module is not the main one, but is used in the main one.

So what ever is inside the **if statement** will only execute if the module is the "main" module.

<br>

### **Recursion**
<br>

**Recursion** is the process where a function keeps iterating until the base case is met, through calling it self over and over again.

Recursion example: [source](https://www.geeksforgeeks.org/recursion/)

```
    def printFun(test):
 
        if (test < 1):
            return
        else:
    
            print(test, end=" ")
            printFun(test-1)  # statement 2
            print(test, end=" ")
            return
            
 
    # Driver Code
    test = 3
    printFun(test)
```


## Things I want to know more about

None.