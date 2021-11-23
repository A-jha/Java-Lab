# Variable and Expressions

We can use General expression in Variable like `+, -, *, /, %`.

**Example 1:** Add two Number

```java
package code;

public class Hello {
    public static void main(String[] args) {
        int num1 = 10;
        int num2 = 20;

        int sum = num1 + num2;
        System.out.println(sum);//30
    }
}
```

- Output will be 30

**Example 2:** Calculate simple interest

```java
package code;

public class Hello {
    public static void main(String[] args) {
        int amount = 1000;
        int rate = 2;//2 percent
        int time = 10;// 10 years

        int simpleInterest = (amount * rate * time)/100;
        System.out.println(simpleInterest);
    }
}
```

**Example 3:** Find the remainder and Quotient of division

```java
package code;

public class Hello {
    public static void main(String[] args) {
        int divisor = 10;
        int dividend = 105;
        int quotient = dividend/divisor;
        int remainder = dividend % divisor;

        System.out.println("Quotient is :"+quotient+ " Remainder is :" + remainder);
    }
}
```

- Here + sign usd between string is known as **String concatenation**
- Output : Quotient is :10 Remainder is :5

### [Next](./primitive.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
