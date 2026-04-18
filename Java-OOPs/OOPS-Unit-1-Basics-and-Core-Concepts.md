# OOPS Unit 1 - Basics and Core Concepts (Java)

---

## 1. POP vs OOP

### Procedural Oriented Programming (POP)

* Focus on functions and algorithms
* Program divided into functions
* Data moves freely
* Less secure
* Top-down approach
* Less reusable code

### Object Oriented Programming (OOP)

* Focus on objects and data
* Program divided into classes and objects
* Data hiding using encapsulation
* More secure
* Bottom-up approach
* High reusability (inheritance, polymorphism)

---

## 2. Class and Object

### Class

* Blueprint of objects
* Contains variables (fields) and methods
* Does not occupy memory until object is created

### Syntax (Java)

```java
class Car {
    String color;
    void drive() {
        // code
    }
}
```

---

### Object

* Instance of a class
* Represents real-world entity

#### Characteristics:

* State → variables
* Behavior → methods
* Identity → unique memory address

---

## 3. Example (Class + Object)

```java
class Student {
    int id;
    String name;

    void study() {
        System.out.println(name + " is studying");
    }
}

public class Main {
    public static void main(String[] args) {
        Student s1 = new Student();
        s1.name = "Rahul";
        s1.study();
    }
}
```

---

## 4. Pillars of OOP

---

### 4.1 Encapsulation

* Wrapping data and methods into one unit
* Provides data hiding

```java
class Account {
    private double balance;

    public void deposit(double amount) {
        balance += amount;
    }
}
```

---

### 4.2 Abstraction

* Shows only essential details
* Hides internal implementation

```java
abstract class Vehicle {
    abstract void start();
}
```

---

### 4.3 Inheritance

* One class acquires properties of another

```java
class Animal {
    void eat() {
        System.out.println("Eating");
    }
}

class Dog extends Animal {
    void bark() {
        System.out.println("Barking");
    }
}
```

---

### 4.4 Polymorphism

* One name, many forms

#### Method Overloading

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```

#### Method Overriding

* Redefining parent class method in child class

---

## 5. Java Basics

```java
public class FirstProgram {
    public static void main(String[] args) {
        System.out.println("Hello");
    }
}
```

---

## 6. Data Types

### Primitive Data Types

* byte
* short
* int
* long
* float
* double
* char
* boolean

---

### Non-Primitive

* String
* Array
* Class

---

## 7. Type Casting

### Widening (Implicit)

```java
int a = 10;
double b = a;
```

### Narrowing (Explicit)

```java
double a = 9.8;
int b = (int) a;
```

---

## 8. Constructors

* Special method to initialize objects
* Same name as class

### Types:

#### Default Constructor

```java
Student() {
    System.out.println("Object created");
}
```

#### Parameterized Constructor

```java
Student(int id, String name) {
    this.id = id;
    this.name = name;
}
```

---

## 9. this Keyword

* Refers to current object

```java
class Employee {
    int id;
    String name;

    Employee(int id, String name) {
        this.id = id;
        this.name = name;
    }
}
```

---

## 10. Method Overloading

* Same method name
* Different parameters

```java
int add(int a, int b)
int add(int a, int b, int c)
```

---

## 11. Static Keyword

* Belongs to class

```java
class Student {
    static String college = "ABC";
}
```

---

## 12. Strings in Java

* String is an object
* Immutable

### Creation:

```java
String s = "Hello";
String s2 = new String("Hello");
```

---

### String Methods:

* length()
* charAt()
* concat()
* equals()
* substring()

---

## 13. Arrays

* Collection of same data type

### Single Dimension:

```java
int[] arr = new int[5];
```

### Multi-Dimension:

```java
int[][] arr = new int[3][3];
```

---

## 14. Garbage Collection

* Automatic memory management
* Removes unused objects

### Points:

* Runs in background
* Object without reference → removed
* Prevents memory leaks

---

## 15. Operators

* Arithmetic (+, -, *, /, %)
* Relational (==, !=, >, <)
* Logical (&&, ||, !)
* Assignment (=, +=, -=)
* Ternary

---

## 16. Control Flow

### Decision:

* if
* if-else
* switch

### Loops:

* for
* while
* do-while

### Jump:

* break
* continue
* return

---

## Summary

* OOP focuses on objects
* 4 pillars are core
* Java basics include data types and control flow
* Strings, arrays, and GC are important
* Constructors and polymorphism are key concepts

---
