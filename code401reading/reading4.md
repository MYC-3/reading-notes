# OOP (Object-Oriented Programming)

## Objects

[Notes taken from this site](https://docs.oracle.com/javase/tutorial/java/concepts/)

- Objects consist of *state* and *behavior*
- E.g. a dog has a state that consists of things like name, color, breed. It also has behaviors like running, wagging, fetching.
- State = variables
- Behavior = methods
- Pros of Objects in programming:
  - modularity
  - information-hiding
  - code re-use
  - pluggability and debugging

## Class

[Notes taken from this site](https://docs.oracle.com/javase/tutorial/java/concepts/class.html)

- A class is like a blueprint from which similar objects are created.
- Example: 
```Java
class Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

    void changeCadence(int newValue) {
         cadence = newValue;
    }

    void changeGear(int newValue) {
         gear = newValue;
    }

    void speedUp(int increment) {
         speed = speed + increment;   
    }

    void applyBrakes(int decrement) {
         speed = speed - decrement;
    }

    void printStates() {
         System.out.println("cadence:" +
             cadence + " speed:" + 
             speed + " gear:" + gear);
    }
}
```

## Binary, Decimals, Hexadecimals

[Notes taken from this site](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)

- Unlike normal "base 10" counting method, Binary is in base 2. e.g. 2 = 10, 23 = 10111

- Hexadecimal example:

|Decimal    |0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15|
|-----------|-|-|-|-|-|-|-|-|-|-|--|--|--|--|--|--|
|Hexadecimal|0|1|2|3|4|5|6|7|8|9| A| B| C| D| E| F|

[Back to HOME](../README.md)