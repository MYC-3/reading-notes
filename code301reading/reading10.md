# Memory Storage

## Javascript Call Stack
[All notes were taken from here](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

- What is a ‘call’?
  - A call is a function invocation.
- How many ‘calls’ can happen at once?
  - One at a time from top to bottom.
- What does LIFO mean?
  - LIFO = Last In First Out.
  - The last function to be pushed into the call stack is the first out.
- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
```JavaScript
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

// Output:
// Hello from firstFunction
// The end from secondFunction
```
> 1. When secondFunction() gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
> 2. secondFunction() then calls firstFunction()which is pushed into the stack.
> 3. firstFunction() returns and prints “Hello from firstFunction” to the console.
> 4. firstFunction() is pop off the stack.
> 5. The execution order then move to secondFunction().
> 6. secondFunction() returns and print “The end from secondFunction” to the console.
> 7. secondFunction() is pop off the stack, clearing the memory.
- What causes a Stack Overflow?
  - When a recursive function doesn't have an exit point and the browser's maximum stack call is reached.

## Javascript Error Messages
[All notes were taken from here](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

- What is a ‘refrence error’?
  - When a variable is referenced but not declared.
- What is a ‘syntax error’?
  - When something cannot be parsed in terms of syntax. (Unexpected comma's or punctuation)
- What is a ‘range error’?
  - When you manipulate an object with an invalid length.
  - For example, an array cannot have a negative length.
- What is a ‘type error’?
  - When you try to use or access data types that are incompatible.
- What is a breakpoint?
  - A specific point in the code where the code will stop running.
- What does the word ‘debugger’ do in your code?
  - Adds a breakpoint in your code.

[Back to HOME](../README.md)