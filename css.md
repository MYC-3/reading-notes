# Reading 5 - Design web pages with CSS

## CSS
CSS (Cascading Style Sheets) is used to control how the HTML elements are presented in your web browser. For example, you can change the color, size, and layout of the content on your page.

### Practical Example
<br/>

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

A seperate file holds all the CSS information and is linked in to your HTML code in the `<head>` section.

### Internal CSS

Useful when a single page HTML pages needs a unique style. Use the `<style>` element in the section of the HTML page.

### Inline CSS

Useful when applying a different style to a single element on the page. FOr example:
```markdown
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```
***IMPORTANT***
If you are using multiple different style sheets, the value from the last read style will be used.


[Back to HOME](README.md)