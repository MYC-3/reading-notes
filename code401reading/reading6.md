# Inheritance and Interfaces

## Inheritance
[Notes taken from this site](https://docs.oracle.com/javase/tutorial/java/concepts/)

- A subclass will inherit the states and behaviors of it's superclass.
- For example, a `MountainBike` class extends the `Bicycle` class. A `Bicycle` has it's own properties like speed, gear, etc that is relevant to a `MountainBike`. But the `MountainBike` class has it's own properties that might not pertain to every `Bicycle.

## Interface
[Notes taken from this site](https://docs.oracle.com/javase/tutorial/java/concepts/)

- A group of related methods with empty bodies.
- [Example code take from here:](https://docs.oracle.com/javase/tutorial/java/concepts/interface.html)
```Java
interface Bicycle {

    //  wheel revolutions per minute
    void changeCadence(int newValue);

    void changeGear(int newValue);

    void speedUp(int increment);

    void applyBrakes(int decrement);
}
class ACMEBicycle implements Bicycle {

    int cadence = 0;
    int speed = 0;
    int gear = 1;

   // The compiler will now require that methods
   // changeCadence, changeGear, speedUp, and applyBrakes
   // all be implemented. Compilation will fail if those
   // methods are missing from this class.

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

- If a class implements an interface, all the methods in that interface must be in included in the class.

## Package
[Notes taken from this site](https://docs.oracle.com/javase/tutorial/java/concepts/)

- Organizes related methods and interfaces.
- Class library = a set of packages aka an application programming interface (API)

[Back to HOME](../README.md)