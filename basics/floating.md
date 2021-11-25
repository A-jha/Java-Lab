# Floating Point Numbers

Unlike whole number, floating point number have fractional part that we express with a decimal point. **3.14159** is an example of floating point number.

Floating point number are also known as real numbers. We use a floating point numbers. We use a floating point number when we need more precision in calculation.

There are two primitive tye in java to store floating point numbers

1. float - Single precision number
2. double - double precision number

### Single and Double Precision

Precision refers to the format and amount of space occupied by the type. Single precision occupies **32 bits**(width of 32) and a Double precision occupies **64 bits**(Width of 64).

As a result the **float** has a range from **1.4E-45 to 3.4028235E+38** and **double** is much more precise with range from **4.9E-324 to 1.7976931948623157E+308.**

## Let's find the range

```java
public class Main {
    public static void main(String[] args) {
        float minFloat = Float.MIN_VALUE;
        float maxFloat = Float.MAX_VALUE;

        double minDouble = Double.MIN_VALUE;
        double maxDouble = Double.MAX_VALUE;

        System.out.println("Minimum Float value = "+minFloat);
        System.out.println("Maximum Float Value = "+maxFloat);
        System.out.println("Minimum Double Value = "+minDouble);
        System.out.println("Maximum Double Value = "+maxDouble);
    }
}
```

Output:

```
Minimum Float value = 1.4E-45
Maximum Float Value = 3.4028235E38
Minimum Double Value = 4.9E-324
Maximum Double Value = 1.7976931348623157E308
```

## Declare and Initialize float and Double

- during initialization we should use suffix
  - f if number is float
  - d if number is double

Example:

```java
public class Main{
  public static void main(String[] args){
        int intNum = 5;
        float floatNum = 5.25f;
        double doubleNum = 5.25d;
        System.out.println(intNum+" "+floatNum+" "+doubleNum);
  }
}
```

Output:

```
5 5.25 5.25
```

**Here is an Interesting problem**

- if d is used and f is removed then then all floating number will be considered as double

```java
public class Main{
  public static void main(String[] args){
        int intNum = 5;
        float floatNum = 5.25;//f is removed
        double doubleNum = 5.25d;
        System.out.println(intNum+" "+floatNum+" "+doubleNum);
  }
}
```

Output--> Error:

```
error: incompatible types: possible lossy conversion from double to float
	float floatNum = 5.25;
	                 ^
```

**We can use the concept of casting to eliminate this error**

```java
public class Main{
  public static void main(String[] args){
        int intNum = 5;
        float floatNum = (float)5.25;// casting used
        double doubleNum = 5.25d;
        System.out.println(intNum+" "+floatNum+" "+doubleNum);
  }
}
```

Output:

```
5 5.25 5.25
```

- Now You better go and add f at the end of float instead of casting.

### Let's apply division

```java
public class Main{
  public static void main(String[] args){
        int intNum = 5;
        float floatNum = 5f;
        double doubleNum = 5d;

        System.out.println("intNum = "+intNum+" floatNum = "+floatNum+" doubleNum = "+doubleNum);

        //apply some division
        int intDiv = intNum / 3;
        float floatDiv = floatNum / 3f;
        double doubleDiv = doubleNum / 3d;

        System.out.println("intDiv = "+ intDiv + " floatDiv = " + floatDiv + " doubleDiv = " + doubleDiv);
  }
}
```

Output:

```
intNum = 5 floatNum = 5.0 doubleNum = 5.0
intDiv = 1 floatDiv = 1.6666666 doubleDiv = 1.6666666666666667
```

- Now You can observe the decimal precision of int, float and double

**Note:** In Java if you deal with decimal number then by default it is of type double and Java is designed in such a way that we do not need to worry about the float and double so feel free to use double every where :).

**TODO:**

1. Write a program to convert fahrenheit to celsius
2. Write a program to find sum of N natural numbers\
3. Write a program to to calculate compound interest

### [Next](./charAndBoolean.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
