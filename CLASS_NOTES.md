```java

class Naveen{
    void raghu(){
        System.out.println("Friend1");
    }
}
class Chaitu{
    void raghu(){
        System.out.println("Friend2");
    }
}
class Bemmi{
    void raghu(){
        System.out.println("Friend3");
    }
}
public class polymorphism {
public static void main(String args[]){
    Naveen n=new Naveen();
    Chaitu c=new Chaitu();
    Bemmi b=new Bemmi();
    n.raghu();
    c.raghu();
    b.raghu();
}
}

```


# abstraction
- abstraction is the process of hadding the certain details and showing the essential details to the user
- It has two types abstaract class,abstract method

### Abstract class
- abstarct class is a restricted class for that we can't create the object 
- we can acess the properties of the abstarct of the abstract class by over ridding the properties in the some other class 
- abstarct supports both concreate ,non concreate methods

- concreate method is also called as non abstract method
- abstract method is also called as non concreate method

- We create the abstract class without abstract method 
- abstract keyword which is used to create the abstract class

### Abstract method

- we can create the abstract method by using the abstract keyword
- abstract method should not have a block of code
- we can acess the abstract method by over ridding the in the some other class 


```java

abstract class hai{
    void college(){
        System.out.println("mec");
    }
    abstract void otp();
}

public class polymorphism extends hai{

    void otp(){
        System.out.println("Message");
    }
    public static void main(String[] args) {
        polymorphism p=new polymorphism();
        p.otp();
        p.college();
    }
}

```


# INTERFACE

- Interface is used to hide the functionalitys fully
- interface is the keyword which will act like a class
- we can't create the object for interfac
- we can able to use the only abstract methods only inside the interface

# Difference Between Interface and Abstract Class in Java

| Feature | Interface | Abstract Class |
|--------|-----------|----------------|
| **Keyword** | `interface` | `abstract` |
| **Purpose** | To achieve 100% abstraction and multiple inheritance | To provide partial abstraction and code reusability |
| **Abstraction Level** | Fully abstract (until Java 7) <br> Java 8+ allows default and static methods | Can be partially abstract (can have both abstract and concrete methods) |
| **Instantiation** | Cannot create object | Cannot create object |
| **Constructors** | Cannot have constructors | Can have constructors |
| **Access Modifiers** | All methods are implicitly `public` and `abstract` (Java 7) | Can use any access modifier (private, protected, public) |
| **Method Implementation** | No method implementation (till Java 7), but Java 8+ allows `default` and `static` methods | Can have both implemented and unimplemented methods |
| **Fields/Variables** | All fields are `public static final` by default | Can have instance variables (not necessarily static/final) |
| **Multiple Inheritance** | Supports multiple inheritance using interfaces | Does not support multiple inheritance |
| **Use Case** | Ideal for defining capabilities or contracts (e.g., `Flyable`, `Drivable`) | Ideal when you want to share code among closely related classes |
| **When to Use** | When you just want to define a contract with no implementation | When you want to provide some common behavior but still require subclasses to define specific behavior |
| **Java 8+ Enhancements** | Can have `default`, `static`, and `private` methods | Java 8 didn't add new features to abstract classes, but they're still powerful |

---

## ✅ Interface Example

```java
interface Animal {
    void sound(); // abstract method
    default void sleep() {
        System.out.println("Sleeping...");
    }
}

class Dog implements Animal {
    public void sound() {
        System.out.println("Dog barks");
    }
}
```

## Abstract Class Example

```java

abstract class Vehicle {
    abstract void start(); // abstract method
    void fuel() {
        System.out.println("Fueling vehicle...");
    }
}

class Car extends Vehicle {
    void start() {
        System.out.println("Car is starting");
    }
}

```
- we can create the relation between the class and interface by using the implements keyword

```java

interface hai
{
    void college();
}
public class polymorphism implements hai {

    public void college(){
        System.out.println("message");
    }
    public static void main(String args[]){
        polymorphism p=new polymorphism();
        p.college();
    }
}

```

```java

interface parent1 
{
    void car();
}
interface parent2 
{
    void bike();
}
class polymorphism implements parent1,parent2
{
    public void bike()
    {
        System.out.print("ninja");
    }
    public void car()
    {
        System.out.print("volkswagen");
    }
    public static void main (String[] args) 
    {
        polymorphism m=new polymorphism();
        m.car();
        m.bike();
    }
}

```

# THREADING 

- Threading the light weight process
### Types of threading

- Single thread, multithread
- by using two ways we cna achive the 2 ways

- extending the thread class 
- implementing the runnable interface
- it have 4 constructors
- Thread()
- Thread(String)
- Thread(Runnable)
- Thread(String,Runnable)

