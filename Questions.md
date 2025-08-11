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


# 14. GENERATE THE AUTOMATIC MACHINE 

- In this take user input,and ask the what you want to show the choices in that factorial,sum_digits,reverse,palindrome,updatenumber,odd or even,count of digits

<details>
<summary>👉ANSWER</summary>

```java
import java.util.Scanner;
public class quesionspractice {
    public static void Line(){  // print lines 
        System.out.println("\n------------------");
    }
    public static int count_digits(int number){ // count of numbers
        int count =0,digit;
        while (number!=0){
            digit=number%10;
            count++;
            number/=10;
        }
        return count;
    }
    public static void Even_odd(int number){//even odd check
    System.out.println((number&1)==0?"Even":"Odd");
    }
    public static int factorial(int number){
        if (number==0||number==1){
            return 1;
        }
        return number *factorial(number-1);
    }
    public static int sum_of_digits(int number){ //sum of digits 
        int sum=0,digit;
        if(count_digits(number)<=1){
                    System.out.println("Take atleast 2 numbers choose 7 update the new value");
        }
        else{
        while (number!=0){
            digit=number%10;
            sum=sum+digit;
            number/=10;
        }
    }
        return sum;
    }
    public static void polindrome(int number,int reversed){ //polindrome
        if(count_digits(number)<=1){
                    System.out.println("Take atleast 2 numbers choose 7 update the new value");
        }
        else if(number==reversed){
            System.out.println("Yes");
        }
        else{
            System.out.println("No");
        }
    }
public static int reverse(int number){ // reverse number 
    int digit,reverse=0;
    if(count_digits(number)<=1){
        System.out.println("Take atleast 2 numbers choose 7 update the new value");
    }
    else{
    while (number!=0){
        digit=number%10;
        reverse=reverse*10+digit;
        number/=10;
    }
}
    return reverse;
}

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter the number : ");
        int number=sc.nextInt(),reversed=reverse(number);
        
        for (int x=1;x==1;){
        System.out.println("\n1.reverseNumber \n2.Polindrome check \n3.Sum of number \n4.factorial\n5.Even(or)Odd\n6.Number of digits\n7.Update the number  \n0.Exit");
        System.out.print("choose one :");
        int choice=sc.nextInt();

        switch (choice) {
            case 1:
            Line();
                System.out.printf("%d Reverse is : %d",number,reverse(number));
                Line();
                break;
            case 2:
            Line();
            System.out.printf("%d is polindrome : ",number);
            polindrome(number, reversed);
            Line();
            break;
            case 3:
            Line();
            System.out.printf("%d Sum of numbers is :%d ",number,sum_of_digits(number));
            Line();
            break;
            case 4:
            Line();
            System.out.printf("%d factorial is : %d",number,factorial(number));
            Line();
            break;
            case 5:
            Line();
            System.out.printf("%d is : ",number);
            Even_odd(number);
            Line();
            break;
            case 6:
            Line();
            System.out.printf("In %d Number of digits : %d",number,count_digits(number));
            Line();
            break;
            case 7:
            System.out.print("Enter the new number : ");
            int newNum=sc.nextInt();
            number=newNum;
            break;
            case 0:
            System.out.println("Bye");
            x=0;
            break;
            default:
            System.out.println("INvalid choice! try again");
            break;
        }
    }
    sc.close();
    }

}
```
</details>



# 15 WITHOUT USING THE INBUILT FUCTION GENERATE a ->A

- R -> r
- a -> A
- 65 ASCI and 97 
- don't use the inbult function and the +,- or if else and variables also


<details>
<summary>ANSWER</summary>

```java
import java.util.Scanner;
public class polymorphism {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println((char)((sc.next().charAt(0))^32));
    }
}

```
</details>

<details>
<summary>CODE</summary>

```python

def armstrong(n):
    l=str(n)
    store=0
    while (n>0):
        d=n%10
        data=d**len(l)
        store=store+data
        n=n//10
    return store
n=int(input())
if(n==armstrong(n)):
    print("yes")
else:
    print("No")

```
</details>


# 16 changing the upper to lower case only the vowels

- Test case 1
 - Ab -> ab
- Test case 2
  - AEIOU -> aeiou
