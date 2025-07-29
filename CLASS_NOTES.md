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