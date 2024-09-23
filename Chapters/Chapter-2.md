# Chapter 2 : Operators and Control Statements

## Q. What is an Operator and why do we need operators?

An **operator** in Java is a special symbol or keyword used to perform operations on variables and values. Operators are essential because they allow us to perform arithmetic, comparison, and logical operations to manipulate data and control the flow of the program.

## Q. List down all the operators available in Java?

Java operators are categorized into several types:

1. **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
2. **Unary Operators**: `+`, `-`, `++`, `--`, `~`, `!`
3. **Assignment Operators**: `=`, `+=`, `-=`, `*=`, `/=`, `%=`
4. **Relational Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
5. **Logical Operators**: `&&`, `||`, `!`
6. **Bitwise Operators**: `&`, `|`, `^`, `~`, `<<`, `>>`, `>>>`
7. **Ternary Operator**: `? :`
8. **Instanceof Operator**: `instanceof`
9. **Type Comparison Operator**: `instanceof`
10. **New Operator**: `new`
11. **Dot Operator**: `.`

## Q. What is the difference between Relational and Logical Operators?

- **Relational Operators**: Used to compare two values. They return `true` or `false` based on the comparison.
  Example: `==`, `!=`, `>`, `<`, `>=`, `<=`

- **Logical Operators**: Used to combine multiple conditions or expressions. They return a boolean value (`true` or `false`).
  Example: `&&` (Logical AND), `||` (Logical OR), `!` (Logical NOT)

## Q. What is the purpose of the 'new' operator?

The `new` operator is used to create new objects in Java. It allocates memory for an object and calls the constructor to initialize the object.

Example:

```java
MyClass obj = new MyClass();
```

## Q. What is the purpose of 'dot(.)' operator?

The **dot (.)** operator is used to access the members (methods, fields) of a class or object. It is used to invoke methods or access variables belonging to an object or class.

Example:

```java
MyClass obj = new MyClass();
obj.myMethod(); // Accessing method using dot operator
```

## Q. What is the purpose of `instanceof` operator?

The `instanceof` operator in Java is used to check whether an object is an instance of a specific class or subclass. It returns a boolean value (`true` or `false`). The `instanceof` operator helps in ensuring that an object is of a certain type before performing type-specific operations on it.

Example:

```java
public class InstanceOfExample {
    public static void main(String[] args) {
        String str = "Hello";
        if (str instanceof String) {
            System.out.println("str is an instance of String");
        }
    }
}
```

## Q. What is the difference between "=" and "==" operators?

- **`=` (Assignment Operator)**: The `=` operator is used to assign a value to a variable. It assigns the value on the right-hand side to the variable on the left-hand side.

Example:

```java
int x = 5; // Assigns the value 5 to the variable x
```

- **`==` (Equality Operator)**: The `==` operator is used to compare two values or objects to check if they are equal. It returns true if the values are equal, and false otherwise.

Example:

```java
if (x == 5) { // Compares the value of x with 5
    System.out.println("x is 5");
}
```

## Q. What is the purpose of Control Statements & List down all the control statements available in Java?

Control statements in Java are used to dictate the flow of program execution based on certain conditions or to repeat a block of code. These statements allow decision-making, looping, and control of the execution flow in the program, which is essential for writing logical programs.

### Types of Control Statements in Java:

1. **Conditional Statements**:

   - `if`
   - `if-else`
   - `else-if`
   - `switch`

2. **Looping Statements**:

   - `for`
   - `while`
   - `do-while`

3. **Branching Statements**:
   - `break`
   - `continue`
   - `return`

---

## Q. Write a Java program on if - else if - else ladder

```java
public class IfElseLadder {
    public static void main(String[] args) {
        int number = 15;

        if (number > 20) {
            System.out.println("Number is greater than 20");
        } else if (number == 15) {
            System.out.println("Number is equal to 15");
        } else {
            System.out.println("Number is less than 15");
        }
    }
}
```

## Q. Write a Java program on 'switch' case

```java
public class SwitchExample {
    public static void main(String[] args) {
        int day = 3;

        switch (day) {
            case 1:
                System.out.println("Sunday");
                break;
            case 2:
                System.out.println("Monday");
                break;
            case 3:
                System.out.println("Tuesday");
                break;
            default:
                System.out.println("Invalid day");
                break;
        }
    }
}
```

## Q. What is the difference between `while` & `do-while` loops?

- **`while` loop**: The condition is checked before the loop body is executed. If the condition is false at the beginning, the loop body will not execute at all.

  Example:

  ```java
  while (condition) {
      // Loop body
  }
  ```

- **`do-while` loop**:The loop body is executed at least once, regardless of the condition, because the condition is checked after the execution of the loop body.

  Example:

  ```java
    do {
    // Loop body
  } while (condition);

  ```

## Q. Write a Java program on 'while' loop

```java
public class WhileLoopExample {
    public static void main(String[] args) {
        int i = 1;
        while (i <= 5) {
            System.out.println(i);
            i++;
        }
    }
}
```

## Q. What is the difference between 'while' loop & 'for' loop?

- **`while` loop**:
  The `while` loop is used when the number of iterations is not known beforehand. It repeatedly executes a block of code as long as the condition is true. The condition is checked before the loop body is executed.

  Example:

  ```java
  while (condition) {
      // Loop body
  }
  ```

- **`for` loop**: The for loop is generally used when the number of iterations is known. It allows you to initialize, set a condition, and update the loop variable in a single line.

Example:

```java
for (initialization; condition; iteration) {
    // Loop body
}
```

## Write a Java program on 'for' loop

Here's an example of a Java program using a `for` loop:

```java
public class ForLoopExample {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.println("Iteration " + i);
        }
    }
}
```

## Write a java program on 'nested for loop'

A nested for loop is a loop inside another loop. The inner loop runs multiple times for each iteration of the outer loop.

### Example Program

```java
public class NestedForLoop {
    public static void main(String[] args) {
        for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 3; j++) {
                System.out.println("Outer loop: " + i + ", Inner loop: " + j);
            }
        }
    }
}
```

## What is the difference between 'break' and 'continue' & 'return' keywords

- **`break`**:

  - Used to terminate the current loop or switch statement. Control passes to the statement following the loop or switch.
  - **Example**: Exiting a loop when a specific condition is met.

- **`continue`**:

  - Used to skip the current iteration of a loop and proceeds to the next iteration of the loop.
  - **Example**: Skipping an iteration when a specific condition is met.

- **`return`**:
  - Used to exit from the current method and can optionally return a value to the method's caller. It terminates the execution of the method.
  - **Example**: Exiting a method early based on a condition and returning a result.

## Write a java program using 'break' keyword

he following program demonstrates the use of the `break` keyword to exit a loop when a certain condition is met.

```java
public class BreakExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            if (i == 5) {
                break; // Exit the loop when i equals 5
            }
            System.out.println(i);
        }
    }
}
```

## Write a java program using 'continue' keyword

The following program demonstrates the use of the continue keyword to skip the current iteration of a loop when a certain condition is met.

```java
public class ContinueExample {
    public static void main(String[] args) {
        for (int i = 1; i <= 10; i++) {
            if (i % 2 == 0) {
                continue; // Skip the even numbers
            }
            System.out.println(i);
        }
    }
}
```
