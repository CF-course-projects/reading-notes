# In memory storage

## Understanding the JavaScript Call Stack
- What is a ‘call’?
  - A call is a function invocation
- How many ‘calls’ can happen at once?
  - JavaScript handles one call at a time as a single threaded language.
- What does LIFO mean?
  - Last In First Out
- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
  - Functions get added to the call stack on a first come basis as JavaScript parses through the code line by line.
- What causes a Stack Overflow?
  - Stack Overflow occurs when the maximum callstack is exceeded: usual culprits are infinite loops or unlimited recursive programming. 

## JavaScript error message
- What is a ‘refrence error’?
  - A reference error is when something being referenced is undefined or unaccessable from where it is being referenced.
- What is a ‘syntax error’?
  - A syntax error occurs when something cannot be parsed due to incorrect placement of symbols (parens/curly braces etc)
- What is a ‘range error’?
  - Occurs when trying to access objects beyond their length etc
- What is a 'type' error’?
  - Occurs when trying to perform operations with incompatible data types, ie trying to multiply a string.
- What is a breakpoint?
  - A breakpoint is a place in the program where the code will stop executing. 
- What does the word ‘debugger’ do in your code?
  - breakpoints are created 
