# Java Complete Notes

### From Basics to Advanced ☕🚀

> A complete Java crash course notes collection covering core concepts from beginner to advanced level including OOP, Multithreading, Exception Handling, and Java Collection Framework.

---

# 📌 Table of Contents

1. Introduction to Java
2. Java Architecture (JDK, JRE, JVM)
3. Java Program Structure
4. Primitive Data Types
5. Type Casting
6. Strings & Characters
7. Operators in Java
8. Conditional Statements
9. Loops
10. Arrays
11. Object Oriented Programming (OOP)
12. Encapsulation
13. Constructors
14. Inheritance
15. Polymorphism
16. Abstraction
17. Interfaces
18. Access Modifiers
19. Multithreading
20. Synchronization
21. Exception Handling
22. Java Collection Framework
23. List Interface
24. Set Interface
25. Map Interface
26. Final Summary

---

# ☕ Introduction to Java

Java is a high-level, object-oriented programming language developed by Sun Microsystems.

## 🔥 Key Features

* Object-Oriented
* Platform Independent
* Secure
* Robust
* Multithreaded
* High Performance (with JIT Compiler)

## 🌍 WORA Principle

**Write Once, Run Anywhere**

Java code runs on any device that has JVM installed.

---

# ⚙️ Java Architecture

## 📦 JDK (Java Development Kit)

Used by developers for writing and compiling Java programs.

Includes:

* Compiler (`javac`)
* JRE
* Debugging tools

---

## 🖥️ JRE (Java Runtime Environment)

Used to run Java applications.

Includes:

* JVM
* Core Libraries

---

## ⚡ JVM (Java Virtual Machine)

Responsible for:

* Running Java Bytecode
* Converting Bytecode into Machine Code

---

# 🔄 Java Execution Process

```text
Java Source Code (.java)
        ↓
Compiler (javac)
        ↓
Bytecode (.class)
        ↓
JVM
        ↓
Machine Code
```

---

# 🧠 Basic Java Program Structure

```java
class Test {

    public static void main(String[] args) {

        System.out.println("Hello World");

    }

}
```

## 🔍 Main Method Breakdown

| Keyword         | Meaning                |
| --------------- | ---------------------- |
| `public`        | Accessible everywhere  |
| `static`        | No object needed       |
| `void`          | Returns nothing        |
| `main`          | Entry point            |
| `String[] args` | Command line arguments |

---

# 📦 Packages in Java

Packages organize classes like folders.

Example:

```java
package com.example.project;
```

Benefits:

* Better code management
* Avoid naming conflicts
* Modular structure

---

# 🔢 Primitive Data Types

| Data Type | Size   | Description          |
| --------- | ------ | -------------------- |
| `byte`    | 8-bit  | Small integer        |
| `short`   | 16-bit | Medium integer       |
| `int`     | 32-bit | Default integer      |
| `long`    | 64-bit | Large integer        |
| `float`   | 32-bit | Decimal values       |
| `double`  | 64-bit | More precise decimal |
| `char`    | 16-bit | Single character     |
| `boolean` | 1-bit  | true / false         |

---

# 🔄 Type Casting

## ✅ Widening Casting

Automatic conversion.

```java
int a = 10;
double b = a;
```

---

## ⚠️ Narrowing Casting

Manual conversion.

```java
double a = 10.5;
int b = (int) a;
```

---

# 🔤 Strings in Java

Strings are objects of the `String` class.

```java
String name = "Zainab";
```

---

## 🧠 String Pool

Java stores string literals in a special memory area called **String Pool**.

---

## ⚠️ String Comparison

### Using `==`

Compares references.

```java
a == b
```

### Using `.equals()`

Compares actual values.

```java
a.equals(b)
```

---

# ➕ Operators in Java

## Arithmetic Operators

| Operator | Meaning        |
| -------- | -------------- |
| `+`      | Addition       |
| `-`      | Subtraction    |
| `*`      | Multiplication |
| `/`      | Division       |
| `%`      | Modulus        |

---

## Increment & Decrement

```java
a++;
++a;
```

---

# 🧮 Bitwise Operators

| Operator | Meaning     |    |
| -------- | ----------- | -- |
| `&`      | AND         |    |
| `        | `           | OR |
| `^`      | XOR         |    |
| `~`      | NOT         |    |
| `<<`     | Left Shift  |    |
| `>>`     | Right Shift |    |

Example:

```java
5 & 3
```

Result:

```text
1
```

---

# ⚖️ Relational Operators

| Operator | Meaning            |
| -------- | ------------------ |
| `>`      | Greater than       |
| `<`      | Less than          |
| `>=`     | Greater than equal |
| `<=`     | Less than equal    |
| `==`     | Equal              |
| `!=`     | Not equal          |

---

# 🔗 Logical Operators

