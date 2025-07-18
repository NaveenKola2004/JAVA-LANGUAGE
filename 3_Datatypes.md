# ☕ Java Data Types

Java data types are divided into two main categories:

- **Primitive Data Types**
- **Non-Primitive Data Types (Reference Types)**

---

## 🔹 1. Primitive Data Types (8 Types)

Primitive data types are the most basic data types in Java. They are not objects and hold raw values.

| Type     | Size       | Default Value | Description |
|----------|------------|----------------|-------------|
| `byte`   | 1 byte     | `0`            | Small integer (-128 to 127) |
| `short`  | 2 bytes    | `0`            | Larger than byte (-32,768 to 32,767) |
| `int`    | 4 bytes    | `0`            | Most commonly used integer |
| `long`   | 8 bytes    | `0L`           | Large integer values |
| `float`  | 4 bytes    | `0.0f`         | Decimal numbers (less precision) |
| `double` | 8 bytes    | `0.0d`         | More precise decimal numbers |
| `char`   | 2 bytes    | `'\u0000'`     | Single character (Unicode) |
| `boolean`| 1 bit*     | `false`        | True or false values |

> 🧠 Note: `boolean` size depends on JVM implementation, but logically it's 1 bit.

---


> ### ALL THE DATATYPE NAMES SHOULD BE IN A SMALL LETTERS 👉E XCEPT (String)

# SYNTAX
#### TO CREATE A DATATYPE

```java
DATATYPE_NAME  VARIABLE =  VALUE;
```
---

### DATA TYPES
> # 👉 byte  👈

- In Java, byte is a primitive data type that represents an 8-bit signed two's complement integer. It's the smallest integer type, useful for conserving memory in large arrays or when dealing with binary data. A byte can hold values ranging from -128 to 127

---

```java
byte num1=127;
byte num2=-128;
```

> # 🫸 integer 🫷

- Integers are whole numbers, meaning they don't have any decimal or fractional parts. 
- A data type used to represent whole numbers (positive, negative, or zero) without any fractional or decimal component.
- Examples include -5, 0, 1, 100, -1000, etc.
### Example

```java
int number=1;
int number2=123456;
```
---
> # 🫸 char 🫷

- characture is used to store the single letter or symbol or number

### Example

```java
char letter='a';
char letter1='A';
char number='2';
char number1='-2';  -> NOT GIVE LIKE THIS BECAUSE - and 2 are two charactures
char symbol='@';
```
---
> # 🫸 float 🫷 

- float is used to store the decimal values in and print the decimal values,
- when we want to get the decimal numbers form the 0,1,2 put the how many decimal points you can assaign the f for  decimal points to print 

```java
    float n=2.09f; // to get the 2.09
```

> ##### Short,double-> discuss later

## 🔹 2. Non-Primitive Data Types (Reference Types)

Non-primitive types are objects and hold references (memory addresses), not actual data.

### Examples:

- `String` → `String name = "Tony";`
- `Array` → `int[] numbers = {1, 2, 3};`
- `Class` → `Student student = new Student();`
- `Interface` → `Runnable r = new MyRunnable();`
- `Enum` → `enum Days { MON, TUE, WED };`
- `Wrapper Classes` → `Integer`, `Double`, `Boolean`, etc.


> 🧠 Unlike primitive types, non-primitive types are **references** to objects, not raw values. They’re flexible, powerful, and object-oriented AF.

---

## 💡 Key Differences from Primitive Types

| Feature            | Primitive Types       | Non-Primitive Types           |
|--------------------|-----------------------|-------------------------------|
| Stored as          | Actual value          | Reference (memory address)    |
| Default value      | 0, false, etc.        | `null`                        |
| Can be customized? | Nope                  | Yes (user-defined classes)    |
| Supports methods?  | No                    | Yes (they have built-in & custom methods) |

---

## 🚀 Types of Non-Primitive Data Types

### 1️⃣ **String**

