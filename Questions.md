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
            System.out.printf("%-15s%03d\n",s1,x);
            }
            System.out.println("================================");

    }
}

```

</details>