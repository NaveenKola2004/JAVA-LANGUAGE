# ARRAY

> ## 1. Find the second largest number

<details>
<summary>CODE</summary>

```java

import java.util.*;
public class Arrayquestion {

    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int[] a=new int[n];
        for (int i=0;i<n;i++){
            int data=sc.nextInt();
            a[i]=data;
        }
        // sorting the array by using bubble sort
        for(int i=0;i<n-1;i++){
            for(int j=0;j<n-i-1;j++){
                if(a[j]>a[j+1]){
                    int temp=a[j];
                    a[j]=a[j+1];
                    a[j+1]=temp;
                }
            }
        }
        //getting the largest number or the smallest any number in the array
        if(n>=2){
            System.out.print("Second largest number : "+a[n-2]);
        }
        sc.close();
    }
}

```

</details>

> ## ARRAY ASSENDING ORDER AND DESENDING ORDER

<details>
<summary>CODE</summary>

```java
import java.util.*;
public class Arrayquestion {

    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        System.out.print("Enter the length of array : ");
        int n=sc.nextInt();
        int[] a=new int[n];
        for (int i=0;i<n;i++){
            System.out.print("Enter the "+(i+1)+" data : ");
            int data=sc.nextInt();
            a[i]=data;
        }
        for(int i=0;i<n-1;i++){
            for(int j=0;j<n-i-1;j++){
                if(a[j]>a[j+1]){ //shift  to the less then it will print the descending order
                    int temp=a[j];
                    a[j]=a[j+1];
                    a[j+1]=temp;
                }
            }
        }
        for(int i=0;i<n;i++){
            System.out.print(a[i]+" ");
        }
    }
}

```
</details>


## Check the string is  palindrome


<details>

<summary> CODE</summary>

```python

def palindrome(word):
    data=word
    normal=""
    for i in data:
        normal=i+normal
    return normal
word=input("Enter the word : ")
reword=palindrome(word)

if(word==reword):
    print("IS palindrome")
else:
    print("Not palindrome")

```

# java

```java

import java.util.*;
public class Arrayquestion {
public static boolean ispolindrome(String str){
    str=str.toLowerCase();
    int left=0;
    int right=str.length()-1;
    while(left<right){
        if(str.charAt(left)!=str.charAt(right)){
            return false;
        }
        right--;
        left++;
    }
    return true;
}
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String str=sc.next();
        if(ispolindrome(str)){
            System.out.println("is polindrome");
        }
        else{
            System.out.println("not polindrome");
        }
        sc.close();

    }
}

```

</details>
