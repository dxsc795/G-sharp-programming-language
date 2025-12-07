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

🔹 Tysc Damnation Binding Full Syntax

1. Purpose

The &> operator binds a key value to a structure or array, producing a damnation mapping.
It is used to create clean, nested mappings for Tysc.


---

2. Single Damnation Binding Syntax

<damnation-binding> ::= <value> "&>" <structure>

<value> → integer, float, string, or variable (acts as the key)

<structure> → array, tuple, nested damnation, or any valid Tysc expression (acts as the value)


Expansion

a &> b  →  { a: b }

Example

x = 5 &> ([2, 7], [5, 7])  ? Bind 5 to the damnation array
vokar(x)                   ? Print the mapping

Output:

{5: ([2, 7], [5, 7])}


---

3. Multiple Damnations

You can create multiple damnation bindings in separate variables or combine them in a list.

d1 = 1 &> ([1,1], [2,2])  ? First damnation
d2 = 2 &> ([3,3], [4,4])  ? Second damnation
all_damn = [d1, d2]       ? Store all in a list
vokar(all_damn)           ? Print the list of mappings

Output:

[{1: ([1, 1], [2, 2])}, {2: ([3, 3], [4, 4])}]


---

4. Nested Damnation

You can nest mappings inside other mappings.

inner = 2 &> ([9,9], [8,8])      ? Inner mapping
outer = 10 &> (inner, [1,0])     ? Outer mapping including inner
vokar(outer)                     ? Print nested damnation

Output:

{10: ({2: ([9, 9], [8, 8])}, [1, 0])}


---

5. Damnation inside Functions

dox makeDamn(x, a, b)             ? Function to create a damnation mapping
    ret x &> (a, b)               ? Return mapping
End #

result = makeDamn(9, [1,9], [8,5]) ? Call function
vokar(result)                      ? Print result

Output:

{9: ([1, 9], [8, 5])}


---

6. Damnation in Loops

? Start counter at 1
i = 1

? Loop while i <= 3
cycle i <= 3
    ? Create a damnation mapping using i
    d = i &> ([i, i+1], [i+2, i+3])

    ? Print mapping for this iteration
    vokar(d)

    ? Increment counter
    i = i + 1
? End of loop

Output:

{1: ([1, 2], [3, 4])}
{2: ([2, 3], [4, 5])}
{3: ([3, 4], [5, 6])}


---

7. Damnation in Conditional Statements

d = 5 &> ([2,7], [5,7])           ? Create mapping

omit 5 == 5
    vokar("Damnation active:", d)  ? Print if condition true
elv
    vokar("No damnation")          ? Else case
#

Output:

Damnation active: {5: ([2, 7], [5, 7])}


---

8. Damnation in Switch (lift) Statements

code = 5

lift code
    case 1
        vokar(1 &> ([0,0], [0,0]))  ? Case 1
    case 5
        vokar(5 &> ([2,7], [5,7]))  ? Case 5
    case default
        vokar("Invalid code")        ? Default case
#

Output:

{5: ([2, 7], [5, 7])}


---

9. Grammar Summary

<statement>        ::= <assignment> | <function> | <loop> | <conditional> | <switch> | <expression>

<assignment>       ::= <identifier> "=" <expression>
<expression>       ::= <damnation-binding> | <value> | <array> | <tuple> | <function-call>

<damnation-binding> ::= <value> "&>" <structure>
<array>            ::= "[" <elements> "]"
<tuple>            ::= "(" <elements> ")"

<elements>         ::= <expression> ("," <expression>)*


---

10. Comments

Single line comment: ? this is a comment

Explains any code line clearly

Must start with ?