- Test case 3
  - Hello world! -> HEllO wOrld!


<details>

<summary> Code </summary>

```java

import java.util.*;;
public class polymorphism {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String c=sc.nextLine();
        String f="";
        for (int i=0;i<c.length();i++){
            char k=c.charAt(i);
            if(k == 'a' || k=='e'||k=='o'||k=='i'||k=='u'){
                   f=f+((char)(k^32));
            }
            else{
                f=f+k;
            }
        }
        System.out.println(f);
        sc.close();
    }
}

```
</details>



# 17 Check the whether the array Or list is sorted or not

<details>

<summary>Code</summary>

```java

import java.util.*;

public class polymorphism {

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        
        int[] arr=new int[n];

        for (int i=0;i<n;i++){
            arr[i]=sc.nextInt();
        }

        boolean asc=true;
        boolean desc=true;
        for (int i=1;i<arr.length;i++){
            if(arr[i]>arr[i-1]) desc=false;
            if(arr[i]<arr[i-1])   asc=false;
        }
        if(asc){
            System.out.println("sorted");
        }
        else if(desc){
            System.out.println("sorted");
        }
        else{
            System.out.println("not sorted ");
        }
    }
}

```

# python

```python

l=[]
n=int(input())
for i in range(1,n+1):
    data=int(input())
    l.append(data)
asc=True
desc=True
for i in range(1,n):
    if(l[i]>l[i-1]):
        desc=False
    if(l[i]<l[i-1]):
        asc=False
if desc or asc :
    print("sorted")
else:
    print("not sorted")

```


</details>


# 18 String is palindrome or not

<details>

<summary>CODE</summary>

```python

def palindrome(word):
    sample=""
    for i in word:
        sample=i+sample
    return sample
word=input("Enter the word to check the palindrome : ")

if(word==palindrome(word)):
    print("yes")
else:
    print("no")
    
```

# JAVA

```java

import java.util.*;
public class solution {
public static void polindrom(String name){
    String sample="";
    for (int i=0;i<name.length() ;i++){
        char s=name.charAt(i);
        sample=s+sample;
    }
    if(name.equals(sample)){
        System.out.println("yes");
    }
    else{
    System.out.println("NO");
    }
}
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String word=sc.next();
        polindrom(word);
    }
}

```

</details>

# 19 COUNT OF THE THE VOWELS AND CONSONENTS IN THE STRING 

<details>

<summary>CODE</summary>

```java

import java.util.*;
public class solution {
    public static void Count_vowel_conso(String word){
        int countvo=0;
        int countconso=0;
        for(int i=0;i<word.length();i++){
            char k=word.charAt(i);
            if(k=='a'||k=='e'||k=='i'||k=='o'||k=='u'){
                countvo+=1;
            }
            else{
                countconso+=1;
            }
        }
        System.out.println("Count of vowels : "+countvo+"\n"+"Count of consonenets : "+countconso);
    }

    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String word=sc.nextLine();
        Count_vowel_conso(word);
    }
}

```

# Python

```python

def count_of_vowels(word):
    vocount=0
    concount=0
    for i in word:
        if(i=='a'or i=='e'or i=='i'or i=='o'or i=='u'):
            vocount+=1
        else:
            concount+=1
    return ("vowelcount : ", vocount),("consonent count :", concount)
word=input()
print(count_of_vowels(word))

```
</details>

### 3/8/25

# 20 Example String is immutable 
print the string "abracadabra" -> abrackdabra
<details>
<summary>CODE</summary>

# python

```python 

def Strin(name,pos,chr):
    l=list(name)
    l[pos]=chr
    string="".join(l)
    print(string)
Strin("abracadabra",5,"k")

```

</details>


# 21 PRINT THE SECOND HEIGHEST NUMBER IN A LIST 

<details>

<summary>CODE</summary>

```python

def second(n):
    a=[]
    for i in range(1,n+1):
        data=int(input())
        a.append(data)
    for i in range (n-1):
        for j in range(0,n-i-1):
            if(a[j]>a[j+1]):
                temp=a[j]
                a[j]=a[j+1]
                a[j+1]=temp
    if(n>=2):
        if (a[n-1]==a[n-2]):
            print(a[n-3])
        else:
            print(a[n-2])
k=int(input())
second(k)

```

