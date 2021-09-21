# Arrays, Loops, and Imports

## Packages and Imports
[Notes were taken based on info from this site](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)
- packages = directories.
- package declarations are optional. Java will create a default package.
- import statements follow a package declaration.
- 3 options for importing:

```Java
import javax.swing.*;  // Make all classes visible altho only one is used.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

```Java
import javax.swing.JOptionPane;  // Make a single class visible.

class ImportTest {
    public static void main(String[] args) {
        JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```
```Java
class ImportTest {
    public static void main(String[] args) {
        javax.swing.JOptionPane.showMessageDialog(null, "Hi");
        System.exit(0);
    }
}
```

## Loops
- Different types of loops:
  1. For Loop - usefull when you know that a chunk of code has to repeat a certain known amount.
  2. For-each Loop
  3. While Loop - uses a boolean expression to loop until that expresssion changes.
  4. Do-while Loop - Very similar to the while loop except the first condition evaluation happens after the first loop, i.e. run through the statement(s) at least once and then check if it is going to be repeated.

[Back to HOME](../README.md)