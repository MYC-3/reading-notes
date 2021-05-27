# Reading 8 - Operators and Loops

## Operators

Different types of Operators:
- Assignment operators
    - The assignment operator assigns the value of the right operand to the left operand.
    - For example: `x = y` assigns the value of `y` to `x`
- Comparison operators
    - The comparison operator will compare the left and right operands and returns a logical value of true or false.
    - Operator | Description
         ------|-----------
        `==`| Returns true if the operands are equal
        `!=`| Returns true if the operands are **not** equal
        `==`| Returns true if the operands are equal and the same data type
        `!==`| Returns true if the operands are the same type but not equal **or** not the same type.
        `>`| Returns true if the left operand is greater.
        `>=`| Returns true if the left operand is greater than or equal to the right.
        `<`| Returns true if the left operand is less
        `<=`| Returns true if the left operand is less than or equal to the right.

- Arithmetic operators
    - `+` addition
    - `-` subtraction
    - `x` multiplication
    - `/` division
    - `++` increment
    - `--` decrement
    - `**` expononent
- Bitwise operators
- Logical operators
    - Used commonly with boolean values (true or false) but can be used to return a non-boolean value.
    - `&&` used to see if both operands are true.
    - `||` used to see if even one operand is true.
    - `!` returns *false* if the single operands is true.
- String operators
- Conditional (ternary) operator
- Comma operator
- Unary operators
- Relational operators

## Loops

### `for` Loop

A `for` loop will repeat its statement until it's condition evaluates as `false`.

For example:

```
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
```

### `while` Loop

A `while` statement will continue executing its statement as long as the specified condition evaluates to `true`.

An example:

```
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
```

For each loop, n is being incremented one and then adding that value to x.

***Important***

Avoid infinite loops. Set up `while` loops to make sure the condition will eventually become `false`, otherwise the loop will never end.

[Back to HOME](README.md)