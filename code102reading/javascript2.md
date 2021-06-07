# Reading 7 - Programming with Javascript

## JavaScript Operators

List of Operators:
- Assignment operators
- Comparison operators
- Arithmetic operators
- Bitwise operators
- Logical operators
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators

## Functions

Functions are a set of statements in JavaScript that can be used to perform a task. In more basic terms, a function takes an input and returns an ouput.  
Key parts of a function:
- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets

It will look something like this:

```javascript
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

## Control Flow

The ***control flow*** is the order in which the computer executes statements in a script, in most cases this will be top to bottom (Line 1, Line 2, Line 3, etc.). Often times a typical script can include strucutres that alter the control flow, like *conditionals* and *loops*. For example:

```javascript
if (field==empty) {
    promptUser();
} else {
    submitForm();
}
```

This script will prompt a user to fill out an empty field. If there are no empty fields than the script will submit the form.

[Back to HOME](../README.md)