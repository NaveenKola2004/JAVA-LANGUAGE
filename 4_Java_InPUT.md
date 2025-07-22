# 🔍 What is Scanner in Java?
- The Scanner class is part of java.util package and is used to take input from the user — like numbers, strings, booleans, etc.

```java
import java.util.Scanner;
```
-Then, create a Scanner object like this:

```java
Scanner sc = new Scanner(System.in);
```


# Gotcha Moment: nextLine() After nextInt()

```java
int age = sc.nextInt();
String name = sc.nextLine(); // ← Skips input? Why?!
```
# ➡️ Happens because nextInt() leaves a newline (\n) in the buffer. Use an extra sc.nextLine() to clear it.

```java
int age = sc.nextInt();
sc.nextLine(); // consume leftover newline
String name = sc.nextLine();
```


## 🧠 Basic Usage by Data Type (Java Scanner)

| Data Type            | Scanner Method     | Example Code                     |
|----------------------|--------------------|----------------------------------|
| `int`                | `nextInt()`        | `int age = sc.nextInt();`        |
| `float`              | `nextFloat()`      | `float marks = sc.nextFloat();`  |
| `double`             | `nextDouble()`     | `double pi = sc.nextDouble();`   |
| `byte`               | `nextByte()`       | `byte b = sc.nextByte();`        |
| `short`              | `nextShort()`      | `short s = sc.nextShort();`      |
| `long`               | `nextLong()`       | `long l = sc.nextLong();`        |
| `String` (1 word)    | `next()`           | `String name = sc.next();`       |
| `String` (full line) | `nextLine()`       | `String sentence = sc.nextLine();` |
| `boolean`            | `nextBoolean()`    | `boolean flag = sc.nextBoolean();` |
