# Read: Class 08

## List Comprehensions in Python

The syntax for creating a list comprehension is:

    the_list_name = [ expression for item in list]

**List Comprehension** is a more compact, flexible and faster than other methods of creating, looping and managing lists.

## Some Examples on Creating a List Comprehension

### Creating a list with range() examples:

    ------------------------------------

    numbers = [num for num in range(20)]
    print(numbers)

    ------------------------------------

    squares = [squ**2 for squ in range(20)]
    print(squares)

    ------------------------------------

    multiple_three = [ mult*3 for mult in range(20) ]
    print(multiple_three)

    ------------------------------------

### List comprehensions with condition example:

    even_nums = [ num for num in range(1,20) if num % 2 == 0]

### Parsing a file using list comprehension example:

    file = open("text_file.txt", 'r')
    txt = [ line for line in file ]

    for line in txt:
        print(line)

### Using functions in list comprehensions example:

    def multi(num):
        return x*2

    nums = [multi(num) for num in range(1,20)]
    print(nums)


## Things I want to know more about

- None.