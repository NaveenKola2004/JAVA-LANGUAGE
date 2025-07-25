# Java Operators Explained

Java provides a rich set of operators to perform operations on variables and values. These are categorized as:

- **Unary Operators**
- **Binary Operators**
- **Ternary Operator**

---

## 1. Unary Operators

Unary operators operate on **a single operand**.

| Operator | Description                          | Example       | Result         |
|----------|--------------------------------------|---------------|----------------|
| `+`      | Unary plus (positive number)         | `+a`          | `+5` if `a = 5`|
| `-`      | Unary minus (negative number)        | `-a`          | `-5` if `a = 5`|
| `++`     | Increment (prefix/postfix)           | `++a` / `a++` | `a = a + 1`    |
| `--`     | Decrement (prefix/postfix)           | `--a` / `a--` | `a = a - 1`    |
| `!`      | Logical NOT                          | `!true`       | `false`        |
| `~`      | Bitwise complement                   | `~a`          | If `a=5`, then `~a = -6` (in binary) |

### Example:
```java
int a = 5;
System.out.println(+a);   // 5
System.out.println(-a);   // -5
System.out.println(++a);  // 6
System.out.println(a--);  // 6 (then becomes 5)
System.out.println(!true); // false

```

# 2. Java Binary Operators

**Binary operators** work with **two operands** and are the most commonly used in Java programming.

Binary operators are categorized into:

- Arithmetic Operators
- Relational (Comparison) Operators
- Logical Operators
- Bitwise Operators
- Assignment Operators

---

## ➕ 1. Arithmetic Operators

These are used to perform basic mathematical operations.

| Operator | Name         | Description                 | Example     | Result  |
|----------|--------------|-----------------------------|-------------|---------|
| `+`      | Addition     | Adds two operands           | `5 + 3`     | `8`     |
| `-`      | Subtraction  | Subtracts second from first | `5 - 3`     | `2`     |
| `*`      | Multiplication| Multiplies operands        | `5 * 3`     | `15`    |
| `/`      | Division     | Divides numerator by denom  | `6 / 2`     | `3`     |
| `%`      | Modulo       | Remainder of division       | `5 % 3`     | `2`     |

### 💡 Example:
```java
int a = 10, b = 3;
System.out.println(a + b);  // 13
System.out.println(a % b);  // 1
```

# 🔍 Java Relational (Comparison) Operators

**Relational operators** in Java are used to **compare two values or expressions**. These comparisons always return a **boolean result**: either `true` or `false`.

They are most commonly used in:

- `if`, `while`, and `for` statements
- Logical conditions
- Expressions involving decision-making

---

## 📋 List of Relational Operators

| Operator | Description                    | Example        | Result       |
|----------|--------------------------------|----------------|--------------|
| `==`     | Equal to                       | `a == b`       | `true` if `a` is equal to `b` |
| `!=`     | Not equal to                   | `a != b`       | `true` if `a` is not equal to `b` |
| `>`      | Greater than                   | `a > b`        | `true` if `a` is greater than `b` |
| `<`      | Less than                      | `a < b`        | `true` if `a` is less than `b` |
| `>=`     | Greater than or equal to       | `a >= b`       | `true` if `a` is greater than or equal to `b` |
| `<=`     | Less than or equal to          | `a <= b`       | `true` if `a` is less than or equal to `b` |

---

## 🧪 Example Code

```java
public class RelationalExample {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        System.out.println("a == b: " + (a == b));   // false
        System.out.println("a != b: " + (a != b));   // true
        System.out.println("a > b: " + (a > b));     // false
        System.out.println("a < b: " + (a < b));     // true
        System.out.println("a >= b: " + (a >= b));   // false
        System.out.println("a <= b: " + (a <= b));   // true
    }
}

```

# 🧠 Java Logical Operators

Logical operators in Java are used to **combine multiple boolean expressions or values** and return a boolean result (`true` or `false`).

They’re super useful in:

- `if`, `while`, and `for` conditions
- Validations
- Decision-making logic

---

## 🧩 Types of Logical Operators

