# INTRODUCTION OF JAVA

- java is one of the programming language which can be used to develop the applications,websites,and desktop applications in this it an object oriented programming language 
- And main thing it is not 100% object oriented programming language
- Because of using primitive data types like INT,CHAR,BOOLEAN,this are not objects 


# ☕ Java Program Breakdown — `learn.java`

## 📄 Code:
```java
public class learn {
    public static void main(String[] naidu) {
        
    }
}
```
🧠 Explanation


🔹 public class learn {

- public = 
This is an access modifier — it means this class can be accessed from anywhere, even outside the package. It’s like saying, “Yo, I’m available for everyone!”

- class = 
This is the keyword used to declare a class in Java. A class is like a blueprint for creating objects.

- learn = 
This is the name of the class.
By convention, Java class names should start with a capital letter, so Learn would be more appropriate.
Since it's a public class, the file name must be learn.java.

🔹 public static void main(String[] naidu) {
This is the main method — the entry point of any standalone Java application.

- public = 
This method is accessible to the JVM, which needs to call it from outside the class.

- static = 
This means you don’t need to create an object of the class to run this method.
The JVM just calls it directly.

- void = 
The method doesn't return anything. It just does stuff, but doesn't give anything back.

- main =
The starting point of execution — Java looks for this method to start running the program.

- String[] naidu = 
This is the parameter — it's an array of strings.
Java passes any command-line arguments into this array.
naidu is just a variable name — it could be args, anything, even banana.

🔹 }
These are the closing braces for the main method and the learn class.


## Java Keywords Table

| **Keyword**   | **Meaning**                                                |
|---------------|-------------------------------------------------------------|
| `public`      | Accessible from anywhere                                    |
| `class`       | Blueprint for an object                                     |
| `static`      | Can be run without creating an object                       |
| `void`        | Doesn’t return anything                                     |
| `main`        | The entry point for Java applications                       |
| `String[]`    | Array to hold command-line arguments                        |
| `naidu`       | Just a variable name — can be anything                      |
