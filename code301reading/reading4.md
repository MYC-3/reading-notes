# React and Forms

## Forms
[All notes were taken from here](https://reactjs.org/docs/forms.html)
- What is a ‘Controlled Component’? <br>
  >An input form element whose value is controlled by React in this way is called a “controlled component”.
- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why. <br>
You should change the state when the user submits the form to avoid unnecessary running of code.
- How do we target what the user is entering if we have an event handler on an input field? <br>
`event.target.value`
You pass in the event as an argument to the handle event function.

## Conditional (Ternary) Operator
- Why would we use a ternary operator?
Allows for simpler, cleaner code.
- Rewrite the following statement using a ternary statement:
```Javascript
 if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

```
x === y ? console.log(true) : console.log(false);
```


[Back to HOME](../README.md)