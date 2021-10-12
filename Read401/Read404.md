# Object-Oriented Programming Concepts

* Object-oriented programming combines a group of data attributes with functions or methods into a unit called an "object"

* OOP languages are class-based, which means that a class defines the data attributes and functions as a blueprint for creating objects, which are instances of the class

### What Is an Object?

Each object has an identity, a behavior and a state. The state of an object is stored in fields (variables), while methods (functions) display the object's behavior.

### What Is a Class?

A class is a user defined blueprint or prototype from which objects are created.  It represents the set of properties or methods that are common to all objects of one type.

**expample**

```
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
} }

the Bicycle class does not contain a main method. That’s because it’s not a complete application; it’s just the blueprint for bicycles that might be used in an application. The responsibility of creating and using new Bicycle objects belongs to some other class in your application.
```

## Binary, Decimal and Hexadecimal Numbers

**Decimals**

The Decimal Number System is also called Base 10, because it is based on the number 10, with these 10 symbols: 0, 1, 2, 3, 4, 5, 6, 7, 8 and 9

**Binary**

in the binary we have two digits (0,1) and it base (2)


**Hexadecimal**

They look the same as the decimal numbers up to 9, but then there are the letters ("A',"B","C","D","E","F") in place of the decimal numbers 10 to 15


