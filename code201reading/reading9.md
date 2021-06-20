# Reading Notes 9 - Form and Events

## Forms
- Forms are a tool in HTML where a user can input some information, like the Google search bar.
- Examples of forms: text boxes, password inputs, checkboxes, submission buttons.
- Code example:
```html
<form action="example" method="get or post">
  <p>Stuff shows up here</p>
</form>
```
- Every `<form>` requires an `action` attribute.
- `methods` can be `get` or `push`.
- `get` is ideal for search boxes or retrieving data.
- `post` is used to upload a file, contains sensitive data, adds data.
- if no `method` is specified, forms will default to `get`
- `<input>` element lets the user type their response.
- `<textarea>` creates a multi-line input box.
- Examples of different `<input>` types: password, radio, checkbox, file, submit.
- `<select>` creates a dropdown list for the user to choose from.
- HTML5 input types: form validation, date, email, url, search.
- CSS can be used to style forms and make them more appealing.

## JS Events
- Events occur whenever the user interacts with the page, i.e. click a link, hover or swipe an element, type, resize the window, page fully loads.
- Events can be used to **trigger** a function or script.
- Main types of events:
  1. UI Event - load, unload, error, resize, scroll
  2. Keyboard Event - keydown, keyup, keypress
  3. Mouse Event - click, dbclick, mousedown, mouseup, mousemove, mouseover, mouseout
  4. Focus Event
  5. Form Event
  6. Mutation Event

[Back to HOME](../README.md)