# Prework

## The Growth Mindset
- Read Upgrade Your Technical Skills with Deliberate Practice. 
  - Deliberate practice can be defined as: Activities designed, typically by a teacher, for the sole purpose of effectively improving specific aspects of an individual’s performance.
  - Key ideas of deliberate practice: 
    - Pushes you just outside your comfort zone
    - Repeated often
    - Feedback on results in continuously available
    - It's highly demanding mentally
    - It's difficult
    - It requires good goals
- Watch Carol Dweck on the Growth Mindset. 
  - Understand the power of 'Yet', with more practice and development, your abilities will grow. Your current abilities are only a reflection of the amount of time and practice you have put in so far.
  - Difficulties and struggles strengthen/develop your abilities the most. 
  - Effort and difficulties are the indicators of growth being made.
- Watch Angela Lee Duckworth on Grit.
  - Grit is often the most determinant factor in long term success when compared to other attributes including intelligence.
  - Grit has also been shown to be inversely related to innate talent. 
  - Grit can be defined as:
    - Having passion and perseverance for very long term goals 
    - Grit is sticking with your vision of the future, day in day out
- Watch Alain de Botton on Redefining Success. 
  - The dominant form of job snobbery today is job snobbery
  - Envy can only occur between relatable individuals
  - You can't be successful in every area of life: A realistic definition of success includes the other areas of life that have been sacrificed 
  - Make sure your concept of success is truly your own.
- Assess your emotional intelligence. If you have done it in the past, now you can identify the areas you have grown in recently
  - I scored 21 in Self-Awareness, 21 in Self-Management, 19 in Social Awareness and 20 in Relationship management. I think that I can improve mostly with my social awareness and my management of relationships with others. Compared to the last time I took this survey, I think that I improved in the Self-Management category. During the curriculum here at CF, I have developed better self-discipline and time management skills. This time around, I’ll work more on developing better relationships with my coursemates and having more social awareness.
- Assess your biases. If you have done it in the past, now you can identify the areas you have grown in recently.
  - I scored 98/120; This is an improved score than the last time I took the assessment in 301. I worked on putting into action the principles of inclusion and bias-management when I encountered it in real life. I made an intentional effort to do so during my collaborative projects in 301. My weakest link is the ‘Empathy and Curiosity’ section. As such, I’ll work on extending more empathy to my colleagues. I’ll try to put myself in their shoes and understand things from their perspective. I’ll also try to indulge my curiosity more with things that I don’t find initial interest in. 

## Practice in the Terminal: 
- Paths: Whenever we refer to file or directory we use one of these two paths
  - Absolute: Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )
  - Relative: Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.
- Path Shortcuts: 
  - (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
  - . (dot) - This is a reference to your current directory. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
  - .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory
- File Manipulation
  - Making a Directory: mkdir \[options] \<Directory>
    - p : tells mkdir to make parent directories as needed
    - v: short for verbose; mkdir logs everytime it makes a parent directory.
  - Ex: 
    - mkdir -pv linuxtutorialwork/foo/bar
    - created directory 'linuxtutorialwork/foo'
    - created directory 'linuxtutorialwork/foo/bar'
- Copying files/directories: cp \[options] \<source> \<destination>
- Moving files/directories: mv \[options] \<source> <destination>
  - To move a file we use the command mv which is short for move. It operates in a similar way to cp. One slight advantage is that we can move directories without having to provide the -r option.
- Removing files/directories: rm \[options] \<file>
  - Option -r: recursive, will remove all nested files/directories within the specified file/directory. 
  - rm -rf \<directory> 
    - f : means no confirmation is needed after running the command
    - This will delete an non-empty directory in one action

## Java Basics

- Primitive datatypes: Types of data built into the system
  - main types:
    - String: must use double quotes “” (Note that Strings are technically objects in Java) 
    - Int: used to categorize WHOLE numbers
    - Double: used for very large/small numbers and decimal points
    - Boolean: used for TRUE or FALSE statements
    - Char: used for characters of any type (letters, space, punctuation mark) MUST BE surrounded by single '' quotation marks
- Method declaration statements: 
  - public: allows other classes to access the method
  - void: there is no return value 
  - signature: the methods name and parameter type
  - Static: You can run the method without creating an instance of it
- Methods:
  - Every Java method has to be within a class
  - Static methods belong to a class while non-static methods belong to objects
  - All parameters to functions are passed by value, primitives content is copied, while objects are not copied and some would say 'passed by reference’
- Array vs ArrayList: 
  - Array:
    - The length must predefined when declaring the array
    - You access/change elements with bracket notation
  - ArrayList
    - Array lists are imported from the java.util.ArrayList package 
    - Dynamic length array
    - CANNOT use bracket notation w/ arrayLists
    - Add elements to the array via .add method
    - Access elements via .get method
    - Delete elements via .remove method
    - Get the index of an element via .indexOf method
  - .length Vs. .length()
    - Use .length for arrays
    - Use .length() for objects/strings (strings are considered objects)


  | Modifier | Class | Package | Child Class | Global | 
  | --- | --- | --- | --- | --- | 
  | public | X | X | X | X |
  | protected | X | X | X |  | 
  | no modifier | X | X |  |  |
  | private | X |  |  |  |

- Classes: 
  - A Java class can inherit fields and methods from another class.
  - Each Java class requires its own file, but only one class in a Java package needs a main() method.
  - Child classes inherit the parent constructor by default, but it’s possible to modify the constructor using super() or override it completely.
  - You can use protected and final to control child class access to parent class members.
  - Java’s OOP principle of polymorphism means you can use a child class object like a member of its parent class, but also give it its own traits.
  - You can override parent class methods in the child class, ideally using the @Override keyword.
  - It’s possible to use objects of different classes that share a parent class together in an array or ArrayList.








