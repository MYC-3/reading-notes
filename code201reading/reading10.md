# Reading Notes 10 - JS Debugging

## Error Handling and Debugging
- Keep in mind the **order of execution** in order to easily find errors.
- Keep in mind the context and scope of variables/code.
- Javascript interprets code one line at a time.
- *Error* objects will give you the name of the error, description, file name, and line # of the error.
- Types of Errors:
  1. Error - generic error.
  2. SyntaxError
  3. ReferenceError
  4. TypeError
  5. RangeError
  6. URIError
  7. EvalError
- The console log is a powerful tool to help you debug.
- Execution of a script can be paused using a breakpoint.
- You can *throw* new errors which creates a new Error object.
- Tips:
  - Try another browser.
  - use console.log to see how far your code reaches before an error.
  - strip down your code to the bare minimum.
  - explain the code out loud.
  - use validation tools like jslint.com

  [Back to HOME](../README.md)