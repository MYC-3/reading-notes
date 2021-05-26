# Reading 6 - Dynamic web pages with Javascript

## About Javascript

Javascript is a just-in-time programming language, which means it is compiled during the execution of the program. Along with HTML and CSS, Javascript is very important to the functionality of the majority of websites on the internet.

## Inputs and Outputs

Javascript can take a user generated inputs and manipulate them to produce an output. For example, a program that allows you to write your name and have the computer greet you.

## Variables

Javascript uses `var` as containers to store data values.

Some examples of Javascript in use:

```
<html>
<head>
  <title>Hello World</title>
</head>
<body>
 
First name: <input id="first_name">
Last name: <input id="last_name">
<button id="say">Say hi!</button>
 
<hr>
<div id="result"></div>
 
<script>
function say_hi() {
    var fname = document.getElementById('first_name').value;
    var lname = document.getElementById('last_name').value;
 
    var html = 'Hello <b>' + fname + '</b> ' + lname;
 
    document.getElementById('result').innerHTML = html;
}
 
document.getElementById('say').addEventListener('click', say_hi);
</script>
 
</body>
</html>
```
[Try it here](https://code-maven.com/try/examples/js/pure_js_greating.html)\
Taken from [code-maven.com](https://code-maven.com/input-output-in-plain-javascript)

[Back to HOME](README.md)