
## **`What is Java?`**

Java is a general-purpose, high-level, object-oriented programming language that was designed by James Gosling and Mike Sheridan at Sun Microsystems, which is now a subsidiary of Oracle Corporation. Java was released in 1995 and has since become one of the most widely used programming languages in the world.

## What are the advantages & Disadvantages

### Advantages of Java:

1. **`Platform Independence`:**
- *Advantage:* Java's "Write Once, Run Anywhere" (WORA) philosophy allows code to be executed on any device with a Java Virtual Machine (JVM).
- *Disadvantage:* Some other languages may be more tightly integrated with specific platforms, potentially offering better performance or more platform-specific features.

2. **Strong Ecosystem:**
- *Advantage:* Java has a vast ecosystem with a rich set of libraries, frameworks, and tools, making development efficient and providing solutions for various domains.
- *Disadvantage:* In some specialized domains, other languages might have more specific libraries or frameworks that are better suited.

3. **Object-Oriented Programming:**
- *Advantage:* Java's strong support for object-oriented programming promotes code organization, reusability, and maintainability.
- *Disadvantage:* For projects that do not require or benefit from OOP principles, languages with different paradigms might be more suitable.

4. **Garbage Collection:**
- *Advantage:* Automatic memory management through garbage collection reduces the risk of memory leaks and makes Java code more robust.
- *Disadvantage:* In performance-critical applications, the automatic garbage collection process can introduce latency.

5. **Multithreading:**
- *Advantage:* Java provides built-in support for multithreading, making it easier to develop concurrent and parallel applications.
- *Disadvantage:* Managing multithreading can be complex, and incorrect implementation may lead to issues like race conditions and deadlocks.

6. **Security:**
- *Advantage:* Java has built-in security features, such as the sandbox for applets and the Security Manager in the Java Runtime Environment (JRE).
- *Disadvantage:* The security features can sometimes be restrictive, affecting the performance of certain application

### Disadvantages of Java:

1. **Performance:**
- *Disadvantage:* Java, while optimized for portability, may not be as performant as lower-level languages like C or C++. However, the performance gap has narrowed with advancements in Java virtual machine technologies.

2. **Verbosity:**
- *Disadvantage:* Java code can be verbose compared to some modern languages, which may impact developer productivity and code readability.

3. **Startup Time:**
- *Disadvantage:* Java applications may have a longer startup time compared to languages that compile to native code.

4. **Memory Consumption:**
- *Disadvantage:* Java applications can have higher memory consumption due to the overhead of the Java Virtual Machine and automatic memory management.

5. **Lack of Modern Language Features:**
- *Disadvantage:* Some modern language features found in newer languages are not present in Java. However, newer versions of Java have introduced improvements to address this.

Ultimately, the choice between Java and other programming languages depends on the specific requirements of the project, the development team's expertise, and other factors such as performance, scalability, and ecosystem support. Many successful and large-scale applications have been built using Java, showcasing its versatility and reliability.

1. Platform Independence:
   Description: Java achieves platform independence through the use of bytecode. After compiling Java source code, it is transformed into bytecode, which is a set of instructions for a virtual machine (JVM). This bytecode can be executed on any device that has a compatible JVM, irrespective of the underlying hardware or operating system.

Advantages for Java:
Code written once can run on multiple platforms without modification.
Simplifies software development and deployment across diverse environments.

2. Object-Oriented:
   Description: Java is designed as an object-oriented programming (OOP) language, which means it revolves around the concept of objects. Objects encapsulate data and behavior, promoting modular and reusable code through the use of classes and objects.

Advantages for Java:
Encapsulation, inheritance, and polymorphism enhance code organization and reusability.
Easier maintenance and modification of code through the principles of OOP.

3. Simple:
   Description: Java is designed to be straightforward and easy to use. It eliminates complexities and features found in other languages to provide a clean and simple syntax.

Advantages for Java:
Reduces the learning curve for new developers.
Simplifies the development process, making code more readable and maintainable.

4. Robust Language:
   Description: Java incorporates features that contribute to the robustness of the language, including strong memory management, exception handling, and type checking during compile time.

Advantages for Java:
Enhances reliability by minimizing runtime errors.
Automatic garbage collection ensures efficient memory management.
Comprehensive exception handling contributes to robust error management.

5. Secure:
   Description: Java is designed with security features to protect systems from harmful activities. It includes a robust security model, a secure runtime environment, and features like bytecode verification.

Advantages for Java:
Applets (small Java applications) run in a secure environment.
Prevents unauthorized access and potential security vulnerabilities.

6. Multithreading:
   Description: Java supports multithreading, allowing multiple threads of execution to run concurrently. This is beneficial for developing applications that require parallel processing or handling multiple tasks simultaneously.

Advantages for Java:
Enables the efficient utilization of system resources.
Facilitates the development of responsive and concurrent applications.

In summary, these features collectively make Java a powerful and versatile programming language. Its platform independence, object-oriented nature, simplicity, robustness, security features, and support for multithreading contribute to its popularity and widespread use in various domains, from web development to enterprise applications. Java's design principles prioritize ease of use, maintainability, and reliability, making it a preferred choice for a wide range of software development projects.


## Package Declaration:
The package keyword is used to declare the package to which the class belongs. It specifies the directory structure for the class.


```java
package com.example.myproject;
```

## Import Statements:
The import keyword is used to bring classes from other packages into the current class. Multiple import statements can be used.

```java
import java.util.ArrayList;
import java.util.List;
```

## Comments:
Comments in Java provide information about variables, methods, classes, etc.
```java
// This is a single-line comment

/*
This is a multiline
comment
*/
```

## Class Definition:
The class keyword is used to define a class. A name is given to the class, and it serves as a blueprint for creating objects.

```java
public class MyClass {
// Class members go here
}
```

## Main Method:
The main method is the entry point of a Java program. Execution starts from this method.

```java
public class MyClass {
public static void main(String[] args) {
// Main method code
}
}
```

## Attributes:
Attributes, also known as fields or variables, represent the state of an object. They are declared within the class.

```Java
public class MyClass {
int myAttribute;
}
```
## Methods/Behaviours:
Methods are functions associated with a class that perform specific tasks. They encapsulate functionality and can be reused by passing variable values.

```java
public class MyClass {
public void myMethod(int parameter) {
// Method code
}
}
```
# Activity example
Create a class called dog with two void methods bark() and main() method.
```java
// Package declaration (optional)
// If your class is part of a package, specify it here
package com.example.animals;

// Import statements (optional)
// You can import classes from other packages if needed

// Class definition
public class Dog {

// Attributes (optional)
// Attributes represent the state of the object
// For simplicity, this example doesn't have any attributes

// Method to simulate the dog barking
public void bark() {
System.out.println("Woof! Woof!");
}

// Main method (entry point of the program)
public static void main(String[] args) {
// Create an instance of the Dog class
Dog myDog = new Dog();

// Call the bark method on the Dog instance
myDog.bark();
}
}
```
