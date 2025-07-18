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

