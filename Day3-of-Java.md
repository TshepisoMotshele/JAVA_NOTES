# What is OOP?

`Object-Oriented Programming (OOP)` is a programming paradigm that organizes code based on the concept of "objects," which can contain data in the form of fields (attributes or properties) and code in the form of procedures (methods or functions). The primary goals of OOP are to improve the modularity, reusability, and maintainability of code.

*Purpose:*

- The primary goal of OOP is to enhance flexibility and maintainability in software development.
- Objects bring together data and behavior in a single unit, making it easier to understand and organize code.

*Features:*

-  Objects have their own procedures (methods) that can access and often modify their own data fields.
- Objects can interact with each other, and OOP involves designing programs by creating and manipulating these objects.


*Languages:*

- OOP languages can be class-based or prototype-based.
- Popular class-based OOP languages include Java, C++, C#, Python, and others.
`Examples of prototype-based languages include JavaScript.`

*Examples of OOP Languages:*

- Class-Based: Java, C++, C#, Python, PHP, Kotlin, Swift, Scala, etc.
- Prototype-Based: JavaScript.

*Object-Oriented Concepts:*

- `Encapsulation:` Bundling data and methods that operate on the data within a single unit (object).
- `Inheritance:` Allowing a class (subclass/derived class) to inherit properties and behaviors from another class (superclass/base class).
- `Polymorphism:` The ability of different classes to be treated as objects of a common base class, allowing for flexibility in code design.

# Features of OOP – Core features

Certainly! Let's summarize the main features of Object-Oriented Programming (OOP) into Core Features and Other Features.

### Core Features:

1. **Abstraction:**
    - Definition: Hiding the implementation details from the user, providing only the functionality.
    - Implementation in Java: Achieved using Abstract classes and interfaces.
    - Example:
      ```java
      abstract class Shape {
          abstract void draw();
      }
      ```

2. **Encapsulation:**
    - Definition: Wrapping data (variables) and code (methods) together as a single unit.
    - Implementation in Java:
        - Declare variables as private.
        - Provide public setter and getter methods.
    - Example:
      ```java
      public class Student {
          private String name;
          public String getName() { return name; }
          public void setName(String newName) { name = newName; }
      }
      ```

3. **Inheritance:**
    - Definition: One class acquires the properties (methods and fields) of another.
    - Implementation in Java: Uses the `extends` keyword.
    - Example:
      ```java
      class Animal {
          void eat() { System.out.println("Eating..."); }
      }
 
      class Dog extends Animal {
          void bark() { System.out.println("Barking..."); }
      }
      ```

4. **Polymorphism:**
    - Definition: Processing objects differently based on their data type.
    - Implementation in Java:
        - **Overloading:** Multiple methods with the same name but different parameters (compile-time polymorphism).
        - **Overriding:** A subclass providing a specific implementation for a method defined in its superclass (runtime polymorphism).
    - Example:
      
      *// Overloading*
          
          int add(int a, int b) { return a + b; }
          double add(double a, double b) { return a + b; }

      *// Overriding*
    - 
           class Animal {
           void makeSound() { System.out.println("Animal makes a sound"); }
           }

          class Dog extends Animal {
          @Override
          void makeSound() { System.out.println("Dog barks"); }
          }


### Other Features:

1. **Overloading:**
    - Definition: Having multiple methods with the same name but different parameters.
    - Example: Shown above in the Polymorphism section.

2. **Overriding:**
    - Definition: A subclass providing a specific implementation for a method defined in its superclass.
    - Example: Shown above in the Polymorphism section.

These features collectively contribute to the principles of OOP, such as encapsulation, modularity, and reusability, making code more organized, understandable, and maintainable.

# More Features
Great! Let's summarize the additional features of Object-Oriented Programming (OOP) you've mentioned:

### Other Features:

1. **Coupling:**
    - **Definition:** Refers to the knowledge, information, or dependency of one class on another.
    - **Types of Coupling:**
        - Strong Coupling: Classes are aware of each other's details.
        - Weak Coupling: Classes are less aware of each other, often achieved using interfaces for reduced concrete implementation.

2. **Cohesion:**
    - **Definition:** Refers to the level of a component performing a single well-defined task.
    - **Types of Cohesion:**
        - High Cohesion: A method performs a single, well-defined task.
        - Low Cohesion: A method is split into separate, unrelated parts.
    - **Example:** `java.io` package is highly cohesive, focusing on I/O-related classes and interfaces.

3. **Association:**
    - **Definition:** Represents relationships between objects.
    - **Types of Association:**
        - One to One
        - One to Many
        - Many to One
        - Many to Many
    - **Directionality:** Can be unidirectional or bidirectional.
    - **Examples:**
        - One country has one president (one to one).
        - President has many cabinet ministers (one to many).
        - Many cabinet ministers can have one prime minister (many to one).
        - Many cabinet ministers can have many departments (many to many).

4. **Aggregation:**
    - **Definition:** A narrower kind of association, a one-way (HAS-A) relationship between two classes.
    - **Characteristics:**
        - One-directional association.
        - Represents a HAS-A relationship.
        - Only one class is dependent on the other.

5. **Composition:**
    - **Definition:** A stricter form of aggregation, where two classes are mutually dependent and can't exist without each other.
    - **Characteristics:**
        - A restricted form of aggregation.
        - Represents a PART-OF relationship.
        - Both classes are dependent on each other.
        - If one class ceases to exist, the other can't survive alone.

These features contribute to the design principles of OOP, allowing for better structuring, reusability, and maintainability of code.


