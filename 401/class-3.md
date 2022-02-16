# Maps, primitives, File I/O

## Primitives vs. Objects
- Autoboxing vs Unboxing:
  - Integer j = 1; // autoboxing
  - int i = new Integer(1); // unboxing
  - The process of converting a primitive type into reference type is called autoboxing, the opposite process is called unboxing.
- Data type memory footprints:
  - boolean: 1 bit
  - byte: 8 bits
  - short, char: 16 bits
  - int, float: 32 bits
  - long, double: 64 bits
  - In practice these can vary from VM.
- Single-element arrays of primitive types are almost always more memory expensive (except for long and double) that the corresponding reference type.

## Exceptions in Java: What is an Exception, the Catch or Specify Requirement, Catching and Handling Exceptions

- What is an Exception?
  - An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions
- The Catch or Specify Requirement
  - Code that may throw an error must be enlosed in a try/catch block
  - Three kinds of Exceptions:
    - checked exception: exceptions that should be anticipated and recovered from easily by the application
    - error: external exception that is not anticipated by the application and usually cannot recover from
    - runtime exception: internal exception that is not anticipated by the applications and usually cannot recover from.

## Using Scanner to read in a fine in Java

- Scanning
  - Objects of type *Scanner* are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.
  - By default, scanners use white space to separate tokens. 
    - To use a diffeent token separator, call *useDelimiter()*, which allows you to use regex.
  
