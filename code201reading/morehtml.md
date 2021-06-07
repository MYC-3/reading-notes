# Reading Notes 2 - HTML Text, CSS Introduction, Basic JavaScript Instructions

## HTML

HTML element cheat sheet:

Element | Description
--------|---------
`<h1>` `<h2>`, etc | Header tags 1 through 6.
`<p>` | paragraph tag. Used for text and other content.
`<b>` `<i>` | **Bold** and *Italic*
`<strong>` `<em>` | similar to **Bold** and *Italic*, respectively
`<sup>` `<sub>` | supercript and subscript
`<br />` `<hr />` | line break
`<blockquote>` | used to quote longer sentences and paragraphs

## CSS
CSS (Cascading Style Sheets) is used to control how the HTML elements are presented in your web browser. For example, you can change the color, size, and layout of the content on your page.

### Practical Example

```css
h1 {
    color: red;
}
```
Here the `h1` is known as a **selector** and it specifies that the following lines of code will only apply to the `h1` tag in HTML. In the next line we have the **property** and the **value** seperated by a colon, in this case `color` and `red` respectively.

## Different ways to insert CSS

There a 3 ways to insert a style sheet to format your HTML document:

1. External CSS
2. Internal CSS
3. Inline CSS

### External CSS

A separate file holds all the CSS information and is linked in to your HTML code in the `<head>` section.

### Internal CSS

Useful when a single page HTML pages needs a unique style. Use the `<style>` element in the section of the HTML page.

### Inline CSS

Useful when applying a different style to a single element on the page. For example:
```markdown
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```
***IMPORTANT***
If you are using multiple different style sheets, the value from the last read style will be used.

## Javascript

Javascript is a just-in-time programming language, which means it is compiled during the execution of the program. Along with HTML and CSS, Javascript is very important to the functionality of the majority of websites on the internet.

### Inputs and Outputs

Javascript can take a user generated inputs and manipulate them to produce an output. For example, a program that allows you to write your name and have the computer greet you.

### Variables

Javascript uses `var` as containers to store data values.
An array is a special variable that stores a list of values.

### Functions

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

[Back to HOME](../README.md)