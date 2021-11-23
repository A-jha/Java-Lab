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
