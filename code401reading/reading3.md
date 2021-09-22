# Maps, primitives, File I/O

## Primitives
[Notes take from this website](https://www.baeldung.com/java-primitives-vs-objects)

- Java has a two-fold type system: Primitives and Reference types.
- Each primitive type has a corresponding reference type.
- Example:

```Java
Integer j = 1;          // autoboxing
int i = new Integer(1); // unboxing
```

- converting a primitive type to a reference type is called unboxing, the reverse is called unboxing.
- Primitive types and memory footprint:
  - boolean – 1 bit
  - byte – 8 bits
  - short, char – 16 bits
  - int, float – 32 bits
  - long, double – 64 bits
- **single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type.**
- More time is required to perform a operation for wrapper classes.
- >Objects in Java are slower and have a bigger memory impact than their primitive analogs.

## Exceptions
[Notes take from here](https://docs.oracle.com/javase/tutorial/essential/exceptions/definition.html)

- Exception = exceptional event, an event that disrupts the normal flow and execution of the program.
- When an error occurs, an *exception object* is created which contains information on the error.
- *Throwing an exception* is when an *exception object* is created and passed to the runtime system.
- **Catch and Specify Requirement** must have the following:
  - > A try statement that catches the exception. The try must provide a handler for the exception
  - > A method that specifies that it can throw the exception. The method must provide a throws clause that lists the exception
- 3 kinds of exceptions:
  1. Checked exception
  2. Error
  3. Runtime exception

## Scanner

- > Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

- A scanner separates tokens by white space (i.e. tabs, empty spaces, line breaks, etc)
- Scanners must be stopped with a *close* method.
- Scanners support all primitive types except for *char*

[Back to HOME](../README.md)