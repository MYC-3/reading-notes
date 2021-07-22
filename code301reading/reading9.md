# Reading 9 - Functional Programming

## Functional Programming Concepts
[All notes were taken from here](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

1. What is functional programming?
> Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
2. What is a pure function and how do we know if something is a pure function?
  - If a function is given the same arguments it will return the same results
  - It does not cause any visible side affects
3. What are the benefits of a pure function?
  - Pure functions are easier to test.
4. What is immutability?
  - Cannot be changed once it has been assigned.
5. What is Referential transparency?
>if a function consistently yields the same result for the same input, it is referentially transparent.
```
pure functions + immutable data = referential transparency
```

[This video was used to answer the following questions](https://www.youtube.com/watch?v=xHLd36QoS4k)

1. What is a module?
  - A separate file that holds a chunk of code meant to do one function.
  - Separating your app into modules makes it cleaner and easier to understand for yourself and other programmers.
2. What does the word ‘require’ do?
  - Imports another file to use in your current app.
3. How do we bring another module into the file the we are working in?
  - `require('PathwayToModuleFile')` in your main app
4. What do we have to do to make a module available?
  - `module.exports = NameOfModule` in your module file.

[Back to HOME](../README.md)