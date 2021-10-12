# Programming Basics
This will teach you about the basics of programming if you are new and have no clue where to start. 
An important tool to all programmers is a search engine, so there is no shame in looking up concepts 
that you may not understand in-depth.

- Syntax: Grammar of programming languages

## Variables
Variables store pieces of information to be referenced or manipulated.

### Types of Variables:
- `Boolean` - a true or false value
- `Integer` - an integer
- `Double` - any number or decimal
- `String` - a 'string' of text
- `Character` - a single letter/number

There are many other types of variables besides these.

## Methods
Methods are used as a triggerable action, Commonly called functions. Two common uses of functions are `start` and `stop`

## Classes
A class is a template or blueprint used to create a set of objects called instances. 
The class stores data that is shared by all instances, and is the main container of methods and properties.

## Objects
Objects are single instances of a class, and inherit key aspects from the base class. 
Objects can have seperate aspects that make them unique.

## Object-Oriented Programming
OOP is a framework used to clearly organize your code, which helps with reducing redundant code, reusing code, 
troubleshooting, and solving complex programming challenges.

## Example (Using Basic Data Types and Outputs)

public class Main {
    public static void main(String args[]) {
        //Whole Number data types
        byte eByte = 127;
        short eShort = 32767;
        int eInt = 2147483647;
        long eLong = 922337203685475580L;

        //Decimal/Floating point
        float eFloat = 243.1f; //Random number, not max positive value
        double eDouble = 2343.1; //Random number, not max positive value

        //<Type>.MAX_VALUE

        //By Java convention, first letter of variable is always lowercase in order to differentiate a class from a variable.

        System.out.println(eFloat + 1000 + "1000");
        System.out.println(eFloat + eDouble + eByte);
        //How do you print the values on the same line without adding them
        System.out.println(Float.toString(eFloat) + " " + Double.toString(eDouble));

        // Backlash n (to enter)

    }

}

