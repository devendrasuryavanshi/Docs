# Java Programming Language: Detailed Notes


---

## 1. Introduction to Java

Java is a versatile, object-oriented programming language developed by Sun Microsystems in 1995. It is designed to be platform-independent and follows the "Write Once, Run Anywhere" (WORA) principle, allowing Java applications to run on any device with the Java Virtual Machine (JVM).

## 2. Boilerplate Code

In Java, boilerplate code refers to the standard, repetitive code that is required to set up a basic program structure. It includes the main method, class definition, and package declaration. Below is an example:

```java
// Boilerplate code
package com.example;

public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

## 3. Output in Java

The `System.out.println` statement is commonly used to display output in Java. It prints the specified message to the console. Example:

```java
// Output in Java
public class OutputExample {
    public static void main(String[] args) {
        System.out.println("This is a sample output.");
    }
}
```

## 4. Variables in Java

Variables are containers that store data in a Java program. They must be declared with a data type. Example:

```java
// Variables in Java
public class VariableExample {
    public static void main(String[] args) {
        int age = 25;
        double height = 5.9;
        char gender = 'M';
        String name = "John";
    }
}
```

## 5. Data Types

Java has various data types, including primitive types (int, double, char) and reference types (String, arrays). Example:

```java
// Data Types in Java
public class DataTypesExample {
    public static void main(String[] args) {
        int integerValue = 42;
        double doubleValue = 3.14;
        char charValue = 'A';
        String stringValue = "Hello, Java!";
    }
}
```

## 6. Comments in Java

Comments are used for documentation and to improve code readability. Java supports both single-line (`//`) and multi-line (`/* */`) comments. Example:

```java
// Comments in Java
public class CommentExample {
    public static void main(String[] args) {
        // This is a single-line comment
        /* This is a
           multi-line comment */
    }
}
```

## 7. Input in Java

To take input from the user, the `Scanner` class can be used. Example:

```java
// Input in Java
import java.util.Scanner;

public class InputExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter your name: ");
        String name = scanner.nextLine();
        System.out.println("Hello, " + name + "!");
    }
}
```

## 8. Type Conversion

Type conversion involves converting a variable from one data type to another. Automatic and explicit conversions are possible. Example:

```java
// Type Conversion in Java
public class TypeConversionExample {
    public static void main(String[] args) {
        int intValue = 42;
        double doubleValue = intValue; // Automatic conversion
        System.out.println("Double Value: " + doubleValue);
    }
}
```

## 9. Type Casting

Type casting is the manual conversion of one data type to another. Example:

```java
// Type Casting in Java
public class TypeCastingExample {
    public static void main(String[] args) {
        double doubleValue = 3.14;
        int intValue = (int) doubleValue; // Explicit casting
        System.out.println("Int Value: " + intValue);
    }
}
```

## 10. Type Promotion in Expressions

Type promotion occurs when different data types are involved in an expression. Java automatically promotes the smaller data type to a larger one. Example:

```java
// Type Promotion in Expressions
public class TypePromotionExample {
    public static void main(String[] args) {
        int intValue = 5;
        double doubleValue = 3.14;
        double result = intValue + doubleValue; // Promotion of intValue to double
        System.out.println("Result: " + result);
    }
}
```

## 11. How Does Java Code Run?

Java code undergoes a two-step process: compilation and interpretation.

- **Compilation:** Java source code is compiled into bytecode by the Java Compiler (`javac`), producing a `.class` file.

- **Interpretation:** The Java Virtual Machine (JVM) interprets the bytecode and executes it. This allows Java programs to be platform-independent.

---


## 12. Types of Operators

Operators in Java are symbols that perform operations on operands. They can be classified into various types based on their functionality.

### 12.1 Arithmetic Operators

Arithmetic operators perform basic mathematical operations. They include addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), and modulus (`%`). 

#### Example:

```java
// Arithmetic Operators
public class ArithmeticOperatorsExample {
    public static void main(String[] args) {
        int a = 10, b = 3;
        
        int sum = a + b;          // 13
        int difference = a - b;    // 7
        int product = a * b;       // 30
        int quotient = a / b;      // 3
        int remainder = a % b;     // 1
    }
}
```

### 12.2 Unary Operators

Unary operators operate on a single operand. Examples include the unary plus (`+`), unary minus (`-`), increment (`++`), and decrement (`--`). 

#### Example:

```java
// Unary Operators
public class UnaryOperatorsExample {
    public static void main(String[] args) {
        int x = 5;
        
        int result1 = +x;   // Unary plus: result1 = 5
        int result2 = -x;   // Unary minus: result2 = -5
        int result3 = ++x;  // Increment: result3 = 6
        int result4 = --x;  // Decrement: result4 = 5
    }
}
```

### 12.3 Relational Operators

Relational operators compare two values and return a boolean result. They include equality (`==`), inequality (`!=`), greater than (`>`), less than (`<`), greater than or equal to (`>=`), and less than or equal to (`<=`). 

#### Example:

```java
// Relational Operators
public class RelationalOperatorsExample {
    public static void main(String[] args) {
        int a = 5, b = 8;
        
        boolean isEqual = (a == b);             // false
        boolean isNotEqual = (a != b);          // true
        boolean isGreaterThan = (a > b);        // false
        boolean isLessThan = (a < b);           // true
        boolean isGreaterOrEqual = (a >= b);    // false
        boolean isLessOrEqual = (a <= b);       // true
    }
}
```

### 12.4 Logical Operators

Logical operators perform logical operations on boolean values. They include AND (`&&`), OR (`||`), and NOT (`!`). Understanding how these operators work is essential for controlling the flow of your program based on different conditions.

#### Logical AND (`&&`)

The logical AND operator (`&&`) returns `true` if both operands are `true`, otherwise, it returns `false`. This operator is often used to combine two or more conditions.

##### Example:

```java
// Logical AND Operator
public class LogicalAndExample {
    public static void main(String[] args) {
        int age = 25;
        boolean isStudent = true;

        // Check if the person is a student and under 30 years old
        boolean isYoungStudent = isStudent && (age < 30);
        System.out.println("Is a young student: " + isYoungStudent);
    }
}
```

#### Logical OR (`||`)

The logical OR operator (`||`) returns `true` if at least one of the operands is `true`. It returns `false` only if both operands are `false`. It is often used to create more flexible conditions.

##### Example:

```java
// Logical OR Operator
public class LogicalOrExample {
    public static void main(String[] args) {
        int temperature = 28;
        boolean isSummer = true;

        // Check if it's either summer or the temperature is above 30 degrees
        boolean isHotDay = isSummer || (temperature > 30);
        System.out.println("Is a hot day: " + isHotDay);
    }
}
```

#### Logical NOT (`!`)

The logical NOT operator (`!`) negates the value of its operand. If the operand is `true`, the result is `false`, and vice versa. It is often used to reverse a condition.

##### Example:

```java
// Logical NOT Operator
public class LogicalNotExample {
    public static void main(String[] args) {
        boolean isSunny = true;

        // Check if it's not sunny
        boolean isNotSunny = !isSunny;
        System.out.println("Is not sunny: " + isNotSunny);
    }
}
```

Logical operators play a crucial role in decision-making within Java programs. They help create conditions that guide the program's execution based on the evaluation of boolean expressions.

### 12.5 Assignment Operators

Assignment operators assign values to variables. They include simple assignment (`=`) and compound assignment (`+=`, `-=`, `*=`, `/=`, `%=`).

#### Example:

```java
// Assignment Operators
public class AssignmentOperatorsExample {
    public static void main(String[] args) {
        int x = 5;
        
        x += 3;  // Equivalent to x = x + 3;  // x = 8
        x -= 2;  // Equivalent to x = x - 2;  // x = 6
        x *= 4;  // Equivalent to x = x * 4;  // x = 24
        x /= 2;  // Equivalent to x = x / 2;  // x = 12
        x %= 3;  // Equivalent to x = x % 3;  // x = 0
    }
}
```

## 13. Operator Precedence

Operator precedence determines the order in which operators are evaluated in an expression. It is crucial to understand the precedence to avoid unexpected results.

### 13.1 Operator Precedence Levels

1. Postfix: `expr++`, `expr--`
2. Unary: `++expr`, `--expr`, `+expr`, `-expr`, `!expr`, `~expr`
3. Multiplicative: `*`, `/`, `%`
4. Additive: `+`, `-`
5. Shift: `<<`, `>>`, `>>>`
6. Relational: `<`, `<=`, `>`, `>=`
7. Equality: `==`, `!=`
8. Bitwise AND: `&`
9. Bitwise XOR: `^`
10. Bitwise OR: `|`
11. Logical AND: `&&`
12. Logical OR: `||`
13. Conditional (Ternary): `? :`
14. Assignment: `=`, `+=`, `-=`, `*=`, `/=`, `%=` and others

### 13.2 Examples