- A sequence of characters.
- Not a primitive, even though it feels like one.
- Immutable (can't change once created).

```java
String name = "Tony";
System.out.println(name.toUpperCase());  // Output: TONY
```
# 2️⃣ Arrays

- Collection of elements of the same type.

- Fixed in size once declared.
```java
int[] marks = {90, 80, 70};
System.out.println(marks[1]);  // Output: 80
```

# 3️⃣ Classes
- Blueprint for creating objects.

- Can define attributes (variables) and behaviors (methods).

```java
class Student {
    int age;
    void showAge() {
        System.out.println(age);
    }
}
```

# 4️⃣ Objects
- Instance of a class.

- Access class methods and properties using dot . notation.
```java
Student s1 = new Student();
s1.age = 18;
s1.showAge();  // Output: 18
```

# 5️⃣ Interfaces
- Contract with method signatures, but no body.

- A class implements an interface to define the behavior.

```java
interface Animal {
    void makeSound();
}
```

# 6️⃣ Enums
- Special class to define constants.

```java 
enum Day {
    MONDAY, TUESDAY, WEDNESDAY
}
```

---

## 1️⃣ String

**Definition:**  
A `String` is a non-primitive, immutable sequence of characters used to store textual data.

**Interview Explanation:**  
> "In Java, `String` is a class, not a primitive type. It’s used to represent text and is immutable, meaning once created, its value cannot be changed. Java optimizes memory by storing strings in a pool."

```java
String name = "Tony";
```
---
# 2️⃣ Array
## Definition:
- An Array is a fixed-size data structure that stores multiple elements of the same type in contiguous memory locations.

### Interview Explanation:

- "An array in Java is a non-primitive object that can hold multiple values of the same data type. It provides fast access using indices but has a fixed size once declared."

```java
int[] nums = {10, 20, 30};
```
---
# 3️⃣ Class
### Definition:
- A Class is a blueprint or template for creating objects, defining their properties (fields) and behaviors (methods).

### Interview Explanation:

- "A class defines the structure and behavior of objects. It encapsulates data and functionality together, supporting object-oriented principles like inheritance and abstraction."

```java 
class Student {
    int age;
    void display() { System.out.println(age); }
}
```

---
# 4️⃣ Object
## Definition:
- An Object is an instance of a class containing its own state (fields) and behavior (methods).

### Interview Explanation:

- "An object is a runtime entity that represents a class instance. It has a memory address and can access the class's methods and attributes through the dot operator."

```java
Student s1 = new Student();
s1.age = 20;
```
---

# 5️⃣ Interface
## Definition:
- An Interface is a contract that defines abstract methods a class must implement.

### Interview Explanation:

- "Interfaces are used to achieve abstraction and multiple inheritance in Java. They contain method signatures without implementation. Classes that implement an interface must provide concrete definitions for all its methods."

```java
interface Vehicle {
    void start();
}
```
---
# 6️⃣ Enum (Enumeration)
## Definition:
- An Enum is a special data type that defines a collection of constant values.

### Interview Explanation:

- "Enums are used to define a fixed set of constants, like days of the week or status codes. They are type-safe and can include methods and constructors, making them more powerful than plain constants."

```java
enum Day { MONDAY, TUESDAY, WEDNESDAY }
```

---

# 7️⃣ Wrapper Classes
### Definition:
- Wrapper classes are object representations of primitive types.

### Interview Explanation:

- "Java provides wrapper classes like Integer, Double, and Boolean to wrap primitive data types into objects. These are essential when working with Collections, as primitives can't be used directly in them."

- Primitive  	-> Wrapper
int    -> 	Integer
char	-> Character
boolean	-> Boolean

```java
Integer num = 100;
```

## 🧠 Summary Table of Non-Primitive Data Types

| Data Type   | Purpose                                 | Mutable? | Fixed Size? | Object-Oriented? |
|-------------|------------------------------------------|----------|--------------|------------------|
| `String`    | Stores text                              | ❌ No     | N/A          | ✅ Yes           |
| `Array`     | Stores multiple elements of same type    | ✅ Yes    | ✅ Yes        | ✅ Yes           |
| `Class`     | Blueprint to create objects              | N/A      | N/A          | ✅ Yes           |
| `Object`    | Instance of a class                      | ✅ Yes    | N/A          | ✅ Yes           |
| `Interface` | Defines method contracts (no body)       | N/A      | N/A          | ✅ Yes           |
| `Enum`      | Represents a fixed set of constants      | ❌ No     | ✅ Yes        | ✅ Yes           |
| `Wrapper`   | Object representation of primitives      | ✅ Yes    | N/A          | ✅ Yes           |
