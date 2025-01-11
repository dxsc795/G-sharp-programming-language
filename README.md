G## created by Emil Binoy

The FIT "Flexible In Time" concept suggests that Jetliner exciting two line by two line


Here is the revised document:

G## Programming Language

Syntax and Semantics
- Consistent naming conventions: camelCase

Here's a brief explanation of each symbol:

- `?`: Used for single-line comments.
- `#`: Used to indicate the end of a statement or block, similar to a semicolon in other languages.
- `[* *]`: Used to enclose multi-line comments.
  

And if you'd like to declare a constant:

Const MaxValue = 10
Walk x from 0 to MaxValue
Vokar//(x)
End

The `Const` keyword allows you to declare a constant value, and the `End` In that case, the `End` statement is used to indicate the end of a line or statement, rather than the end of a program or loop.

```
Const MaxValue = 10 End
Walk x from 0 to MaxValue End
Vokar//(x) End
```


Keywords
_Control Structures_
- `kalt` - input
- `vokar` - print
- `omit` - Conditional statement
- `elv` - Else clause
- `el` - Elif statement
- `lift` - Switch statement
- `cycle` - While loop
- `walk` - For loop

_Functions_
- `dox` - Function definition
- `Lamb` - Lambda function
- `outer` - Nonlocal function
- `universal` - Global function

_Classes and Objects_
- `type` - Type definition
- `this` - This parameter
- `lize` - Constructor method
- `tost` - String representation method
- `tore` - Representation method

_Exceptions_
- `attempt` - Try block
- `catch` - Catch block
- `ensure` - Finally block
- `throw` - Raise statement
- `verify` - Assert statement

_Modules and Packages_
- `load` - Import statement
- `exload` - Export statement
- `loadfrom` - From statement
- `loas` - As statement
- `packet` - Package statement

_Other_
- `remove` - Delete statement
- `execute` - Execute statement
- `eval` - Evaluate statement
- `using` - With statement
- `async` - Asynchronous statement
- `waitfor` - Await statement

Data Types
- `int` - Integer
- `float` - Float
- `str` - String
- `bool` - Boolean
- `list` - List
- `tuple` - Tuple
- `mapa` - Dictionary
- `void` - Null
- `unin` - Undefined
- `graph` - Graph data structure
- `tree` - Tree data structure
- `heap` - Heap data structure
- `set` - Set data structure
- `matrix` - Matrix data structure
- `vector` - Vector data structure




Operators
- Arithmetic operators: `+`, `-`, `*`, `/`, `**`, `!!`, `%`
- Comparison operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Logical operators: `and`, `or`, `not`
- Bitwise operators: `&`, `|`, `^`, `<<`, `>>`

Text-to-Speech Keywords
1. `Vocal` - Convert text to speech.
2. `Emotion` - Convey emotions through speech.
3. `Modulate` - Modulate the voice pitch and volume.

Artificial Intelligence/Machine Learning Keywords
1. `Learn` - Train a machine learning model.
2. `Predict` - Make predictions using a trained model.

Internet of Things (IoT) Keywords
1. `Connect` - Connect to a device.
2. `Send` - Send data to a connected device.

Graphics Keywords
1. `Shape` - Draw a shape.
2. `Color` - Set the color.

Security Keywords
1. `Encrypt` - Encrypt data.
2. `Decrypt` - Decrypt data.

Miscellaneous Keywords
1. `Gesture` - Perform a gesture.
2. `Face` - Display a facial expression.
3. `Translate` - Translate text.

Control Structures
_Conditional Statements_
G## supports conditional statements using the `omit` keyword.

```
omit condition #
  ? code to execute if condition is true
elv #
  ? code to execute if condition is false
```

_Loops_
G## supports loops using the `cycle` and `walk` keywords.

```
cycle condition #
  ? code to execute repeatedly while condition is true

walk variable in iterable #
  ? code to execute for each item in the iterable
```

_Switch Statements_
G## supports switch statements using the `lift` keyword.

```
lift expression #
  case value1 #
    ? code to execute if expression equals value1
  case value2 #
    ? code to execute if expression equals value2
  default #
    ? code to execute if expression does not equal any of the cases
```

Functions
*Function Definitions

Here is the revised section on functions:

Functions

_Function Definitions_

In G##, functions are defined using the `dox` keyword.

```
dox functionName(parameters) #
  ? function body
```

_Function Calls_

Functions can be called by their name followed by parentheses containing the arguments.

```
functionName(arguments)
```

_Lambda Functions_

G## also supports lambda functions, which are small anonymous functions.

```
Lamb(parameters) #
  ? lambda function body
```

_Nonlocal Functions_

Nonlocal functions are functions that are defined inside another function.

```
outer functionName(parameters) #
  ? nonlocal function body
```

_Global Functions_

Global functions are functions that are defined outside of any other function.

```
universal functionName(parameters) #
  ? global function body
```

_Function Examples_

Here is an example of a simple function:

```
dox greet(name) #
  vokar("Hello, " + name + "!")

greet("Emil")
```

This will output: "Hello, Emil!"
Here is the rest of the document:

Classes and Objects

_Class Definitions_

In G##, classes are defined using the `type` keyword.

```
type ClassName #
  ? class body
```

_Class Constructors_

Class constructors are special methods that are called when an object is created.

```
lize(parameters) #
  ? constructor body
```

_Class Methods_

Class methods are functions that belong to a class.

