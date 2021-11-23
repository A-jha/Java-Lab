# Primitive Types

In Java primitive types are most basic data types. The int is one of eight primitive types.

### The Eight primitive types are

1. boolean
2. byt
3. char
4. short
5. int
6. long
7. float
8. double

# Int

An Int has a Much large range and it occupy **32 bits** and has width of 32.

## Range

In Java Each primitive data type has some range beyond that range it can not store the value.

Java program to find range of integer.

- MIN_VALUE
- MAX_VALUE

```java
public class Main{
    public static void main(String[] args){
        int myInt = 10000;
        int myMinInt = Integer.MIN_VALUE;//return minimum value int can hold
        int myMaxInt = Integer.MAX_VALUE;// maximum value an Integer can Hold
        System.out.println("Minimum Value :"+myMinInt + " Maximum Value :" +myMaxInt);
    }
}
```

Output:

```
Minimum Value :-2147483648 Maximum Value :2147483647
```

## Wrapper Class

Java Uses the concept of a wrapper class for all eight primitive types -in the case of **int**, we can use **integer**, and by doing that it gives us ways to perform operations on an **int**

## Overflow and Underflow

If you try and put a value larger than the maximum value in java, Or a value smaller than the minimum value in java, then you will get an **Overflow** in cas of maximum value and **Underflow** in case of Minimum value.

The computer just skip back to the minimum number or maximum number, which is usually not what we want.

```java
public class Main{
    public static void main(String[] args){
        int myInt = 10000;
        int myMinInt = Integer.MIN_VALUE;//return minimum value int can hold
        int myMaxInt = Integer.MAX_VALUE;// maximum value an Integer can Hold
        System.out.println("Minimum Value :"+myMinInt + " Maximum Value :" +myMaxInt);

        // add 1 to max value
        System.out.println("Busted Minimum Value :"+(myMinInt-1) + "Busted Maximum Value :" +(myMaxInt+1));
    }
}
```

Output:

```
Minimum Value :-2147483648 Maximum Value :2147483647

Busted Minimum Value :2147483647Busted Maximum Value :-2147483648
```

We should always avoid these conditions.

# byte

It is one of the primitive data type in Java.

## Range of Byte

```java
public class Main {
    public static void main(String[] args) {
        byte minByte = Byte.MIN_VALUE;
        byte maxByte = Byte.MAX_VALUE;
        System.out.println("Minimum Byte Value: "+minByte+" and Maximum Byte Value: "+ maxByte);
    }
}
```

Output:

```
Minimum Byte Value: -128 and Maximum Byte Value: 127
```

**Note:** Similar concept is in byte of underflow and Overflow so be aware of that.

Now days computer has a lot of memory that does not mean that we should write a bulky code and smaller range data type are quicker to access and more efficient as well.

## Size of Primitive Type and Width

A Byte occupies 8 bits. A bit is not directly represented in a Primitive type -we have boolean which is not really same. So a Byte occupies 8 bit. We say that a byte has width of 8.

# Sort

Sort can store a large range of number and occupies **16bits**, and has a width of 16.

## Range of Sort

```java
public class Main {
    public static void main(String[] args) {
        short minSort = Short.MIN_VALUE;
        short maxSort = Short.MAX_VALUE;
        System.out.println("Minimum Short Value: "+minSort+" and Maximum Short Value: "+ maxSort);
    }
}
```

Output:

```
Minimum Short Value: -32768 and Maximum Short Value: 32767
```

# long

To declare long we should use uppercase L such that compiler has no confusion.

- Long has width of 64

- L at the end is not Necessary

```java
long normalLong = 1000;
long specifiedLong = 1000L;
```

Output:

```
Normal Long: 1000
Specified as L: 1000
```

## Range of Long

```java
public class Main {
    public static void main(String[] args) {
        long minLong = Long.MIN_VALUE;
        long maxLong = Long.MAX_VALUE;
        System.out.println("Minimum Long Value: "+minLong+" and Maximum Long Value: "+ maxLong);
    }
}
```

Output:

```
Minimum Long Value: -9223372036854775808 and Maximum Long Value: 9223372036854775807
```

**Note:** Each primitive type needs different width int requires 4 time more memory than a byte.

### [Next](./casting.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
