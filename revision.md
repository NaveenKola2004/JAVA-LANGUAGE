#  Reverse number

```java
import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);

        int num=sc.nextInt();
        int rev=0,digit;
        while(num>0){
           digit=num%10;
           rev=(rev*10)+digit;
           num=num/10;
        }
        System.out.println(rev);
    }
}
```

# Polindrome number 

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);

        int num=sc.nextInt();
        int temp=num;
        int rev=0,digit;
        while(num>0){
           digit=num%10;
           rev=(rev*10)+digit;
           num=num/10;
        }
        if(temp==rev){
            System.out.println("polindrome number");
        }
        else{
            System.out.println("Not polindrome");
        }
    }
}

```

# Armstrong

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);

        int num=sc.nextInt();
        int temp=num;
        int store=0,digit,data;
        int len=(int)(Math.log10(temp)+1);
        while (num>0) {
            digit=num%10;
            data=(int)(Math.pow(digit, len));
            store+=data;
            num/=10;
        }
        
        if(store==temp){
            System.out.println("Armstrong number");
        }
        else{
            System.out.println("not");
        }
    }
}

```


# print armstrong numbers in range 

```java

import java.util.*;
public class CODE_PRACTICE {

    public static int Armstrong(int n){
        int store=0,digit;
        int len=(int)(Math.log10(n)+1);
        while(n>0){
            digit=n%10;
            store=store+((int)Math.pow(digit,len));
            n=n/10;
        }
        return store;
    }
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);

        int number=sc.nextInt();

        for(int i=11;i<=number;i++){
            int temp=i;
            int check=(Armstrong(i));
            if(temp==check){
                System.out.println(check);
            }
        }
        sc.close();
    }
}

```

# Generate Fibonacci series


```java

import java.util.*;

public class CODE_PRACTICE {
    public static void feb(int n){
        int a=0,b=1;
        System.out.print("feb "+a+" "+b);
        for(int i=2;i<n;i++){
            int c=a+b;
            System.out.print(" "+c);
            a=b;
            b=c;
        }
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        feb(n);
        sc.close();
    }
}

```

# Calculate factorial (loop & recursion)

```java

import java.util.*;
public class CODE_PRACTICE {
    public static int fact(int n){

        if(n==0)
        {
            return 1;
        }
        else{
            return n*fact(n-1);
        }
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        System.out.println(fact(num));
        sc.close();
    }
}

```

# Check if number is prime


```java

import java.util.*;

public class CODE_PRACTICE {

    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        boolean isprime=true;
        for(int i=2;i<=Math.sqrt(n);i++){
            if(n%i==0){
                isprime=false;
                break;
            }
        }
        if(isprime){
            System.out.println(n+" is prime number");
        }
        else{
            System.out.println(n+" not prime number");
        }
        sc.close();
    }
}

```

# Count number of digits

```java

import java.util.Scanner;

public class CODE_PRACTICE {
public static int count_digits(int n){
    int count=0;
    while(n>0){
        int digit=n%10;
        count++;
        n=n/10;
    }
    return count;
}

public static void main(String args[]){
    Scanner sc=new Scanner(System.in);
    int n=sc.nextInt();
System.out.println(count_digits(n));
sc.close();
}
}

```

# Sum of digits of a number


```java

import java.util.*;
public class CODE_PRACTICE {
    public static int Sum_of_num(int n){
        int sum=0;
        while(n>0){
            int digit=n%10;
            sum+=digit;
            n/=10;
        }
        return sum;
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        System.out.println(Sum_of_num(n));
    }
}

```

#  Swap two numbers (temp & no temp)

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
         Scanner sc=new Scanner(System.in);
         int num1=sc.nextInt(),num2=sc.nextInt();
         int temp=num1;
         num1=num2;
         num2=temp;

         System.out.println(num1+" "+num2);
    }
}

```

# Without Temp keyword

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int a=5;
        int b=6;

        a=a+b;
        b=a-b;
        a=a-b;
        System.out.println(a+" "+b);
    }
}

```

