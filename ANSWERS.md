> ## 1. Reverse number 

<details>
<summary>👉ANSWER</summary>

```java 
import java.util.Scanner;
public class quesionspractice {
    public static int reverse_no(int number){
        int digit,reverse=0;
        while (number!=0) {
            digit=number%10;
            reverse=reverse*10+digit;
            number/=10;
        }
        return reverse;
    }
    public static void main(String[] args) {
        Scanner sc =new Scanner(System.in);
        int num2=12;
        int num1=sc.nextInt();
        int reversed_number=reverse_no(num1);
        System.out.println("Origonal number is : "+num1);
        System.out.println("Reversed number is : "+reversed_number);
    sc.close();
    }
}

```

</details>

----

> ## 2. Check if number is palindrome  

<details>

<summary>👉ANSWER</summary>

```java
import java.util.Scanner;
public class quesionspractice {
public static int Check_palinderome(int a){
    int digit,reverse=0;
    while(a!=0){
        digit=a%10;
        reverse=reverse*10+digit;
        a/=10;
    }
    return reverse;
}
    public static void main(String[] Check_palindrome_number){
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter the number : ");
        int num=sc.nextInt();
        int Reverse_number=Check_palinderome(num);
        System.out.println((num==Reverse_number)? "is palindrome":"Not polindrome");
        sc.close();
    }
}

```

</details>

---

> ## 3. Check if number is Armstrong 

<details>
<summary>👉ANSWER</summary>


```python

def Armstrong(num):
    dup=int(num)
    store=0
    while(dup>0):
        digit=dup%10
        store=store+digit**len(num)
        dup=dup//10
    return store
number=input("Enter the number : ")
dup2=int(number)
return_number=Armstrong(number)
if(dup2==return_number):
    print(number+" is Armstrong number ")
else:
    print(number+" is not Armstrong number ")

```

</details>

---