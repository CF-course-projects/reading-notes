# Arrays, Loops, Imports

## Java Imports
- Package = directory
  - You declare packages when you define your Java program, and you name the packages you want to use from other libraries in an import statement.
- Package declaration syntax
  - Statement order:
    - 1. Package statement (optional)
    - 2. Imports (optional)
    - 3. Class or interface definitions
  - package illusration
  - import java.awt.*;
  - public class Drawing { 
    ...
  }
  - Imports: three options
    - import javax.swing.*; // makes all classes visible tho only one is used.
    - import javax.swing.JOptionPane; // Makes a single class visible
    - We can also use the fully qualified class name without an import
  - Common imports:
    - import java.awt.*; // Commmon GUI elements
    - import java.awt.event.*; // The most common GUI event listeners.
    - import javax.swing.*; // More common GUI elements. Note "javax."
    - import java.util.*; // Data structures (collections), time, Scanner, etc classes.
    - import java.io.*; // Input-output classes.
    - import java.text.*; Some formatting classes.
    - import java.util.regex.&; Regular expression classes.
  - Import FAQ
    - Q: Does importing all classes in a package make my object file larger?
      - A: No, import only tells the compiler where to look for symbols
    - Q: Is it less efficicent to imprt all classes than only the classes I need?
      - A: No. The seach for names is very efficient so there is no effectice difference
    - Q: Why don't I need an import to use String, System, etc?
      - A: All classes in the java.lang package are visible without an impoort.


## Different types of loops in Java
- For Loop: control structure that allows us to repat certain operations by incrementing and evaluating a loop counter.
- While Loop: Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true. 
- Do-While Loop: The do-while loop works just like the while loop except that the first condition evaluation happens after the first iteration of the loopo