# by using the binary format

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int a=5;
        int b=6;

       a=a^b;
       b=a^b;
       a=a^b;
       System.out.println(a+" "+b);
    }
}

```



# printing the patterns

## cube hallow and normal

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for (int i=1;i<=n;i++){
            for (int j=1;j<=n;j++){
                if(i==1|| j==1||j==5||i==5){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

```

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for (int i=1;i<=n;i++){
            for (int j=1;j<=n;j++){
                if(i>=1){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

```

# printing the X pattern 

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for (int i=1;i<=n;i++){
            for (int j=1,k=n;j<=n && k>=1;j++,k--){
                if(i==j || i==k){  // pring the  X symbole
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

```

# Right angled triangle

### condition  if (j<=i)

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1,k=n;j<=n && k>=1;j++,k--){
                if(j<=i){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

*         
* *       
* * *     
* * * *   
* * * * *

```

# Flipped Right angled triangle
### Condition if (j<=n-i+1)

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1,k=n;j<=n && k>=1;j++,k--){
                if(j<=n-i+1){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

* * * * * 
* * * *   
* * *     
* *       
*

```

# Left angled Triangle

### if (j>=n-i+1)

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1,k=n;j<=n && k>=1;j++,k--){
                if(j>=n-i+1){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

        * 
      * * 
    * * * 
  * * * * 
* * * * * 

```

# Flipped Left angled triangle
### if(j>=i)

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1,k=n;j<=n && k>=1;j++,k--){
                if(j>=i){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

* * * * * 
  * * * *
    * * *
      * *
        *

```

# Triangle (pyramid) 
### inner loop (for (int j=1;j<=2*n-1;j++))
### if(j>=n-i+1 && j<=n+i-1)

```java

public class CODE_PRACTICE {

    public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1;j<= 2 * n-1;j++){
                if(j>=n-i+1 && j<=n+i-1){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

        *
      * * *
    * * * * *
  * * * * * * *
* * * * * * * * *

```

# Flipped Triangle
### Inner loop ((for int j=1;j<=2*n-1;j++))
### condition if(j>=i && j<2*n-i)

```java

public class CODE_PRACTICE {
public static void main(String[] args) {
        int n=5;
        for(int i=1;i<=n;i++){
            for(int j=1;j<= 2 * n -1 ;j++){
                if(j>=i && j<=2*n-i){
                    System.out.print("* ");
                }
                else{
                    System.out.print("  ");
                }
            }
            System.out.println();
        }
    }
}

// OUTPUT

* * * * * * * * * 
  * * * * * * *
    * * * * *
      * * *
        *

```

# Floyd’s triangle
# inner loop ((for int j=1;j<=i;j++))

```java

public class CODE_PRACTICE {
public static void main(String[] args) {
        int n=5;
        int num=1;
        for(int i=1;i<=n;i++){
            for(int j=1;j<=i;j++){
                System.out.print(num+" ");
                num++;
            }
            System.out.println();
        }
    }
}

// OUTPUT

1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15 

```

# Flipped Floyd’s triangle
# outer loop ((for int i=n;i>=1;i--))

```java

public class CODE_PRACTICE {
public static void main(String[] args) {
        int n=5;
        int num=1;
        for(int i=n;i>=1;i--){
            for(int j=1;j<=i;j++){
                System.out.print(num+" ");
                num++;
            }
            System.out.println();
        }
    }
}
// OUTPUT

1 2 3 4 5 
6 7 8 9 
10 11 12 
13 14 
15 

```



> # ARRAY

# Find largest and smallest in array

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];

        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }

        for(int i=0;i<n-1;i++){
            for(int j=0;j<n-i-1;j++){
                if(a[j]>a[j+1]){
                    int temp=a[j+1];
                    a[j+1]=a[j];
                    a[j]=temp;
                }
            }
        }
        System.out.println(a[n-1]+" is largest number");
        System.out.print(a[n-n]+" is smallest number");
    }
}

```

# Sum of all array elements

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];

        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }

        int sum=0;
        for (int i=0;i<n;i++){
            sum+=a[i];
        }
        System.out.println(sum);
        sc.close();
    }
}

```

# Find second largest number

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];

        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }

        for (int i=0;i<n-1;i++){
            for(int j=0;j<n-i-1;j++){
                if(a[j]>a[j+1]){
                    int temp=a[j+1];
                    a[j+1]=a[j];
                    a[j]=temp;
                }
            }
        }
        System.out.println(a[n-2]);
        sc.close();
    }
}

