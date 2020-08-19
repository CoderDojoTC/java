# Lesson 2

## Repl link

[Lesson 2](https://repl.it/@AaronKorver1/Lesson-2-Variables#Instructions.txt)

## Instructions

Variables are names of things that can change value.  We've seen from lesson one the variable "name" in our Superhero class.

## Syntax

To create a variable you will use the following sytax.

` data_type variable_name = value;`

For our Superhero name we used the following:

`String name = "Groot";`

If you want to set a variable of another object, you can use the "dot" notation.

`objectname.variablename = value;`

## More SuperHero variables

Right now our Superhero has a name, but we need to give it some more information.

Let's add a variable that captures your hero's traits.  For now, we can continue using the data type of `String`.  Next lesson we will discuss different data types.  The first trait we've added is `eyeColor`.  Here are the steps we took to add that property.

1) Add a variable to the Superhero class of type String
1) Set the value of the variable in the Main class
1) Read the value in the `println()` function to print it out.

## Exercise

Think about what things change between different Superheros.  What variables can you add to your Superhero?  Add at least two more variables and print them out.

## Code

```java
class Main {
  public static void main(String[] args) {
    Superhero me = new Superhero();
    me.name = "Groot";
    me.eyeColor = "green";
    System.out.println(me.name);
    System.out.println(me.eyeColor);
  }
}

class Superhero
{
  String name = "";
  String eyeColor = "";
}
```