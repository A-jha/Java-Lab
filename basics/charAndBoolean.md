# Char and Boolean

## Char

A chart occupies two bytes of memory of 16 bits and thus width of char is 16.**The reason it's not just a single byte is that it allows us to store Unicode characters.**

- Single character
- Written inside single quotes 'A'
- char is a keyword in Java
- Primitive Data Type

### Unicode

Unicode is an international encoding standard for use with different languages and scripts, by which each letter, digit, or symbol is assigned a unique numeric value that applies across different platform and programs.

In English alphabet, We have A to Z. Meaning only 26 characters but in other language need more characters.

Unicode allows us to represent these Language and the way it works is that by using a combination of the Two bytes that a char takes up in memory it can represent and one of 65535 different types of characters.

You can learn more about unicode [here](https://unicode-table.com/en/)

0905 = अ

**Example of Char**

```java
public class Main{
  public static void main(String[] args){
        char normalChar = 'a';
        char unicodeChar = '\u0905';

        System.out.println("normal Char = "+normalChar);
        System.out.println("Unicode char = "+ unicodeChar);
  }
}
```

Output:

```
normal Char = a
Unicode char = अ
```

## Boolean

A boolean value allows for two choices True/1 or False/0. In Java terms we have a boolean primitive type and it can be set to two values only.

Example:

```java
public class Main{
  public static void main(String[] args){
        boolean isFemale = true;
        boolean isKind = false;
        boolean isSlected = false;
        System.out.println("isFemale : "+isFemale+" isKind : "+isKind+" isSelected : "+isSlected);;
  }
}
```

Output:

```
isFemale : true isKind : false isSelected : false
```

Now we have completed All Eight Primitive type in Java

- byte
- short
- int
- long
- float
- double
- char
- boolean

### [Next](./string.md)

<hr/>
<p align="center"> Noted By &copy Avinash Jha</p>
<hr/>
