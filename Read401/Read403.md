# Maps, primitives, File I/O

## Java Primitives versus Objects

**Java Type System**

* Java contains two types of primitives such as inet and boolean

* Every object contains a single value of primitive type and the wrapper classes are immutable

```
Integer j = 1;          // autoboxing
int i = new Integer(1); // unboxing
```

* The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

**Pros and Cons**

* Single Item Memory Footprint : they live on the heap and are relatively slow to access , single variable of Boolean type occupies as much space as 128 primitive ones, while one Integer variable occupies as much space as four int ones 

* Memory Footprint for Arrays : We can see either that singlee-element arrays of primitive types are always more expensive (except for long and double) than the corresponding reference type.

* Performance : Even for such a simple operation, we can see that performing the operation for assembler classes requires more time. In the case of more complex operations such as addition, multiplication or division, the difference in speed may increase.

* Default Values : This means that primitive types may acquire values only from their domains, while reference types may acquire a (null) value that does not in some sense belong to their domains. There is no such problem with wrapper class variables because null is a clear indication that the variable has not been initialized.

**Conclusion**

* Primitive types are much faster and require much less memory. Therefore, we may prefer to use it.

* The current Java language specification does not allow raw types to be used in parameterized types (generics), in Java collections or the Reflection API.

## Exceptions in Java

**What Is an Exception?**

* An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

* A Runtime error is called an Exceptions error. It is any event that interrupts the normal flow of program execution.

**The Catch or Specify Requirement**

* Catch : A method can catch an exception by providing an exception handler for that type of exception.

* Specify : A method specifies that it can throw exceptions by using the throws clause in the method declaration

* The Three Kinds of Exceptions

    1- the checked exception

    2- exception is the error

    3- exception is the runtime exception

**Example on how to throw an Exceptions**
```
public Object pop() {
    Object obj;

    if (size == 0) {
        throw new EmptyStackException();
    }

    obj = objectAt(size - 1);
    setObjectAt(size - 1, null);
    size--;
    return obj;
}
```
* The exceptions that a method can throw include

1- Any exception thrown directly by the method with the throw statement

2- Any exception thrown indirectly by calling another method that throws an exception

**Scanning**

Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