| Operator | Meaning |   |    |
| -------- | ------- | - | -- |
| `&&`     | AND     |   |    |
| `        |         | ` | OR |
| `!`      | NOT     |   |    |

---

# 🔀 Conditional Statements

## If Statement

```java
if(condition) {

}
```

---

## If-Else

```java
if(condition) {

} else {

}
```

---

## Else-If Ladder

```java
if() {

} else if() {

} else {

}
```

---

## Switch Case

```java
switch(day) {

    case 1:
        break;

    default:
}
```

---

## Ternary Operator

```java
condition ? trueValue : falseValue;
```

---

# 🔁 Loops in Java

## While Loop

```java
while(condition) {

}
```

---

## For Loop

```java
for(int i = 0; i < 5; i++) {

}
```

---

## Do While Loop

```java
do {

} while(condition);
```

---

## For-Each Loop

```java
for(int num : arr) {

}
```

---

# 📚 Arrays in Java

```java
int[] arr = new int[5];
```

Features:

* Fixed Size
* Same Data Type
* Zero-based indexing

---

# 🏗️ OOP in Java

## Class

Blueprint of objects.

```java
class Car {

}
```

---

## Object

Instance of class.

```java
Car c1 = new Car();
```

---

# 🔒 Encapsulation

Wrapping data and methods together.

Use:

* Private variables
* Getters & Setters

Example:

```java
class Student {

    private int age;

    public void setAge(int age) {
        this.age = age;
    }

    public int getAge() {
        return age;
    }

}
```

---

# 🛠️ Constructors

Special methods used to initialize objects.

```java
class Car {

    Car() {
        System.out.println("Constructor Called");
    }

}
```

---

# 🧬 Inheritance

Allows one class to inherit another class.

```java
class Animal {

}

class Dog extends Animal {

}
```

---

## Types of Inheritance

* Single
* Multilevel
* Hierarchical

Java does NOT support multiple inheritance using classes.

---

# 🎭 Polymorphism

## Method Overloading

Same method name with different parameters.

```java
void add(int a, int b) {

}

void add(int a, int b, int c) {

}
```

---

## Method Overriding

Subclass provides its own implementation.

```java
class Animal {

    void sound() {

    }

}

class Dog extends Animal {

    void sound() {

    }

}
```

---

# 🎨 Abstraction

Hiding implementation details.

Achieved using:

* Abstract Classes
* Interfaces

---

## Abstract Class

```java
abstract class Animal {

    abstract void sound();

}
```

---

# 🔌 Interfaces

Blueprint for classes.

```java
interface Mobile {

    void makeCall();

}
```

---

## Java 8 Features in Interfaces

* Default Methods
* Static Methods

---

# 🔑 Access Modifiers

| Modifier    | Accessibility        |
| ----------- | -------------------- |
| `private`   | Same class only      |
| default     | Same package         |
| `protected` | Package + subclasses |
| `public`    | Everywhere           |

---

# 🧵 Multithreading

Running multiple threads simultaneously.

---

## Creating Threads

### Extending Thread Class

```java
class MyThread extends Thread {

    public void run() {

    }

}
```

---

### Implementing Runnable Interface

```java
class MyThread implements Runnable {

    public void run() {

    }

}
```

---

## Starting Thread

```java
t.start();
```

---

# 🔐 Synchronization

Prevents race conditions.

```java
synchronized void increment() {

}
```

---

# ⚠️ Exception Handling

Used to handle runtime errors.

---

## Try Catch

```java
try {

} catch(Exception e) {

}
```

---

## Finally Block

```java
finally {

}
```

Always executes.

---

# 📦 Java Collection Framework (JCF)

Provides ready-made data structures.

---

# 📋 List Interface

Allows:

* Ordered data
* Duplicate values

## Implementations

* ArrayList
* LinkedList

Example:

```java
ArrayList<String> list = new ArrayList<>();
```

---

# 🧩 Set Interface

Stores unique values only.

## Implementations

* HashSet
* LinkedHashSet

Example:

```java
HashSet<Integer> set = new HashSet<>();
```

---

# 🗺️ Map Interface

Stores key-value pairs.

## Implementations

* HashMap
* LinkedHashMap

Example:

```java
HashMap<Integer, String> map = new HashMap<>();
```

---

# 🚀 Final Summary

This Java crash course covered:

✅ Java Basics
✅ Data Types
✅ Operators
✅ Conditions & Loops
✅ Arrays
✅ OOP Concepts
✅ Multithreading
✅ Exception Handling
✅ Collection Framework

---

# ⭐ Recommended Next Topics

* JDBC
* File Handling
* Generics
* Lambda Expressions
* Streams API
* Spring Boot
* Hibernate
* DSA in Java

---

# 🤝 Contribution

Feel free to fork this repository and improve the notes.

---

# 📜 License

Open Source — Free to Use

---

# 💙 Made with Java & Coffee ☕
