# Lesson 4

## Repl

[Lesson 4](https://repl.it/@AaronKorver1/Lesson-4-Constructor#Main.java)

## Constructors

We have seen how primitive values are created, now we are moving onto objects.

`Superhero me = new Superhero();`

This is an example of creating an object in Java.  There is a special keyword `new` that is used to tell Java that we want to take the class defined by the name `Superhero` and create an object in memory.  Java will use a special method in the class called a Constructor to build the object.

## Default Constructors

If you look at the class right now, you will see that there doesn't look like there is a constructor there!  What is happening?

All classes will by default get an empty constructor added to them by the compiler.  A default constructor looks like this:

```java
Superhero()
{

}
```

## Parameterized Constructors
The second type of constructors is a parameterized constructor.  This is how we can pass values to an object when we create it.  We can also place code in the constructor that runs when the object is created.  The code in the constructor will have access to the values that are passed into it.

## Exercise
We are going to create a parameterized constructor for our superhero.  Let's start by looking at the Superhero class and finding the parameterized constructor.

```java
Superhero(String nameIn)
{

}
```

Next we will need to set the objects name to be the value that was passed in.

```java
Superhero(String nameIn)
{
    name = nameIn;
}
```

Lastly, we need to update where we create our Superhero to pass in the name.

`Superhero me = new Superhero("Groot");`

 We can add more parameters to the constructor, make sure you separate them with a comma.  Let's add the `eyecolor` parameter as well.

```java
Superhero(String nameIn, String eyecolorIn)
{
    name = nameIn;
    eyeColor = eyecolorIn;
}
```

And be sure to update the line of code where you create your Superhero with the new parameter.

You can continue adding more parameters if you would like to your constructor.

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

## Challenge
Create another class called `Superpower`.  Within the `Superpower` class create a variable called `name` and a parameterized constructor for `name`.  Then add a variable of type `Superpower` to the `Superhero` class.  Finally print out the name of your super power in the main method.