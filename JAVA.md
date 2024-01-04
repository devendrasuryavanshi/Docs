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
