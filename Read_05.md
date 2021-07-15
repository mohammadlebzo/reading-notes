# Expressions, operators and loops:

### ***Operator precedence***:
The precedence of operators determines the order they are applied when evaluating an expression. You can override operator precedence by using parentheses.

The following table describes the precedence of operators, from highest to lowest.


|**Operator type** | **Individual operators** |
|---------|------------------------|
|member|. []|
|call / create instance|() new|
|negation/increment|! ~ - + ++ -- typeof void delete|
|multiply/divide|	* / %|
|addition/subtraction|	+ -|
|bitwise shift|	<< >> >>>|
|relational|< <= > >= in instanceof|
|equality|== != === !==|
|bitwise-and|&|
|bitwise-xor|	^|
|bitwise-or|`|`|
|logical-and| 	&&|
|logical-or|`||`|
|conditional|?:|
|assignment|`= += -= *= /= %= <<= >>= >>>= &= ^= |= &&= ||= ??=`|
|comma|,|
<br>

### **Operators examples:**
I will only be listing the ***assignment operators*** and the ***comparison operators***.

* **Assignment Operators**:

|**Name** | **Shorthand operator** | **Meaning**|
|---------|------------------------|---------------------|
|Assignment|	x = y | 	x = y |
|Addition assignment| 	x += y | 	x = x + y |
|Subtraction assignment| x -= y | 	x = x - y |
|Multiplication assignment| 	x *= y | 	x = x * y |
|Division assignment| 	x /= y | 	x = x / y |
|Remainder assignment| 	x %= y | 	x = x % y |
|Exponentiation assignment| 	x **= y | 	x = x ** y |
|Left shift assignment| 	x <<= y | 	x = x << y |
|Right shift assignment| x >>= y | x = x >> y |
|Unsigned right shift assignment| x >>>= y | 	x = x >>> y|
| Bitwise AND assignment| 	x &= y | 	x = x & y |
|Bitwise XOR assignment| x ^= y | x = x ^ y|
|Bitwise OR assignment| `	x |= y`|`x = x | y`
|Logical AND assignment| 	x &&= y | x && (x = y)|
|Logical OR assignment| `	x ||= y` | `x || (x = y)`|
|Logical nullish assignment| x ??= y | 	x ?? (x = y) |
<br>

* **Comparison operators**:

|**Operator** | **Description** | **Examples returning true**|
|---------|------------------------|------------|
|Equal (==)| Returns true if the operands are equal.|3 == var1, "3" == var1 / 3 == '3'|
|Not equal (!=)|Returns true if the operands are not equal.|var1 != 4 / var2 != "3"|
|Strict equal (===)|Returns true if the operands are equal and of the same type.|3 === var1|
|Strict not equal (!==)|Returns true if the operands are of the same type but not equal, or are of different type.|var1 !== "3" / 3 !== '3'|
|Greater than (>)|Returns true if the left operand is greater than the right operand.|var2 > var1, "12" > 2|
|Greater than or equal (>=)|Returns true if the left operand is greater than or equal to the right operand.|var2 >= var1, var1 >= 3|
|Less than (<)|Returns true if the left operand is less than the right operand.|var1 < var2, "2" < 12|
|Less than or equal (<=)|Returns true if the left operand is less than or equal to the right operand.|var1 <= var2, var2 <= 5|

------------------

### ***Loops***:
**Loops** offer a quick and easy way to do something repeatedly.

There are many different kinds of loops, but they all essentially do the same thing: *repeating actions for a specific number of times*.

**The statements for loops provided in JavaScript are:**
* for statement
* do...while statement
* while statement
* labeled statement
* break statement
* continue statement
* for...in statement
* for...of statement

Im going to briefly touch on **for** and **while** loops.

### **Loops statements and Examples**:
A **for** statement looks as follows:
```
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```

***A while statement executes its statements as long as a specified condition evaluates to true.***<br> A **while** statement looks as follows:
```
while (condition)
  statement
```
**Examples**:

```
for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}
```

```
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```
