# Lesson 1

## Repl link

[Lesson 1](https://repl.it/@AaronKorver1/Lesson-1-Objects)

## Instructions

Welcome to the first lesson.  We are going to talk about Object Oriented Languages and specifically the Java language.

Object Oriented or OO languages are built around the concept of an Object.  We can think of an Object as a container that has a name, it has some properties, and it has some functionality.  The computer can make many copies of an object and give them all different names and different properties.

We describe an object in something called a Class.  A class in Java is a way for us to tell the computer all the different aspects of the object.  The class serves as a template for all the objects that Java will create.  This is easier to show than to read about!

This is a class!  It has a name "Superhero" that we will use to tell Java that we want an object of TYPE "Superhero".  You can see that it has a single property right now, and the property is called "name".

```java
//This class holds our superhero information
class Superhero 
{
  String name = "";
}
```

Here we are creating our first object.  The syntax here is important.  We start with the type of Object we want.  In this case it is "Superhero".  Then we have to give this Object a name.  Each Object needs a unique name.

```java
class Main {
  public static void main(String[] args) {
    //We are going to create a new superhero!
    Superhero myName = new Superhero();
    System.out.println("Hello " + myName.name);
  }
}
```

Rename this Object to be YOUR name.

Now also replace the word "myName" with the same name that you gave your superhero.

Let's run this and see what happens.

You should see "Hello".  Why is that?  Can you read the code and think through it?

Notice that we are using the "name" property of the Superhero.  In our Superhero class, we didn't give this a value!  Let's fix that.

In the Superhero class, set the "name" property to your secret SuperHero name!  My favorite is "Groot".

Now run the code again and see what it prints out.