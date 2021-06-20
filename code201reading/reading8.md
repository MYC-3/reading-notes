# Reading Notes 8 - More CSS Layout

## CSS
- When designing a webpage, keep in mind that the screen sizes and resolutions will differ from user to user.
- Web designers generally try to keep pages somewhere between 960-1000 pixels wide.
- Fixed width layouts do not scale or change size when the user increases/decreases their browser window.
  - Advantages: pixels are accurate at measuring, greater control, image sizes will stay the same.
  - Disadvantages: can lead to big gaps on the edges of the page, higher resolution leads to smaller page, changes in font size can mess up the page, works best on devices with a similar size.
- Liquid layouts stretch to fit the browser window using percentages.
  - Advantages: little wasted space, more tolerant of user's font sizes and screen size.
  - Disadvantages: Can lead to unexpected spaces or crowded elements, wider windows lead to long lines of text.
  - Website layouts are often in a grid pattern. Makes it easier to read and modify.
  - CSS frameworks exist to provide prewritten code for common tasks. (960.GS CSS Framework)
  - You can use multiple stylesheets. For example, one controls the layout and the other controls the font/color.
  - CSS can use `@import` rule to reference other stylesheets.
  - HTML can use multiple `<link>` elements for each stylesheet.

[Back to HOME](../README.md)