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

# 6 in this print the code even and odd

- Take the two inputs
- print the odd and evens

# Sample input

```java
1 2
```

# Sample output

```java
1 3 5 7
2 4 6
```

<details>
<summary><strong>💀🤷‍♂️</strong></summary>

```java 
import java.util.Scanner;
public class Practice {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int num1=sc.nextInt();
        int num2=sc.nextInt();
        for (int i=num1;i<=num2;i++){
            if(i%2!=0){
                System.out.print(i+" ");
            }
        }
        System.out.println();
        for (int i=num1;i<=num2;i++){
            if(i%2==0){
                System.out.print(i+" ");
            }
        }
        sc.close();
    }
}

```
</details>

# 7 PRINT THE SUM OF N NATURAL NUMBERS

- Take the input as the number 
- print the sum of the the number upto the range

# sample input

```java
4
```

# sample output

```java
10   //1+2+3+4
```
<details>
<summary><strong>🤷‍♂️💀ANSWER</strong></summary>

```java

public class Practice {

    public static void main(String[] args) {
        int num=4;
        int sum=0;
        for (int i=1;i<=num;i++){
            sum=sum+i;
        }
        System.out.println(sum);
    }
}

```

</details>

# 8 Print the given number is Automorphic Number ot not 

- 5 is automorphic number because 5 X 5=25 the last number is 5 
- 4 is not automorphic number 4 X 4=16 the lat number is 6

# sample input
```java 
5
```

# sample output

```java
Automorphic Number
```

<details>
<summary><strong>🤷‍♂️💀ANSWER</strong></summary>

```java
public class Practice {

    public static void main(String[] args) {
        int num=7;
        int sq=num*num;
        if ((sq%10)==num){
            System.out.println("Automorphic Number");
        }
        else{
            System.out.println("Not Automorphic Number");
        }
    }
}

```

</details>


# 9 Print the given number is Harshad number or not

- 12 input 1+2=3 so 12 % 3 it return reminder as 0
- so that's why it is harshad number

# sample input 
```java
12
```
# output
```java
Harshad Number
```

<details>
<summary><strong>🤷‍♂️💀</summary></strong>

```java
import java.util.Scanner;
public class Practice {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        int temp=num;
        int sum=0;
        while(num>0){
            int def =num%10;
            sum=sum+def;
            num=num/10;
        }
        if (temp%sum==0){
            System.out.println("Harshad Number");
        }
        else{
            System.out.println("Not Harshad Number");
        }
        sc.close();
    }
}
```

</details>

# 10 Check the person reache thir destination or not

- when a man buy a new car he not check the fuel level and he started to go to the temple in that we display the when he reached the destination or not fuel is thir to that destination display "can reach" or not "can not reach"

# sample input
- input consists of 1 float and 2 int's

```java
11
6
67
```

# sample output

```java
Cannot reach
```
<details>
<summry><strong>🤷‍♂️💀ANSWER</summary></strong>

```java
import java.util.Scanner;
public class Practice {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        float millage=sc.nextFloat();
        int liters=sc.nextInt();
        int distance=sc.nextInt();
        System.out.println((millage*liters>=distance)?"can reach":"cannot reach");
        sc.close();
    }
}
```
</details>

# 11 to find the students who are the attend theh placements in drive 

- The students with 0 arrears with above 7.0 CGPA 
- The studnets with 1,2 arrears  with above 7.5 CGPA THIS ARE THE Eliglble for placements 
- Take user input name,roll,CGPA,arrears
- TWO ints and one float (arrears)
- And String

# sample input 

```java
raghu
78
7.2
2
```
# sample output

```java
raghu
78
not eligible for placements
```

<details>
<summary><strong>💀🤷‍♂️Answer</strong></summary>

```java
import java.util.Scanner;
public class patterns {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String name=sc.nextLine();
        int roll=sc.nextInt();
        float cgpa=sc.nextFloat();
        int arrea=sc.nextInt();
    if ((arrea==0 & cgpa>=7.0)){
        System.out.println(name+"\n"+roll+"\nEligible to attend placement");
    }
    else if((cgpa>7.5) & (arrea==1||arrea==2)){
        System.out.println(name+"\n"+roll+"\nEligible to attend placement");
    }
    else{
        System.out.println(name+"\n"+roll+"\nNot Eligible to attend placement");
    }
    }
}

```
</details>

# 12 Print the follwing information based

- car 1 travelling into 3 roads in that we can get the in which road the car travelled in the road 
- road1,road2,road3
- tip is when the lest distance travelled in this win the race 
- take the user input as the three roads distance 
- in that print the least distance travelled it is same like in 3 digit number least number
- it pass the all the test cases it is an example

# sample input 

```java
123
43
24
```

# sample output

```java
Car 1 goes into road B
```

<details>
<summary><strong>🤷‍♂️💀ANSWER</strong></summary>

```java
import java.util.Scanner;
public class patterns {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int road1=sc.nextInt();
        int road2=sc.nextInt();
        int road3=sc.nextInt();
        if (road1<road2){
            if(road1<road3){
                System.out.println("Car 1 goes road A");
            }
            else{
                System.out.println("car 1 goes road  B");
            }
        }
        else{
            if(road2<road3){
                System.out.println("car 1 goes road B");
            }
            else{
                System.out.println("car 1 goes road C");
            }
        }
        sc.close();
    }
}

```

</details>


# 13 Print the profit and lose of shop seller 
- when 12 bananna rs is x and 1 bananna rs is y print the when seller selllon the bananna total at amout rs and 1 price also displayed in that we calculate the when the seller is profit,lose,and break even out 

# sample input 
```java
60
4
```

# sample output

```java
Lose
```

<details>
<summary><strong>🤷‍♂️💀ANSWER</strong></summary>

```java

```
</details>