```
methodName(parameters) #
  ? method body
```

_Class Properties_

Class properties are variables that belong to a class.

```
property_name = value
```

_Object Creation_

Objects can be created using the `new` keyword.

```
new ClassName(arguments)
```

_Object Examples_

Here is an example of a simple class:

```
type Person #
  lize(name, age) #
    this.name = name
    this.age = age

  sayHello() #
    vokar("Hello, my name is " + this.name + " and I am " + this.age + " years old.")

person = new Person("Emil", 30)
person.sayHello()
```

This will output: "Hello, my name is Emil and I am 30 years old."

Exceptions

_Try-Catch Blocks_

G## supports try-catch blocks for exception handling.

```
attempt #
  ? code that may throw an exception
catch exception #
  ? code to handle the exception
ensure #
  ? code to always execute, regardless of whether an exception was thrown
```

_Throwing Exceptions_

Exceptions can be thrown using the `throw` keyword.

```
throw exception
```

_Assertions_

Assertions can be used to verify that a condition is true.

```
verify condition
```

_Exception Examples_

Here is an example of a try-catch block:

```
attempt #
  x = 5 / 0
catch exception #
  vokar("An error occurred: " + exception.message)
```

This will output: "An error occurred: Division by zero"

Modules and Packages

_Importing Modules_

Modules can be imported using the `load` keyword.

```
load moduleName
```

_Exporting Modules_

Modules can be exported using the `exload` keyword.

```
exload moduleName
```

_Package Management_

G## supports package management using the `packet` keyword.

```
packet packageName #
  ? package contents
```

_Module Examples_

Here is an example of importing a module:

```
load math

result = math.add(2, 3)
vokar//(result)  ? outputs 5
```
Here is the rest of the document:

Standard Library

The G## standard library provides a wide range of functions and classes for various tasks, including:

- Math functions: `add`, `subtract`, `multiply`, `divide`, etc.
- String functions: `concat`, `split`, `replace`, etc.
- Array functions: `sort`, `reverse`, `push`, `pop`, etc.
- Object functions: `keys`, `values`, `entries`, etc.

Best Practices

Here are some best practices for writing G## code:

- Use meaningful variable names and follow a consistent naming convention.
- Use comments to explain your code and make it easier to understand.
- Use functions to organize your code and make it reusable.
- Use classes to define custom data types and organize your code.
- Use exceptions to handle errors and make your code more robust.

Future Development

The G## language is still in development, and there are many features and improvements planned for the future. Some of the planned features include:

- Support for concurrency and parallel programming.
- Support for functional programming.
- Improved support for object-oriented programming.
- A comprehensive standard library.
- A debugger and other development tools.

Conclusion

G## is a powerful and flexible programming language that is designed to be easy to learn and use. With its simple syntax, robust features, and comprehensive standard library, G## is an ideal language for a wide range of applications, from simple scripts to complex systems.

Here is the rest of the document:

Text-to-Speech

G## provides a built-in text-to-speech system that allows you to convert text into spoken words.
Here is the syntax for each keyword:

Artificial Intelligence/Machine Learning
- `Learn>> model_name # dataset` - Train a machine learning model
- `Predict>> model_name # input_data` - Make predictions using a trained model

Internet of Things (IoT)
- `Connect>> device_id # protocol` - Connect to a device
- `Send>> device_id # data` - Send data to a connected device

Graphics
- `Shape>> shape_type # size` - Draw a shape
- `Color>> color_value` - Set the color

Security
- `Encrypt>> data # key` - Encrypt data
- `Decrypt>> encrypted_data # key` - Decrypt data

Miscellaneous
- `Gesture>> gesture_type` - Perform a gesture
- `Face>> face_expression` - Display a facial expression
- `Translate>> text # language` - Translate text
- `Vocal>> text # voice` - Convert text to speech
- `Emotion>> emotion_type # intensity` - Convey emotions through speech
- `Modulate>> pitch # volume` - Modulate the voice pitch and volume


Here is the rest of the document:

Examples

Here are some examples of G## code:

Hello World
```
vokar//("Hello, World!")
```

Conditional Statement
```
x = 5
omit x > 10 #
  vokar//("x is greater than 10")
elv #
  vokar//("x is less than or equal to 10")
```

while Loop
```
x = 0
cycle x < 10 #
  vokar//(x)
  x = x + 1
```

for loop
```
Walk x from 0 to 9 + 1
Vokar(x)
```

Function
```
dox greet(name) #
  vokar//("Hello, " + name + "!")

greet("Emil")
```

Class
```
type Person #
  lize(name, age) #
    this.name = name
    this.age = age

  sayHello() #
    vokar//("Hello, my name is " + this.name + " and I am " + this.age + " years old.")

person = new Person("Emil", 30)
person.sayHello()
```

Glossary

Here is a glossary of G## terms:

- *Class*: A blueprint for creating objects.
- *Conditional statement*: A statement that executes different blocks of code based on conditions.
- *Function*: A block of code that can be called multiple times.
- *Loop*: A statement that executes a block of code repeatedly.
- *Object*: An instance of a class.
- *Variable*: A storage location that holds a value.

References

Here are some references for further learning:

- G## Language Specification
- G## Standard Library
- G## Tutorials

Conclusion

G## is a powerful and flexible programming language that is designed to be easy to learn and use. With its simple syntax, robust features, and comprehensive standard library, G## is an ideal language for a wide range of applications, from simple scripts to complex systems.