| Operator | Name         | Description                                               | Example                   | Result     |
|----------|--------------|-----------------------------------------------------------|---------------------------|------------|
| `&&`     | Logical AND  | Returns `true` if **both** conditions are true            | `a > 10 && b < 20`        | true/false |
| `||`     | Logical OR   | Returns `true` if **at least one** condition is true      | `a > 10 || b < 20`        | true/false |
| `!`      | Logical NOT  | Reverses the boolean value (`true` becomes `false`, etc.) | `!(a > 10)`               | true/false |

---

## 🔍 Detailed Explanation

### ✅ `&&` (Logical AND)
Both conditions must be `true` to return `true`.

```java
int a = 10, b = 15;
if (a > 5 && b < 20) {
    System.out.println("Both conditions are true");
}
```

# ✅ || (Logical OR)

- Only one condition needs to be true.

```java 
int a = 5, b = 30;
if (a > 0 || b < 10) {
    System.out.println("At least one condition is true");
}
```

### Output: At least one condition is true


# ✅ ! (Logical NOT)

- Flips the boolean value.

```java

boolean isRaining = false;
if (!isRaining) {
    System.out.println("Go outside, it's dry!");
}
Output: Go outside, it's dry!

```

# ⚙️ Java Bitwise Operators

**Bitwise operators** in Java allow you to manipulate individual **bits** of integer values (like `int`, `byte`, `short`, `long`). They're super fast and useful in **low-level programming**, **optimizations**, **graphics**, **encryption**, and more.

> 🔐 These operators only work on **integer types**, not floats or booleans.

---

## 🧮 List of Bitwise Operators

