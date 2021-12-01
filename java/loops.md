# Loops
- Practice writing for-loops and while-loops
- Practice writing a constructor

## Prerequisites
- [Hello World](helloworld.md)
- [Calculator](calculator.md)

## Instructions
1. Create a new project called `Loops` and a new Java class within your project. Name the file `Main`.
Create your `main` method.

2. Create another Java class within your `src` folder and name it `Loops`. 

3. Create a method called `basicLoops`. Write four separate loops that will...    
    - Part 1: print variable x in 0-10 inclusive
    - Part 2: print variable x in 0-10 not inclusive of 10
    - Part 3: print variable x in 0-10 inclusive skipping every other number
    - Part 4: print variable x in 10-0 inclusive skipping every other number
  
4. Create a method called `forLoops`. Write two separate for loops.    
    - Part 1: declare a list called `colors` of three string elements. Using a for loop, print each element in the list.
    - Part 2: create a new for loop that will iterate through the index and value of each element in `colors`. In the body of your loop, print the index and value in one line.
  
5. Create a method called `whileLoop`. In your method declare an integer variable named `x` set to 0. Set your loop so that it prints the value of `x` while `x` is less than 10. Remember to increase `x` by 1 in the body of the loop. 
     
6. Create a method called `delay`. Add two print statements and add code for a 2 second delay between the statements.
   
7. At the top of your `Loops` class, add an initializing constructor that prints `Initialize`
   
8.  Go back to the file with your `main` method. Inside the `main` method, create an instance of your `Loops` class and then call each of the methods from that class. Print the outputs to the console.

## Results
Try it yourself before looking at these!

<details>
    <summary>Code</summary>
    <details>
        <summary>Main.java</summary>

            public class Main {
                public static void main(String[] args) throws InterruptedException {
                    Loops loopObj = new Loops();
                    loopObj.basicForLoops();
                    loopObj.forLoops();
                    loopObj.whileLoop();
                    loopObj.delay();
                }
            
            }
    
</details>

<details>
    <summary>Loops.java</summary>
    
        import java.util.ArrayList;
        import java.util.List;
        
        public class Loops {
        
            public Loops(){
                System.out.println("Initialize");
            }
        
            public void basicForLoops() {
        
                int x = 0;
        
                System.out.print("\nPart 1: ");
                while (x <= 10) {
                    System.out.print(x);
                    if (x < 10) System.out.print(", ");
                    x++;
                }
        
                x = 0;
        
                System.out.print("\nPart 2: ");
                while (x < 10) {
                    System.out.print(x);
                    if (x < 9) System.out.print(", ");
                    x++;
                }
        
                x = 0;
        
                System.out.print("\nPart 3: ");
                while (x <= 10) {
                    System.out.print(x);
                    if (x < 10) System.out.print(", ");
                    x = x + 2;
                }
        
                x = 10;
        
                System.out.print("\nPart 4: ");
                while (x <= 10 && x >= 0) {
                    System.out.print(x);
                    if (x > 1) System.out.print(", ");
                    x = x - 2;
                }
            }
        
            ;
        
            public void forLoops() {
                System.out.println("\nPart 1: ");
                List<String> colors = new ArrayList<String>();
                colors.add("red");
                colors.add("green");
                colors.add("blue");
                for (String color : colors) System.out.println(color);
        
                System.out.println("Part 2: ");
                for (int i = 0; i < colors.size(); i++) System.out.println(i + ": " + colors.get(i));
            }
        
        
            public void whileLoop() {
                int x = 0;
                while (x < 10) {
                    System.out.println(x);
                    x++;
                }
            }
        
           public void delay() throws InterruptedException {
                System.out.println("FRC5190");
                Thread.sleep(2000);
                System.out.println("Green Hope Falcons");
           }
        
        }
          

</details>
</details>

<details>
    <summary>Console Output</summary>
        <details>
        <summary>basicForLoops</summary>
            
            Initialize
            
            Part 1: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10
            Part 2: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9
            Part 3: 0, 2, 4, 6, 8, 10
            Part 4: 10, 8, 6, 4, 2, 0
            Process finished with exit code 0
</details>
        <details>
        <summary>forLoops</summary>
        
        Initialize
        
        Part 1: 
        red
        green
        blue
        Part 2: 
        0: red
        1: green
        2: blue

        Process finished with exit code 0

</details>

<details>
        <summary>whileLoop</summary>
        
        Initialize
        0
        1
        2
        3
        4
        5
        6
        7
        8
        9
        
        Process finished with exit code 0

</details>


<details>
        <summary>delay</summary>
        
        Initialize
        FRC5190
        Green Hope Falcons
        
        Process finished with exit code 0

</details>
</details>
