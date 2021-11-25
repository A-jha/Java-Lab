# String

The **String** is a Datatype in Java, which is not a primitive datatype. it's actually aa **Class**, but it enjoys a bit of favoritism in java to make it easier to ue than a regular class.

A **String** is sequence of characters.A single character is also a string.

Example 1: Print an String

```java
public class Main{
  public static void main(String[] args){
        String quotes = "Give Respect to be Respected";
        System.out.println(quotes);
  }
}
```

Output:

```
Give Respect to be Respected
```

Example 2: Number as String

```java
public class Main{
  public static void main(String[] args){
        float num1 = 25.5f;
        String num2 = "24.5";
        String sum = num1 + num2;
        System.out.println("num1 = "+num1+" num2 = "+num2+" sum = "+ sum);
  }
}
```

Output:

```
num1 = 25.5 num2 = 24.5 sum = 25.524.5
```

- java is smart enough to convert int, float etc to string during such operations.

- We will learn More about String

### [Next](./operator.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
