Tysc Programming Language
========================
Created by: Emil Binoy
Formerly: G##

--- What is Tysc? ---
Tysc is a flexible, easy-to-learn programming language designed for modern microcomputing. 
It supports clean syntax, powerful data structures, loops, conditional statements, functions, classes, exceptions, modules, and more.

--- How to Use ---
1. Write code in a .tysc file.
2. End statements with `#`.
3. Comments:
   - Single-line: ? This is a comment
   - Multi-line: [* This is a multi-line comment *]
4. Run Tysc interpreter to execute the code.

--- Basic Syntax ---
- Constants: Const MAX = 10#
- Variables: x = 5#
- Statement end: # or End

--- Data Types ---
- int, float, str, bool
- list, tuple, mapa, set, slide
- graph, tree, heap, matrix, vector
- void, unin

--- Operators ---
- Arithmetic: + - * / ** !! %
- Comparison: == != < > <= >=
- Logical: and or not
- Bitwise: & | ^ << >>

--- Control Structures ---
- If-Else: omit, el, elv
- Loops: cycle (while), walk (for)
- Switch: lift

--- Loops Examples ---
Inline Initialization:
cycle [x = 0] < 10 #
  vokar//x:#
  x = x + 1#

Classic Style:
x = 0#
cycle x < 10 #
  vokar//x:#
  x = x + 1#

For Loop:
Walk x from 0 to 9 + 1 #
  vokar//x:#

--- Functions ---
Keywords: fun (dox), lam, nl (outer), gl (universal)
fun greet(name) #
  vokar//"Hello, " + name: #

greet "Emil"#

Lambda Example:
lam(x, y) # x + y#
vokar//lam(2, 3):#

--- Classes & Objects ---
Keywords: cls (forma), strct (molde), init (crea), del (dest), pub (libre), pri (privy), pro (comun), ext (hereda), ovr (morf), op (opera), new (nuevo), rm (borra), self (esto), stat (fijo)

cls Person #
  init(name, age) #
    self.name = name#
    self.age = age#

  sayHello() #
    vokar//"Hello, my name is " + self.name: + " and I am " + self.age: + " years old."#

person = new Person "Emil", 30#
person.sayHello()#

--- Exceptions ---
Keywords: try (attempt), exc (catch), fin (ensure), raise (throw), chk (verify)

try #
  x = 5 / 0#
exc e #
  vokar//"Error: " + e.message#
fin #
  vokar//"Always runs"#

raise "CustomError"#

--- Modules & Packages ---
Keywords: load, exload, packet
load math#
result = math.add(2, 3)#
vokar//result#

packet MyPackage #
  fun hello() #
    vokar//"Hi from package!"#

--- Slide Data Structure ---
Create Slide:
slide fruits = ["Apple", "Banana", "Cherry"]#

Add Elements:
fruits >> "Orange" >> "Grapes"#

Insert Elements:
fruits << 1 << "Mango"#

Remove Elements:
fruits -- 2#  # Remove index 2
fruits -- -1# # Remove last

Access Elements:
fruits[0]#  # First element
fruits[-1]# # Last element

Query Slide:
fruits.len#
fruits.empty?#

Transform Slide:
fruits.upper#
fruits.lower#
fruits.join "-"#
fruits.line#

Loop Slide:
walk item in fruits #
  vokar//item:#

--- Notes ---
- End statements with `#`
- Inline and classic loops supported
- Slides use >> push, << insert, -- remove
- Functions, classes, exceptions are easy to type
- Ready for interpreter implementation
