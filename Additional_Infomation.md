# IN THIS WE CAN SEE THE ADDITION INFORMATION ABOUT THE JAVA

1. static Keyword in Java

- The static keyword in Java is mainly used for memory management, allowing variables and methods to belong to the class itself rather than individual instances. The static keyword is used to share the same variable or method of a given class. The users can apply static keywords with variables, methods, blocks, and nested classes. The static keyword belongs to the class rather than an instance of the class. The static keyword is used for a constant variable or a method that is the same for every instance of a class.

2. Dynamic meaning in java

- Java is considered a dynamic language because of its ability to adapt and modify itself during runtime. This feature allows for greater flexibility in the coding process by enabling developers to update and alter elements of a program without requiring a complete recompilation.


# 🔢 Data Type Precedence (Promotion Hierarchy)

> 📚 This hierarchy is based on **widening conversion** or **type promotion** used in languages like Java and C.

## 🧠 Order: Highest to Lowest Precedence

| Rank | Data Type | Description |
|------|-----------|-------------|
| 1️⃣   | `double`   | 64-bit floating-point, highest precision |
| 2️⃣   | `float`    | 32-bit floating-point |
| 3️⃣   | `long`     | 64-bit integer |
| 4️⃣   | `int`      | 32-bit integer (default integer type) |
| 5️⃣   | `char`     | 16-bit Unicode character (acts like int in math ops) |
| 6️⃣   | `short`    | 16-bit integer |
| 7️⃣   | `byte`     | 8-bit integer |

---

## ⚠️ Special Note:

- `boolean` is **not** part of this hierarchy — you can’t use it in arithmetic expressions.
- In mixed expressions, the **lower type automatically gets promoted** to the higher one.

---

## 💡 Example in Java:

```java
int a = 5;
double b = 6.7;
System.out.println(a + b);  // Output: 11.7 (a promoted to double)
