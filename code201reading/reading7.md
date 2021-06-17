# Reading Notes 7 - HTML Tables; JS Constructor Functions

## Domain Modeling

Domain Modeling is a conceptual model used to solve problems in that domain.

## HTML Tables

- A table visualizes information in a grid format.
- Example:
```html
  <table>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
    </tr>
    <tr>
      <td>4</td>
      <td>5</td>
      <td>6</td>
    </tr>
  </table>
```

Looks like this:
  <table>
    <tr>
      <td>1</td>
      <td>2</td>
      <td>3</td>
    </tr>
    <tr>
      <td>4</td>
      <td>5</td>
      <td>6</td>
    </tr>
  </table>

- `<th>` element is used to give headers for rows and columns within the table.
- `<colspan>` is used to span columns.
- `<rowspan>` is used to span row
- `<thead>`, `<tbody>`, `<tfoot>` can be used to distinguish the first and last line from the rest of the table.

##  Objects

- Objects are made up of properties and methods.
- Properties and methods are made up of keywords and values.
- You can update the properties of an object but not a method using the dot notation or square brackets.
- You can create and change properties of an object using literal notation or object constructor notation.
- Arrays are a type of object where the key is the index number for each value.
- You can combine arrays and objects and contain them within each other.
- There are 3 groups of built-in objects:
  1. Browser Object Model
  2. Document Object Model
  3. Global Javascript Objects.
- Javascript has several built in objects like: String, Number, Math, and Date.

[Back to HOME](../README.md)