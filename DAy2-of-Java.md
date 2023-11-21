# Java Basic Fundamentals

A variable is a name given to a memory location. It is the basic unit of storage in a program.
The value stored in a variable can be changed during program execution.
A variable is only a name given to a memory location; all the operations done on the variable effects that memory location.
In Java, all the variables must be declared before use.

## How to declare a variable?

In Java, you declare a variable by specifying its `data type` and giving it a name.



`data_type variable_name;` (Here, data_type represents the type of data that the variable can hold, and variable_name is the name you give to the variable. After declaring a variable, you can assign a value to it.)


// Declaration of integer variable

          int myNumber;

// Declaration of double variable

        double myDouble;

// Declaration of String variable

        String myString;

**You can also initialize the variable at the time of declaration:**

// Declaration and initialization of integer variable

        int myNumber = 42;

// Declaration and initialization of double variable 

     double myDouble = 3.14;

// Declaration and initialization of String variable

    String myString = "Hello, Java!";

**In Java, variables must be declared before they are used.
Attempting to use a variable without declaring it will result in a `compilation error`.**

Additionally, Java is a `statically-typed language`, meaning that once you declare a variable with a specific type, you cannot change its type later on. 

For example.... if you declare an integer variable, you cannot later assign a string to it.

## Class in Java

Class in Java:

- A class in Java is a blueprint or template that describes the behavior and state that objects of its type support.
- It acts as a constructor, a "blueprint" or a factory for creating objects.
- Essential components of a class include a constructor, methods, and variables/properties.

Creating a Class:

- To create a class, use the keyword class.
- A class includes a constructor, which is a method called when creating an object from the class. If not explicitly defined, the compiler generates a default constructor.
- Constructors may accept parameters, and a class can have multiple constructors.
- Methods define the behaviors of the class.
- Variables or properties describe the attributes of objects created from the class.

```java
public class Person {
    // Variables/Properties
    String name;
    int age;
    double height;

    // Constructor
    public Person() {
        // Constructor code
    }

    // Methods
    public void run() {
        // Method code for running
    }

    public void walk() {
        // Method code for walking
    }

    public void sleep() {
        // Method code for sleeping
    }
}
```

Object in Java:

- An object is an instance of a class, created from classes.
- Objects have states/attributes and behaviors.
Example: A dog is an object with states like color, name, breed, and behaviors like wagging the tail, barking, eating.

- Creating an Object:

- In Java, an object is created from a class.
- Use the class name followed by the object name and the new keyword.
- Call the constructor to initialize the object.


*Person person1 = new Person();*