```

# Sort array (Bubble, Insertion, Selection)

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];

        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }

        for (int i=0;i<n-1;i++){
            for(int j=0;j<n-i-1;j++){
                if(a[j]>a[j+1]){
                    int temp=a[j+1];
                    a[j+1]=a[j];
                    a[j]=temp;
                }
            }
        }
        for (int i=0;i<n;i++){
            System.out.println(a[i]);
        }
        sc.close();
    }
}

```
# Count even and odd numbers

```java

import java.util.*;
public class CODE_PRACTICE {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];

        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }

        int even=0,odd=0;
        for(int i=0;i<n;i++){
            if((a[i] & 1)==0){
                even++;
            }
            else{
                odd++;
            }
        }
        System.out.println(even +" even numbers \n"+odd+" odd numbers");
        sc.close();
    }
}

```


# FREQUENCY ARRAY
### Basic way to create the Frequency
```java

public class practice {

    public static void main(String[] args) {
        int[] a={0,1,2,2,3,4,5,6,7};
        int[] c=new int[100];

        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int i=0;i<c.length;i++){
            if(c[i]==1){
                System.out.print(i);
            }
        }
    }
}

```

# 1. Unique elements from numbers

### Condition if(c[i]==1)

```java

public class practice {

    public static void main(String[] args) {
        int[] a={1,1,2,2,3,4,5,6,6};
        int[] c=new int[100];

        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int i=0;i<c.length;i++){
            if(c[i]==1){
                System.out.print(i+" ");
            }
        }
    }

}

```

# Duplicate elements
### Condition if(c[i]>1)

```java

public class practice {

    public static void main(String[] args) {
        int[] a={1,1,2,2,3,4,5,6,6};
        int[] c=new int[100];

        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int i=0;i<c.length;i++){
            if(c[i]>1){
                System.out.print(i+" ");
            }
        }
    }
}

```

# Missing elements (don’t appear at all)
### Condition if(c[i]==0)

```java

public class practice {

    public static void main(String[] args) {
        int[] a={1,1,2,2,3,4,5,6,6};
        int[] c=new int[100];

        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int i=0;i<c.length;i++){
            if(c[i]==0){
                System.out.print(i+" ");
            }
        }
    }
}

```

# Elements appearing at most k times example k=2
### condition id(c[i]>=2 && c[i]>0)

```java

public class practice {

    public static void main(String[] args) {
        int[] a={1,1,2,2,3,4,5,6,6};
        int[] c=new int[100];

        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int i=0;i<c.length;i++){
            if(c[i]>=2 && c[i]>0){
                System.out.print(i+" ");
            }
        }
    }
}

```

# Sorting numbers by occurrence
### condition for(int freq=1;freq<=a.length;freq++)
### condition if(c[i]==freq)
### condition for(int k=0;k<freq;k++)

```java

public class practice {
    public static void main(String[] args) {
        int[] a={1,1,2,2,3,4,5,6,6};
        int[] c=new int[100];
        for(int i=0;i<a.length;i++){
            c[a[i]]++;
        }
        for(int freq=1;freq<=a.length;freq++){
            for(int i=0;i<c.length;i++){
                if(c[i]==freq){
                    for(int k=0;k<freq;k++)
                    System.out.print(i+" ");
                }
            }
        }
    }
}

```

# Sorting numbers ascending
### 