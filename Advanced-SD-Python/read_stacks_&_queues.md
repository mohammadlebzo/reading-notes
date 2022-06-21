# Read: Stacks & Queues

## Stacks

### Some basic information about stacks:

- A stack is a data structure that consist of nodes that hold values and point to the next one in line.
- Stacks follow the following concepts:
    - **FILO**(First In Last Out), Which means that the first element added will be the last to be *popped*.
    - **LIFO**(Last In First Out), which means that the last added element will be the first to be *popped*.

As you just saw I used the term **"popped"**, what does that mean?

In order to understand what does that mean, **lets list some common terminologies for stack**:

|**Term**|**Meaning**|
|--------|-----------|
|*Push*|add an element to stack|
|*Pop*|remove an element to stack, popping an empty stack will return an exception|
|*Top*|Points to the top of the stack|
|*Peek*|View the top node of the stack, peeking an empty stack will return an exception|
|*isEmpty*|Return true if empty|

## Queues

### Some basic information about queues:

- A queue is a data structure that consist of nodes that hold values and point to the next one in line.
- Queues follow the concept of **FIFO**(First In First Out), Which means that the first element in added will be the first to be **dequeued**.

And as you saw I used the term **"dequeued"** here for queues, which means that, just like stacks there are some common terms we need to know, which are the following:

|**Term**|**Meaning**|
|--------|-----------|
|*Enqueue*|Add an element to queue|
|*Dequeue*|Remove an element to queue, dequeuing an empty queue will return an exception|
|*Front*|point to the first node|
|*Rear*|point to the last point|
|*Peek*|view the value of the front node, peeking an empty queue will return an exception|
|*IsEmpty*|Return true if empty|


***Note***: **Each of the stack terms and the queue terms represent a method of the of it's data structure methods, and each of them have a time and space complexity of** ***O(1)***.

## Things I want to know more about

- None.
