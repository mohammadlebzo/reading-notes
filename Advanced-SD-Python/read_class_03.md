# Read: class 03

## Reading and Writing Files in Python

**Files** are sets of bytes that contains data. These **Files** are composed of three main parts:

- **Header:** metadata about the file.
- **Data:** contents of the file.
- **End of file (EOF):** special character that indicates the end of the file

### **Opening and Closing a File in Python**:

When you want to open a file in python you need to use the **"open(file path)"** and to close the file you need to use **"close()"**.

Another way to open and close is using the keyword **"with"**, example:

```
with open('test.txt') as reader
```

There are also some modes when opening files, and they are indicated by characters:

|**Character**|**Meaning**|
|---------|-------|
|'r'|The default mode, which is read only|
|'w'|Write only, which is used to overwriting the file contents|
|'b'|Open in binary, you can add 'r' or 'w' before it('rb'/'wb') to read or write in binary mode.|
|'a'|Used to append data to the content of the file|

### **Reading and Writing Methods:**

After opening a file there are some methods we use in order to read from or write in the file, and these are:

**Reading methods**:

|**Method**|**Use**|
|----------|-------|
|.read(5)|If the size is given it will return based on the number of the size reading in bytes, but if there is no size specified then it will return the entire file content|
|.readline(5)|If the size is given it will return based on the number of the size reading in charachters in a line, but if there is no size specified then it will return the content line by line|
|.readlines()|Returns the content of the file line by line as a list|

**Writing methods**:

|**Method**|**Use**|
|----------|-------|
|.write(string)|Writes a string to the file|
|.writelines(seq)|Writes a sequence to the file, and leaves the line endings to the user|

### **Some Key Values When Dealing With Bytes**:

|**Value**|**Meaning**|
|---------|-----------|
|0x89|Means that this is the start of a `PNG`|
|0x50 0x4E 0x47|PNG in ASCII|
|0x0D 0x0A|DOS line ending \r \n|
|0x1A|DOS EOF character|
|0x0A|Unix line ending \n|

<br>

## Exceptions in Python

There are many ways to make an **Exception** in python, so lets look some of them:

- **Raising an Exception**: this can be done by using `raise Exception()`, and adding the message to in between the parentheses.

- **The AssertionError Exception**: can be done by using the `assert()` method, after that you can add a condition and a message, so that if the condition wasn't met where will be a message to throw in the console.

- **The `try` And `except`**: `try` is where the main code goes, and the `except` is where the exception goes if there was an error.


## Things I want to know more about

None.