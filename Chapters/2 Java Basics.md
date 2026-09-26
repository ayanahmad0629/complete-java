# 2 Java Basics
In this chapter, we will learn about Java basics, like the first class, key terms of Java like JDK, JVM, and more in detail to start making our first code.

![Java-Logo](https://github.com/ayanahmad0629/complete-java/blob/main/Images/Java-Logo.png) 

## 2.1 Intstalling JDK
JDK is the core to make Java programs, containing only the essentials that are heavily required for developers to make programs. To install JDK, follow these steps:
- Search JDK Download in any browser or [Click here](https://www.oracle.com/in/java/technologies/downloads/)
- Make sure to download from the oracle website
- Download the latest version according to your software like Window, macOs, Linux

## 2.2 First Class or Code using Text Editor
To code Java using a text editor, you need Notepad (Windows), GNOME Text Editor or Kate (Linux), or TextEdit (macOS).
Here is the code to make our first output. Try not to copy-paste it yourself. See the code and write it by yourself. 
### Notepad (Windows)
- Open Notepad and type this code [Click here](https://github.com/ayanahmad0629/complete-java/blob/main/Chapters-Code/BasicCode.java)
- Save the file as `BasicCode.java`. Make sure it is not saved as `BasicCode.java.txt`.
- Open Terminal or CMD (press `WIN + R`).
- Locate the folder where you saved the file. For example, if it is on your Desktop, type `cd Desktop`.
- Now compile the Java code using `javac BasicCode.java`.
    - If there are no errors, a new file named `BasicCode.class` will be created on your Desktop. This is the bytecode.
- To get the output, type `java BasicCode`.
### GNOME Text Editor or Kate (Linux)
- Open GNOME Text Editor or Kate and type this code [Click here](https://github.com/ayanahmad0629/complete-java/blob/main/Chapters-Code/BasicCode.java)
- Save the file as `BasicCode.java`. Make sure it is not saved as `BasicCode.java.txt`.
- Open Terminal or CMD (press `Ctrl + Alt + T`).
- Locate the folder where you saved the file. For example, if it is on your Desktop, type `cd Desktop`.
- Now compile the Java code using `javac BasicCode.java`.
    - If there are no errors, a new file named `BasicCode.class` will be created on your Desktop. This is the bytecode.
- To get the output, type `java BasicCode`.
### TextEdit (macOS)
- Open Open TextEdit type this code [Click here](https://github.com/ayanahmad0629/complete-java/blob/main/Chapters-Code/BasicCode.java) 
- Go to TextEdit Settings (or Preferences on older macOS)
- Under New Document select Plain Text instead of Rich text.
- Save the file as `BasicCode.java`. Make sure it is not saved as `BasicCode.java.txt`.
- Locate the folder where you saveRd the file. For example, if it is on your Desktop, type `cd Desktop`.
- Now compile the Java code using `javac BasicCode.java`.
    - If there are no errors, a new file named `BasicCode.class` will be created on your Desktop. This is the bytecode.
- To get the output, type `java BasicCode`.

## 2.3 Compiling and Running
Compiling and running is the process used by Java and many other programming languages. It converts the code you write in a `.java` file into a `.class` file, which is then run by the JVM using JIT (Just-In-Time) compilation to give you the output.

![Compiling-and-Running](https://github.com/ayanahmad0629/complete-java/blob/main/Images/Compiling-and-Running.png)

## 2.4 Anatomy of a Class
Anatomy of a Java Class means understanding the different parts of a class and the different methods used to write Java code, just like learning the structure of the human body. You don't need to understand everything in detail right now; just take a look at what they are used for in simple words.

![Compiling-and-Running](https://github.com/ayanahmad0629/complete-java/blob/main/Images/BasicCode.png)

- First line: `public class BasicCode {`
    - `public`: means it is accessible from anywhere in the program.
    - `class`: tells Java to create a class or a container to hold Java code.
    - `BasicCode`: the name you want to give the class.
    - `{`: the opening bracket that tells Java the class begins here.
- Second line: `public static void main(String[] args) {`
    - This is the main method, where Java starts executing the program.
        - `public`: this makes the method accessible to Java's runtime.
        - `static`: we will cover this later.
        - `void`: means the method does not return anything.
        - `main`: the special name of the method where Java starts executing the program.
        - `(String[] args)`: this tells Java that arguments can be passed to the program from the command line. (Just look at this for now; no need to go deep.)
        - `{`: this tells Java that the main method begins here.
- Third line: `System.out.println("Love isn't just something you feel; love is something you do...");`
    - `System.out.println()`: the code used to print text in the output.
    - `""`: tells Java that this is a string containing characters.
    - `;`: tells Java that the statement has ended. Most Java statements end with a semicolon.
- Fourth line: `}`
    - Tells Java that the main method ends here.
- Fifth line: `}`
    - Tells Java that the class ends here.

## 2.5 File Extensions
### .JAVA
- Contains Java Source Code
- High Level Human Readable
- Used for Development
- File is editable
### .CLASS
- Contains Java Bytecode
- For JVM to convert into Machine code 0/1
- Used for Execution
- Not meant to be edited

## 2.6 JDK vs JRE vs JVM

![JDK-JRE-JVM](https://github.com/ayanahmad0629/complete-java/blob/main/Images/JVM-JDK-JRE.png)

### JDK 
- It's a software development kit required to develop Java applications.
- Includes the JRE, an interpreter/loader (Java), a compiler (javac), a doc generator
  (Javadoc), and other tools needed for Java development.
- Essentially, JDK is a superset of JRE.
### JRE 
- It's a part of the JDK but can be downloaded separately.
- Provides the libraries, the JVM, and other components to run applications.
- Does not have tools and utilities for developers like compilers or debuggers.
### JVM
- It's a part of JRE and responsible for executing the bytecode.
- Ensures Java’s write-once-run-anywhere capability.
- Not platform-independent: a different JVM is needed for each type of OS.

## 2.7 Showing Output

![Showing-Output](https://github.com/ayanahmad0629/complete-java/blob/main/Images/Showing-Output.png)

### `System.out.print("One");`
`print("One");` means the cursor stays on the same line after printing the output.
### `System.out.println("Two");`
`println("Two");` means the cursor moves to a new line after printing the output.
### `System.out.println();`
`println();` creates a new line without printing any text.

## 2.8 Importance of the main method 
### `public static void main(String args[]);`
-  Entry Point: It's the entry point of a Java program, where the execution starts.
   Without the main method, the Java Virtual Machine (JVM) does not know where to
   begin running the code.

- Public and Static: The main method must be public and static, ensuring it's accessible
  to the JVM without needing to instantiate the class.
- Fixed Signature: The main method has a fixed signature: `public static void
  main(String[] args)`. Deviating from this signature means the JVM won't recognize it
  as the starting point.

## 2.9 What is IDE
- IDE stands for Integrated Development Environment.
- A software suite that consolidates the basic tools required for software development.
- A central hub for coding, finding problems, and testing.
- Designed to improve developer efficiency.

### Need for an IDE
- Streamlines development.
- Increases productivity.
- Simplifies complex tasks.
- Offers a unified workspace.

### IDE Features
- Code Autocomplete
- Syntax Highlighting
- Version Control
- Error Checking

### Installing an IDE
You can use any IDE you want, like VS Code or IntelliJ IDEA. I'm going to show you how to set up IntelliJ IDEA because it is great for Java development.

- Search for IntelliJ IDEA.
- Download the latest version from the official JetBrains website. [Click here](https://www.jetbrains.com/idea/download/)
- Make sure to download the version according to your operating system, such as Windows, macOS, or Linux.
- Install it.

### Creating Your First Project
- Click on `New Project`.
- Add a name for your project.
- Select the JDK (Java version).
- Create the project.
- IntelliJ IDEA may add some pre-made code. You can remove it and add our code instead. [Click here](https://github.com/ayanahmad0629/complete-java/blob/main/Chapters-Code/BasicCode.java)
- Click the green Run button at the top to run your code.
