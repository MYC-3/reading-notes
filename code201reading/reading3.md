# Reading Notes 3 - HTML Lists, CSS Boxes, JavaScript Control Flow

## Lists
There are 3 types of lists:
- `<ol>` Ordered list - numbered list
- `<ul>` Unorder list - bulleted list
- `<dl>` Definition list - terms followed by definitions.
Lists can be nested within other lists. Like so:

- List 1
- List 1
  1. List 2
  2. List 2
  3. List 2
- List 1

## Boxes
CSS treats each HTML element as if it were in its own box.
Each "box" has these properties:
- Margin
- Border
- Padding

Block level elements can be changed in to inline level elements and vice versa.

## Arrays
- Arrays store a list of variables.
- Variables in an array do not need to be the same data type, i.e. Boolean, Number, String.
- Each item in an array is given an index, a number used to find specific items in the array.
- Indexes start at 0 not 1.

## If..Else statements
This statement checks if a condition is true or false. If true it runs the following section of code. If false it'll move to check the next condition of the statement.

## Switch statements
A switch statment is similar to the "if..else" statement. A switch statement has a switch value variable. The value of that variable will determine which code should be run.

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

[Back to HOME](../README.md)