</details>

# 22 print the grade of students by order 

### Explanation

- Given the names and grades for each student in a class of  students, store them in a nested list and print the name(s) of any student(s) having the second lowest grade.

Note: If there are multiple students with the second lowest grade, order their names alphabetically and print each name on a new line.

Example

The ordered list of scores is , so the second lowest score is . There are two students with that score: . Ordered alphabetically, the names are printed as:

alpha
beta
Input Format

The first line contains an integer, , the number of students.
The  subsequent lines describe each student over  lines.
- The first line contains a student's name.
- The second line contains their grade.

Constraints

There will always be one or more students having the second lowest grade.
Output Format

Print the name(s) of any student(s) having the second lowest grade in. If there are multiple students, order their names alphabetically and print each one on a new line.

Sample Input 0

5
Harry
37.21
Berry
37.21
Tina
37.2
Akriti
41
Harsh
39
Sample Output 0

Berry
Harry
Explanation 0

There are  students in this class whose names and grades are assembled to build the following list:

python students = [['Harry', 37.21], ['Berry', 37.21], ['Tina', 37.2], ['Akriti', 41], ['Harsh', 39]]

The lowest grade of  belongs to Tina. The second lowest grade of  belongs to both Harry and Berry, so we order their names alphabetically and print each name on a new line.

<details>

<summary> 👉👉👉Code</summary>

```python
# this code has out of 10 test cases it is faill the 2 test cases
l=[]
n=int(input())
for i in range(1,n+1):
    name=input()
    grade=float(input())
    l.append([grade,name])
g=[]
for i in range(0,len(l)):
    for j in range(0,1):
        g.append(l[i][j])
for i in range(n-1):
    for j in range(n-i-1):
        if(g[j]<g[j+1]):
            tepm=g[j]
            g[j]=g[j+1] 
            g[j+1]=tepm
k=[]
if(n>=2):
    if(g[n-2]==g[n-3]):
        k.append(g[n-2])
        k.append(g[n-3])
    else:
        k.append(g[n-2])

sec=k[0]
name=[]
for student in l:
    if student[0]==sec:
        name.append(student[1])


name.sort()
for i in name:
    print(i)

```

</detials>

# 23 check the missing number in an array (1 to n)

<details>
<Summary>CODE</summary>


```java



```

```python


```

</details>


# 24 DENOMINATION

<details>
<summary>CODE</summary>

```java

import java.util.*;
public class Main{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int total=sc.nextInt();
        int cost=sc.nextInt();
        int change=total-cost;
        
        int n=sc.nextInt();
        int[] denomination=new int[n];
        for (int i=0;i<n;i++){
            denomination[i]=sc.nextInt();
        }
        for (int denom :denomination){
            while(change>=denom){
                System.out.println(denom);
                change-=denom;
            }
        }
    }
}

```

</details>

# 25 finding the how much liters of water we can store in this

#### smaple
- 3,9,1,4,8
- so in this largest second number will be subtract with the other lowest numbers

```java 
5
9 8 2 1 7
14
```

<details>
<summary>CODE</summary>

```java


import java.util.*;

public class Main{
    public static void main (String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];
        
        for (int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }
        for(int i=0;i<n-1;i++){
            for (int j=0;j<n-1-i;j++){
                if(a[j]>a[j+1]){
                    int temp=a[j];
                    a[j]=a[j+1];
                    a[j+1]=temp;
                }
            }
        }
       int max2=a[n-2];
       int sum=0;
       for(int i=0;i<a.length-2;i++){
           sum+=max2-a[i];
       }
           System.out.println(sum);
    }
}

```

</details>


# insert the value in the pirticular index 

<details>
<summary>code</summary>

```java

import java.util.*;

public class Main{
    public static void main (String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n+1];
        
        for (int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }
        int index=sc.nextInt();
        int value=sc.nextInt();
        
        for(int i=n;i>index;i--){
            a[i]=a[i-1];
        }
        a[index]=value;
        
        for (int i=0;i<a.length;i++){
             System.out.print(a[i]+" ");
        }
    }
    
}

```
</details>