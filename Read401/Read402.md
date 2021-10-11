# Arrays, Loops, Imports

## Packages and Import

**Packages**

* Package (directory) in Java is a mechanism to encapsulate a group of classes, sub packages.
* package name is the same as the directory folder name which contains the .java files You declare packages when you define your Java program
* if you want use another package you need to import that package.

**Imports**

To import a package within your program you can use one or more of these syntaxes:
```
import java.util.*; // using the * character to specify the use of all classes within the package.

import java.util.Random; // is used to grab the random class with the util package only.

int seconds =  LocalDateTime.now().getSeconds(); // using the class name without importing.
```

important note :

* you can importing all classes in a package and dose not make the object file (.class or .jar) larger
* All classes in the java.lang package are visible without an import (i.e String, System).
* Order in import list is not required.
* There are 166 packages containing 3279 classes and interfaces in Java 5, only a few packages are used in most programming (most used packages --> [References](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)).

**Loops**

Looping is the feature which allows to execute a certain block of code multiple times with certain controlling set of instructions.

Java provides different types of loops : 

* Simple for loop : "For" Loop is used to repeat a specific block of code a known number of times.

* Enhanced for-each loop : It's functionality is the same as the ordinary for loop. The only differnce is that it has simpler srtucture.

* While loop : The while loop loops through a block of code as long as a specified condition is true

* Do-While loop : The do while loop checks the condition at the end of the loop. This means that the statements inside the loop body will be executed at least once even if the condition is never true. 






