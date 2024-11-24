Guawa language:powefull code in every bite 

_Syntax and Semantics_

- Consistent naming conventions: camelCase
- Simplified comments: `?` (single-line), `/*,*\` (multi-line)
- Indentation-based code block syntax with clear rules for scope

the lines starting with `?` are comments and are ignored by the Guawa interpreter

*Tab (or four spaces):*

In guawa, indentation (using tabs or four spaces) is used to denote block-level structure. This means that you need to indent your code to indicate where a block of code begins and ends.

*wave (~):*

In guawa, the wave (~) is used to indicate the start of a block of code. It's often used in conjunction with indentation to define the structure of your code

_Keywords_

- `omit` - conditional statement
- `swot` - else clause
- `wot` - elif
- `lift` - switch statement 
- `surge` - while loop
- `torvik` - for loop
- `dox` - function definition
- `vokar` - print function
- `kalt` - input function
- `sygma` - return statement
- `try` - try block
- `catch` - catch block
-`break` -> `exitloop`
-`continue` -> `skip`
-`pass` -> `nop`
-`yield` -> `produce`
-`for` -> `iterate`

_Operators_

- `+` - addition
- `-` - subtraction
- `*` - multiplication
- `/` - division
- `==` - equality
- `!=` - inequality
- `<` - less than
- `>` - greater than
- `<=` - less than or equal
- `>=` - greater than or equal
- `&&` - logical AND
- `||` - logical OR
- `!` - logical NOT
- `**` - exponentiation
- `!!` - floor division
- `%` - modulus
- `&` - bitwise AND
- `|` - bitwise OR
- `^` - bitwise XOR
- `:` - bitwise NOT
- `<<` - left shift
- `>>` - right shift

_Data Types_

- `kal` - integer
- `nexa` - float
- `vix` - string
- `dual` - boolean
- `sek` - list
- `kor` - tuple
- `mapa` - dictionary
- `void` - null
- `unin` - undefined
- `graph` - graph data structure
- `tree` - tree data structure
- `heap` - heap data structure
- `set` - set data structure
- `matrix` - matrix data structure
- `vector` - vector data structure

_Control Structures_

- Conditional statements: `omit`, `swot`
- Loops: `surge`, `torvik`
- Switch statements: `switch`
- Try-catch blocks: `try`, `catch`

*Functions*

Def -> `dox`
Lambda -> `Lamb`
Nonlocal -> `outer`
Global -> `universal`

*Classes and Objects*

- `type` - type definition
- `this` - this parameter
- `lize` - constructor method
- `tost` - string representation
  method
- `tore` - representation method

*Exceptions*

- `attempt` - try block
- `catch` - except block
- `ensure` - finally block
- `throw` - raise statement
- `verify` - assert statement

*Modules and Packages*

- `load` - import statement
- `load ex` - import statement
- `loadfrom` - from statement
- `loas` - as statement
- `namespace` - package statement

*Other*

- `remove` - delete statement
- `execute` - execute statement
- `eval` - evaluate statement
- `using` - with statement
- `async` - asynchronous statement
- `waitfor` - await statement

*New Additions*

- `matrix` - matrix data structure
- `vector` - vector data structure
- `graph` - graph data structure
- `tree` - tree data structure
- `heap` - heap data structure
- `set` - set data structure
- `async` - asynchronous statement
- `await` - await statement
- `try` - try block
- `catch` - catch block
- `finally` - finally block
- `raise` - raise statement
- `assert` - assert statement
- 
In the Guawa programming language, the `lift` statement is used similarly to a `switch` statement in other languages. It allows you to perform different actions based on the value of a variable or expression.

Here's an example of how you might use the `lift` statement in Guawa:
```
vokar("What is your choice? ")
kal choice = kalt()
lift choice
  case 1:
    vokar("You chose option 1!")
  case 2:
    vokar("You chose option 2!")
  case 3:
    vokar("You chose option 3!")
  default:
    vokar("Invalid choice!")
```
In this example, the `lift` statement is used to execute different blocks of code based on the value of the `choice` variable.
