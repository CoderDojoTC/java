# Lesson 3

## Repl

[Lesson 3](https://repl.it/@AaronKorver1/Lesson-3-Data-types)

## Data Types

Java is a statically typed language. A language is statically typed, if the data type of a variable is known at compile time. This means that you must specify the type of the variable (Declare the variable) before you can use it.

A data type defines the type of values that a variable can have assigned to it. For example if a variable has `int` data type, it can only take integer values. In java we have two categories of data types: 1) Primitive data types 2) Non-primitive data types – Strings and arrays are non-primitive data types.

## Primitive data types

In Java, we have eight primitive data types: boolean, char, byte, short, int, long, float and double.

`byte`, `short`, `int` and `long` data types are used for storing whole numbers.

`float` and `double` are used for fractional numbers.

`char` is used for storing characters(letters).

`boolean` data type is used for variables that holds either true or false.

## Non-primitive data types

Two data types in Java are not considered primitive.  `String` and arrays.  You have already seen how to create a String, but you may be wondering why it is not a primitive.  `String` variables have methods that you can use as well as properties!  We will discuss methods in a later lesson.  But this is the reason that `String` is not considered a primitive.

Arrays are used to describe a list of variables.  Example:

`int arr[]={2,11,45,9};`

this array is a list of `int` and it has four values in it.  Note that you cannot grow or shrink an array.  This makes them a bit inflexible.  They definitely have their place in our toolbox, but we have some better options that provide us more functionality.  We will talk about arrays and lists in a later lesson.

## Exercise
In Lesson 2 we added variables to your Superhero.  The data type we picked for the variables was a `String`.  Look at those variables and decide if they should stay as `String` or if a different data type would be appropriate.  Change or add two variables in your Superhero and use a data type that is NOT a `String`.  In the example below, we have added an "age" variable of type `int`.  Note that primitive values do NOT have any quotes around the value.

## Code

```java
class Main {
  public static void main(String[] args) {
    Superhero me = new Superhero();
    me.name = "Groot";
    me.age = 10;
    System.out.println(me.name);
    System.out.println(me.age);
  }
}

class Superhero
{
  String name;
  int age;
}
```