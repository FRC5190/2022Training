# Integrated Development Environment (IDE)
An IDE is the program you will be using to actually write your code. 
There are many different types of IDEs designed for different languages and developers.

## Jetbrains IntelliJ IDEA
IntelliJ is a powerful IDE primarily designed for `Java` and `Kotlin`.
It has lots of tools to help you program including integration with "Kotlin Koans," a series
of lessons and exercises you will complete later on.
The company behind Intellij, Jetbrains, also has IDEs for numerous other programming languages with the same
"look and feel," though excluding `PyCharm` for `Python` they are generally not as capable as Intellij is with 
`Java` and `Kotlin`.

You can download Intellij at the link [here](https://www.jetbrains.com/idea/download). Select the community edition.

## Visual Studio Code
Visual Studio Code is an IDE that can be used for almost any language.
It is extension based, relying on the community to develop plugins to make coding easier and to add support
This means that it is very lightweight and good for scripting languages.
Visual Studio and Visual Studio Code are different IDEs.

###Getting Started (Intellij): Creating a Project
1. To create a new project in IntelliJ open the program, go to the top left hand corner and click on 
`File` -> `New` -> `Project...` A window should pop up titled "New Project" 
Make sure that the type of project selected is "Java" in the top left hand corner of the window.
2. Click in the "Next" button near the bottom center-right of the window. A new box should appear next to text saying "Create project from template." Click on that box, it should show a checkmark in the box and then select "Command Line App" if it isn't done automatically.
3. Here we name our project, choose it's location, and give it a package name. Make the name of the project whatever the instructions for the lesson tell you to name it. Don't change the "Project location" alone unless you understand file paths and know that you want to save your project to a different location. Set the "Base package" to `org.ghrobotics.yourlastname.yourfirstname` This last part is not strictly neccessary but important for organizational purposes. You can learn more about them [here](). Then click "finish"
4. Finally, there may be a popup asking you if you would like to Open the Project in this window, a new window, or to cancel. "This Window" replaces the current project you are working or whatever screen you are currently on with the new project you just created, saving your previous work and progress. "New Window" will open your project in a seperate window so you can have both whatever you were working on before and your new project open at the same time.

###Getting Started (Intellij): Creating a new Class/File
1. Once your project loads, click on the dropdown on your project folder in the top left hand corner which should show 
the name of the project in bold.
2. Right click the `src` folder and select `New` -> `Java Class` for Java and `New` -> `Kotlin Class/File` for Kotlin.
3. Name the file whatever the assignment you are working on tells you to name it.

## Others
If you prefer another IDE like Eclipse, Netbeans, or no IDE (VIM, Emacs, other text editors) 
you will be able to write code for the robot and complete the training assignments, but you will be largely on your own 
for IDE specific issues. Most programmers on the team either use Jetbrains or Visual Studio Code.