Understanding operator precedence is crucial to writing correct and efficient Java expressions. Ensure to use parentheses to explicitly control the order of evaluation when needed.

#### Example:

```java
// Operator Precedence Examples
public class OperatorPrecedenceExample {
    public static void main(String[] args) {
        int result = 5 + 3 * 2;  // Multiplication has higher precedence than addition: result = 11
        boolean condition = (result > 10) && (result % 2 == 0);  // Logical AND has higher precedence than logical OR
    }
}
```

---


## 14. Conditional Statements

Conditional statements in Java allow the execution of different code blocks based on specified conditions. They enable your program to make decisions and choose different paths of execution.

### 14.1 `if` Statement

The `if` statement is the most basic form of a conditional statement. It executes a block of code if the specified condition is true.

#### Example:

```java
// If Statement
public class IfStatementExample {
    public static void main(String[] args) {
        int x = 10;

        if (x > 5) {
            System.out.println("x is greater than 5");
        }
    }
}
```

### 14.2 `if-else` Statement

The `if-else` statement extends the `if` statement by providing an alternative block of code to execute when the condition is false.

#### Example:

```java
// If-Else Statement
public class IfElseStatementExample {
    public static void main(String[] args) {
        int x = 3;

        if (x % 2 == 0) {
            System.out.println("x is even");
        } else {
            System.out.println("x is odd");
        }
    }
}
```

### 14.3 `else if` Statement

The `else if` statement allows the testing of multiple conditions. It is useful when there are more than two possible outcomes.

#### Example:

```java
// Else If Statement
public class ElseIfStatementExample {
    public static void main(String[] args) {
        int dayOfWeek = 3;

        if (dayOfWeek == 1) {
            System.out.println("It's Monday");
        } else if (dayOfWeek == 2) {
            System.out.println("It's Tuesday");
        } else if (dayOfWeek == 3) {
            System.out.println("It's Wednesday");
        } else {
            System.out.println("It's another day");
        }
    }
}
```

### 14.4 Ternary Operator (`? :`)

The ternary operator is a concise way to write simple `if-else` statements in a single line. It evaluates a boolean expression and returns one of two values based on whether the expression is true or false.

#### Example:

```java
// Ternary Operator
public class TernaryOperatorExample {
    public static void main(String[] args) {
        int x = 7;
        String result = (x % 2 == 0) ? "Even" : "Odd";
        System.out.println("Number is " + result);
    }
}
```

## 15. Switch Statement

The `switch` statement provides a way to handle multiple conditions based on the value of an expression. It's particularly useful when there are several possible values for a variable.

### 15.1 Basic Switch Statement

The basic form of the `switch` statement compares the value of an expression against different cases and executes the corresponding block of code.

#### Example:

```java
// Switch Statement
public class SwitchStatementExample {
    public static void main(String[] args) {
        int dayOfWeek = 2;

        switch (dayOfWeek) {
            case 1:
                System.out.println("It's Monday");
                break;
            case 2:
                System.out.println("It's Tuesday");
                break;
            case 3:
                System.out.println("It's Wednesday");
                break;
            default:
                System.out.println("It's another day");
        }
    }
}
```

### 15.2 Switch Statement with Fall-Through

In a `switch` statement, each `case` typically ends with a `break` statement. However, fall-through behavior allows the execution to continue into the next case without a `break`.

#### Example:

```java
// Switch Statement with Fall-Through
public class SwitchFallThroughExample {
    public static void main(String[] args) {
        int dayOfWeek = 3;

        switch (dayOfWeek) {
            case 1:
                System.out.println("It's Monday");
                // Fall-through
            case 2:
                System.out.println("It's a weekday");
                break;
            case 3:
            case 4:
            case 5:
                System.out.println("It's a workday");
                break;
            default:
                System.out.println("It's another day");
        }
    }
}
```

### 15.3 Switch Statement with Strings (Java 7+)

Starting from Java 7, the `switch` statement supports strings, allowing you to switch on the value of a string expression.

#### Example:

```java
// Switch Statement with Strings
public class SwitchStringExample {
    public static void main(String[] args) {
        String day = "Wednesday";

        switch (day) {
            case "Monday":
                System.out.println("It's the first day of the week");
                break;
            case "Wednesday":
                System.out.println("It's the middle of the week");
                break;
            default:
                System.out.println("It's another day");
        }
    }
}
```

Conditional statements and the `switch` statement are powerful tools for controlling the flow of your Java programs. They allow you to create flexible and dynamic logic based on various conditions and values. Understanding their usage is essential for effective programming in Java.

---
