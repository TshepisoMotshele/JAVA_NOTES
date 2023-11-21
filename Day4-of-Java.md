# desion control
**Introduction to Decision Control in Java:**

When writing programs, it's often necessary to execute different sets of statements based on certain conditions. Decision control structures in Java allow you to implement this logic, making your programs dynamic and responsive to varying situations.

### Need for Decision Control:

In programming, situations arise where you need to perform different actions based on specific conditions. For example, consider a scenario where you want to determine if a number is positive or negative. Depending on whether the number is greater than zero or less than zero, you would want to execute different sets of statements.

### Control Flow Statements:

Control flow statements are used to dictate the flow of execution in a program. Decision control, specifically, helps you choose which set of instructions to execute based on the evaluation of conditions.

### Decision Making Structures:

Decision-making structures in Java involve one or more conditions that are evaluated by the program. Depending on the result of these conditions, specific statements are executed. These structures typically include:

1. **Conditions:**
    - Conditions are expressions that evaluate to either true or false.
    - Example:
      
           int number = 5;
          if (number > 0) {
          // Code to execute if the condition is true
          System.out.println("Positive Number");
          } else {
          // Code to execute if the condition is false
          System.out.println("Negative Number");
          }
    

2. **True Block and False Block:**
    - The true block contains the statements to be executed if the condition is true.
    - The false block contains statements to be executed if the condition is false.

3. **Multiple Conditions:**
    - Decision control can involve multiple conditions using constructs like `else if` or `switch`.
    - Example:
      
          int number = 0;
          if (number > 0) {
          System.out.println("Positive Number");
          } else if (number < 0) {
          System.out.println("Negative Number");
          } else {
          System.out.println("Zero");
          }
    

### Importance:

Decision control structures are fundamental for creating adaptive and intelligent programs. They enable your code to respond dynamically to different scenarios, enhancing the flexibility and functionality of your applications.

In summary, decision control in Java allows you to design programs that can make choices and execute specific actions based on the evaluation of conditions, making your code more versatile and capable of handling diverse situations.

### If Statement:

An `if` statement is a fundamental control flow statement that allows you to execute a block of code based on the evaluation of a Boolean expression.

**Syntax:**

    if (Boolean_expression) {
    // Statements will execute if the Boolean expression is true
    }


- If the `Boolean_expression` evaluates to true, the block of code inside the `if` statement will be executed.
- If the `Boolean_expression` evaluates to false, the block of code inside the `if` statement will be skipped.

### IF ELSE Statement:

An `if` statement can be followed by an optional `else` statement, allowing you to handle the case when the Boolean expression is false.

**Syntax:**

    if (Boolean_expression) {
    // Statements will execute if the Boolean expression is true
    } else {
    // Statements will execute if the Boolean expression is false
    }


- If the `Boolean_expression` is true, the first block of code will be executed.
- If the `Boolean_expression` is false, the second block of code (inside the `else` statement) will be executed.

**Example:**

    int num = 30;

    if (num < 50) {
    System.out.println("num is less than 50");
    } else {
    System.out.println("num is greater than or equal to 50");
    }


### Nested If Statement:

An `if` statement can be followed by an optional `else if...else` statement, allowing you to test various conditions using a single `if...else if` construct.

**Syntax:**

    if (condition1) {
    // Statements executed if condition1 is true
    } else if (condition2) {
    // Statements executed if condition2 is true
    } else {
    // Statements executed if none of the conditions are true
    }


- Multiple `else if` statements allow testing various conditions in sequence.
- Once an `else if` succeeds, none of the remaining `else if` or `else` statements will be tested.

**Example:**

    int x = 20;

    if (x == 10) {
    System.out.print("Value of X is 10");
    } else if (x == 20) {
    System.out.print("Value of X is 20");
    } else if (x == 30) {
    System.out.print("Value of X is 30");
    } else {
    System.out.print("This is the else statement");
    }


In the provided example, only the block associated with the first true condition will be executed. Once a condition is true, the rest of the `else if` and `else` blocks are skipped.

### Switch Statement:

A `switch` statement in Java allows a variable to be tested for equality against a list of values. It provides a concise way to perform different actions based on the value of a variable.

#### General Rules:

1. The variable in a `switch` statement can be integers, convertible integers (byte, short, char), strings, and enums.
2. Each case is followed by the value to be compared to and a colon.
3. The value for a case must be the same data type as the variable in the switch, and it must be a constant or a literal.
4. When the variable being switched is equal to a case, the statements following that case will execute until a `break` statement is reached.
5. If no `break` appears, the flow of control will fall through to subsequent cases until a `break` is reached.
6. A `switch` statement can have an optional `default` case, which must appear at the end. The default case is executed when none of the cases is true. No `break` is needed in the default case.

#### Syntax:


      switch (expression) {
    case value1:
        // statements
        break;
    case value2:
        // statements
        break;
    // ... other cases
    default:
        // statements for the default case
}


#### Example:


      int day = 3;
      String dayType;

      switch (day) {
    case 1:
        dayType = "Monday";
        break;
    case 2:
        dayType = "Tuesday";
        break;
    case 3:
        dayType = "Wednesday";
        break;
    // ... other cases
    default:
        dayType = "Unknown day";
      }

      System.out.println("Day: " + dayType);


### Ternary Operator:

The ternary operator (`? :`) is a concise way to express conditional statements. It is often used as a shorthand for simple `if-else` statements.

#### Syntax:


      (expression1) ? expression2 : expression3;


- If `expression1` is true, the value of the whole expression is `expression2`.
- If `expression1` is false, the value of the whole expression is `expression3`.

#### Example:


      int age = 20;
      String message = (age < 18) ? "You are a minor" : "You are an adult";
      System.out.println(message);


In the example, if the `age` is less than 18, the value of `message` will be "You are a minor"; otherwise, it will be "You are an adult". The ternary operator is a concise way to handle simple conditional logic.