| Operator | Name                   | Description                                          | Example       |
|----------|------------------------|------------------------------------------------------|---------------|
| `&`      | Bitwise AND            | 1 if **both** bits are 1                             | `5 & 3` → 1   |
| `|`      | Bitwise OR             | 1 if **either** bit is 1                             | `5 | 3` → 7   |
| `^`      | Bitwise XOR            | 1 if **only one** bit is 1                           | `5 ^ 3` → 6   |
| `~`      | Bitwise Complement     | Inverts all bits (1's complement)                    | `~5` → -6     |
| `<<`     | Left Shift             | Shifts bits to the left (multiplies by 2ⁿ)           | `5 << 1` → 10 |
| `>>`     | Right Shift            | Shifts bits to the right (divides by 2ⁿ)             | `5 >> 1` → 2  |
| `>>>`    | Unsigned Right Shift   | Shifts bits right with zero-fill                     | `-5 >>> 1`    |

---

## 🧾 Bitwise Truth Tables

### Bitwise AND (`&`)
| A | B | A & B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 0      |
| 1 | 0 | 0      |
| 1 | 1 | 1      |

### Bitwise OR (`|`)
| A | B | A \| B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 1      |
| 1 | 0 | 1      |
| 1 | 1 | 1      |

### Bitwise XOR (`^`)
| A | B | A ^ B |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 1      |
| 1 | 0 | 1      |
| 1 | 1 | 0      |

---

## 🔎 Example Breakdown (a = 5, b = 3)

- In binary:

- a = 5 → 0101
- b = 3 → 0011


### Calculations:
```java

a & b  → 0001  = 1
a | b  → 0111  = 7
a ^ b  → 0110  = 6
~a     → 1010  = -6 (in 2's complement)
a << 1 → 1010  = 10
a >> 1 → 0010  = 2

```


# 📝 Java Assignment Operators

**Assignment operators** in Java are used to **assign values to variables**. Some assignment operators also perform an operation **and** assign the result in a shorthand way.

> 💡 Every assignment operator stores a value into a variable.

---

## 🧾 Basic Assignment Operator


| Operator | Description              | Equivalent To     |
|----------|--------------------------|--------------------|
| `=`      | Assign                   | `a = 10`           |
| `+=`     | Add and assign           | `a = a + 5`        |
| `-=`     | Subtract and assign      | `a = a - 5`        |
| `*=`     | Multiply and assign      | `a = a * 5`        |
| `/=`     | Divide and assign        | `a = a / 5`        |
| `%=`     | Modulus and assign       | `a = a % 5`        |
| `&=`, `|=`, `^=` | Bitwise assign   | `a = a & b`, etc.  |
| `<<=`, `>>=`, `>>>=` | Shift assign | `a = a << 2`, etc. |

```java
int a;
a = 10;
System.out.println(a); // 10
```


## 3 . 

3. Ternary Operator
The ternary operator is a shorthand for if-else.

>> Syntax:

```java

condition ? expression_if_true : expression_if_false;

```

>> Example:
```java
int a = 10, b = 20;
int max = (a > b) ? a : b;
System.out.println("Max: " + max); // Output: Max: 20
It's called ternary because it involves three operands.
```

<details>
<summary>👉SUMMARY TABLES OF ALL OPERATORS</summary>

# 🧾 Java Operators – Summary Tables Only

This file gives you a **quick reference** to all types of Java operators with simple and clean summary tables.

---

## 🔹 1. Unary Operators

| Operator | Description                      | Example  |
|----------|----------------------------------|----------|
| `+`      | Unary plus (positive sign)       | `+a`     |
| `-`      | Unary minus (negate value)       | `-a`     |
| `++`     | Increment (prefix/postfix)       | `++a`, `a++` |
| `--`     | Decrement (prefix/postfix)       | `--a`, `a--` |
| `!`      | Logical NOT                      | `!true`  |
| `~`      | Bitwise complement               | `~a`     |

---

## 🔹 2. Arithmetic Operators (Binary)

| Operator | Description       | Example     |
|----------|-------------------|-------------|
| `+`      | Addition           | `a + b`     |
| `-`      | Subtraction        | `a - b`     |
| `*`      | Multiplication     | `a * b`     |
| `/`      | Division           | `a / b`     |
| `%`      | Modulus (remainder)| `a % b`     |

---

## 🔹 3. Relational (Comparison) Operators

| Operator | Description                  | Example     |
|----------|------------------------------|-------------|
| `==`     | Equal to                     | `a == b`    |
| `!=`     | Not equal to                 | `a != b`    |
| `>`      | Greater than                 | `a > b`     |
| `<`      | Less than                    | `a < b`     |
| `>=`     | Greater than or equal to     | `a >= b`    |
| `<=`     | Less than or equal to        | `a <= b`    |

---

## 🔹 4. Logical Operators

| Operator | Description           | Example             |
|----------|-----------------------|---------------------|
| `&&`     | Logical AND           | `a > 5 && b < 10`   |
| `||`     | Logical OR            | `a > 5 || b < 10`   |
| `!`      | Logical NOT (unary)   | `!true`             |

---

## 🔹 5. Bitwise Operators

| Operator | Description             | Example     |
|----------|-------------------------|-------------|
| `&`      | Bitwise AND             | `a & b`     |
| `|`      | Bitwise OR              | `a | b`     |
| `^`      | Bitwise XOR             | `a ^ b`     |
| `~`      | Bitwise NOT (unary)     | `~a`        |
| `<<`     | Left shift              | `a << 2`    |
| `>>`     | Right shift             | `a >> 2`    |
| `>>>`    | Unsigned right shift    | `a >>> 2`   |

---

## 🔹 6. Assignment Operators

| Operator | Description              | Equivalent To     |
|----------|--------------------------|--------------------|
| `=`      | Assign                   | `a = 10`           |
| `+=`     | Add and assign           | `a = a + 5`        |
| `-=`     | Subtract and assign      | `a = a - 5`        |
| `*=`     | Multiply and assign      | `a = a * 5`        |
| `/=`     | Divide and assign        | `a = a / 5`        |
| `%=`     | Modulus and assign       | `a = a % 5`        |
| `&=`, `|=`, `^=` | Bitwise assign   | `a = a & b`, etc.  |
| `<<=`, `>>=`, `>>>=` | Shift assign | `a = a << 2`, etc. |

---

## Ternary Operator

| Operator | Description              | Example                     |
|----------|--------------------------|-----------------------------|
| `? :`    | Conditional (ternary)    | `condition ? a : b`         |

---

🧠 **Tip:** Use this file as your **Java Operators Cheat Sheet** during coding interviews, quick revisions, or when you're deep into Java DSA or backend logic.


</details>