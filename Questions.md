# 1🧾 Java Task — Read and Print Integers

## ✅ Task

In this challenge, you must read **3 integers** from standard input (stdin) and then print them to standard output (stdout).  
Each integer must be printed on a **new line**.

A portion of the code is already provided in the editor — complete it to finish the task.

---

## 📝 Input Format

There are **3 lines of input**, and **each line contains a single integer**.

---
```java 
123
34
45
```

## 🖨️ Output Format

Print each integer on a **new line**, in the **same order** as the input.


## 🧪 Sample Input

```java
123
34
45
```
---
# Output

```java
123
34
45
```
---


<details>
<summary>
<strong>💀🤷‍♂️ANSWER</strong></summary>

```java
import java.util.Scanner;
public class Practice {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int a=sc.nextInt();
        int b=sc.nextInt();
        int c=sc.nextInt();
        System.out.println(a+"\n"+b+"\n"+c);
        sc.close();
    }
}

```

</details>

# 2 🧠 Java Conditional Task — "Weird or Not Weird"

## ✅ Task Description

Given an integer `n`, perform the following conditional actions:

- If `n` is **odd**, print `"Weird"`
- If `n` is **even** and in the **inclusive range of 2 to 5**, print `"Not Weird"`
- If `n` is **even** and in the **inclusive range of 6 to 20**, print `"Weird"`
- If `n` is **even** and **greater than 20**, print `"Not Weird"`

Complete the stub code to determine whether the input is "Weird" or "Not Weird".

---

## 📝 Input Format

A single line containing a **positive integer**, `n`.
- bitween 1 to 100 only 

# sample input 

```java 
number =3
output: Weird

number=23
output : Not weird
```

<details>
<summary><strong>💀🤷‍♂️ANSWER</strong></summary>

```java
public class Practice {

    public static void main(String[] args) {
        int N=3;
        if ((N&1)!=0){
            System.out.println("Weird");
        }
        else{
            if (N>=2 & N<=5){
            System.out.println("Not Weird");
            }
            else if (N >=6 &N<=20){
                System.out.println("Weird");
            }
            else{
                System.out.println("Not Weird");
            }
        }
    }
}
```
</details>



# 3 # 📚 Java Formatting Challenge — String and Integer Output

## ✅ Task

Every line of input will contain a **String followed by an integer**.

You must print each pair in a specific format:

- The **String** should be **left-justified** in a field of exactly `15` characters.
- The **Integer** should be **zero-padded** and exactly `3` digits wide.

---

## 📥 Input Format

- Each line of input contains a **String** and an **integer** separated by a space.
- Each String will contain **no more than 10 alphabetic characters**.
- Each integer will be in the **inclusive range from 0 to 999**.
- You will be given **3 lines** of such input.

---

## 📤 Output Format

Your output should look like this:

# 📚 Java Formatting Challenge — String and Integer Output

## 🧪 Sample Input (Table Format)

| String | Integer |
|--------|---------|
| java   | 100     |
| cpp    | 65      |
| python | 50      |

---

## 🧾 Sample Output (Formatted Table Look)


| String | Integer |
|--------|---------|
| java   | 100     |
| cpp    | 065      |
| python | 050      |

<details>
<summary><strong>💀🤷‍♂️ANSWER</strong></summary>

```java
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
            Scanner sc=new Scanner(System.in);
            System.out.println("================================");
            for(int i=0;i<3;i++){
                String s1=sc.next();
                int x=sc.nextInt();
                //Complete this line
            // %-15s → left justify string in 15 characters
            // %03d → integer in 3 digits, padded with 0s if needed
            System.out.printf("%-15s%03d\n",s1,x);
            }
            System.out.println("================================");

    }
}

```

</details>

# 4  🔁 Java Loops Challenge — Multiplication Table

## 🎯 Objective

In this challenge, we're going to use **loops** to help us do some simple math.

---

## ✅ Task

Given an integer `N`, print its **first 10 multiples**.  
Each multiple `i` (where `1 <= i <= 10`) should be printed on a new line in the following format:

# Sample input 

```
n=2
```
# output 

```
2 X 1 = 2
2 X 2 = 4
2 X 3 = 6
2 X 4 = 8
2 X 5 = 10
2 X 6 = 12
2 X 7 = 14
2 X 8 = 16
2 X 9 = 18
2 X 10 = 20

```
<details>
<summary><strong>💀🤷‍♂️ANSWER</strong></summary>

```java

public class Practice {
public static void main(String[] args) {
        int N=2;
        for (int i=1;i<=10;i++){
            System.out.println(N+" X "+i+" = "+*i);
        }
    }
}

```

</details>

# 5 ## Problem: Java Stdin and Stdout II

### Input Format

There are three lines of input:
1. The first line contains an integer.
2. The second line contains a double.
3. The third line contains a String.

### Output Format

There are three lines of output:
- On the first line, print `String:` followed by the unaltered String read from stdin.
- On the second line, print `Double:` followed by the unaltered double read from stdin.
- On the third line, print `Int:` followed by the unaltered integer read from stdin.

### Sample Input

```java
42
3.1415
Welcome to HackerRank's Java tutorials!
```

### Sample Output
```java
String: Welcome to HackerRank's Java tutorials!
Double: 3.1415
Int: 42
```

<details>
<summary><strong>💀🤷‍♂️ANSWER</strong></summary>

```java
import java.util.Scanner;
public class Practice {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        double num2=sc.nextDouble();
        sc.nextLine();
        String data=sc.nextLine();

        System.out.println("String : "+data);
        System.out.println("Double : "+num2);
        System.out.println("Int : "+num);
        sc.close();
    }
}

```

</details>

