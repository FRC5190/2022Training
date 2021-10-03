# Calculator Program
- Practice writing methods to perform algebraic tasks
- Practice calling and implementing methods from a different class

## Prerequisites
- [Hello World](helloworld.md)

## Instructions
1. Create a new project called `Calculator` and add a new Java Class inside the `src` folder. Name the file `Main`.
Create your `main` method.

2. Create another Java class in your `src` folder. Name it `Calculate`.
   
3. Create four new methods within the `Calculate` file that will compute and return the sum, difference, product, and quotient of two numbers passed to them.
 
4. Add another method that will convert inches to feet. The method should take in one input and return a string stating the total amount of feet as well as the inches left over.

5. Back in the `Main` file, in your `main` method, initialize three variables, create an instance of the `Calculate` class, call each of the five methods using the instance you created, and print the outputs to the console.


## Results
Try it yourself before looking at these!

<details>
    <summary>Code</summary>
        <details>
            <summary>Main.java</summary>

            public class Main {
            
                public static void main(String[] args) {
                    double x = 5.0;
                    double y = 10.0;
                    double inches = 30.0;
                    Calculate calculate = new Calculate();
                    System.out.println(calculate.add(x, y));
                    System.out.println(calculate.subtract(x, y));
                    System.out.println(calculate.multiply(x, y));
                    System.out.println(calculate.divide(x, y));
                    System.out.println(calculate.inchesToFeet(inches));
                }
            }

</details>

<details>
            <summary>Calculate.java</summary>

            public class Calculate {
                public double add(Double x, Double y) {
                    return x + y;
                }
            
                public double subtract(Double x, Double y) {
                    return x - y;
                }
            
                public double multiply(Double x, Double y) {
                    return x * y;
                }
            
                public double divide(Double x, Double y) {
                    return x / y;
                }
            
                public String inchesToFeet(Double x) {
                    int feet = (int) (x / 12);
                    int inchesLeftOver = (int) (x % 12);
                    return feet + " feet and " + inchesLeftOver + " inches";
                }
            }
            
</details>
</details>

<details>
    <summary>Console Output</summary>

    15.0
    -5.0
    50.0
    0.5
    2 feet and 6 inches
    
    Process finished with exit code 0
</details>