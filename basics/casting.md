# Arithmetic and Casting

Look at this Problem 💯

```java
public class Main {
   public static void main(String[] args) {
       int intNum = 13;
       byte byteNum = 13;

       int intTotal = intNum / 2;
       byte byteTotal = byteNum / 2;

       System.out.println("Int total = "+intTotal);
       System.out.println("Byte total = "+ byteTotal);
   }
}
```

Error:

```error
Main.java:7: error: incompatible types: possible lossy conversion from int to byte
	byte byteTotal = byteNum / 2;

```

While we are applying arithmetic Operation compiler thinks that the number is int.

## Casting In Java

Casting means to treat or convert a number from one type to another. We put the type we want the number to be in the parenthesis like this

```java
(byte)(byteNum/2);//this tells compiler that after operation the number returned is of byte type
```

**Let's correct the above example**

- We have to Type cast such that after division the result is converted into byte.

```java
public class Main {
    public static void main(String[] args) {
        int intNum = 13;
        byte byteNum = 13;

        int intTotal = intNum / 2;
        byte byteTotal =(byte) (byteNum / 2);

        System.out.println("Int total = "+intTotal);
        System.out.println("Byte total = "+ byteTotal);
    }
}
```

Output:

```
Int total = 6
Byte total = 6
```

**If You don't specify the type the java by default assume it as integer.**

### [Next](./floating.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
