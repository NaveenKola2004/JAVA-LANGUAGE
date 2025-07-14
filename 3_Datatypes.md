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

## 🔹 2. Non-Primitive Data Types (Reference Types)

Non-primitive types are objects and hold references (memory addresses), not actual data.

### Examples:

- `String` → `String name = "Tony";`
- `Array` → `int[] numbers = {1, 2, 3};`
- `Class` → `Student student = new Student();`
- `Interface` → `Runnable r = new MyRunnable();`
- `Enum` → `enum Days { MON, TUE, WED };`
- `Wrapper Classes` → `Integer`, `Double`, `Boolean`, etc.

---

## 🔄 Autoboxing and Unboxing

Java allows conversion between primitive and wrapper objects:

```java
int x = 10;           // primitive
Integer y = x;        // autoboxing (primitive -> object)
int z = y;            // unboxing (object -> primitive)
