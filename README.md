Guawa:Powerful coding in every bite

Guawa Language Specification

*Syntax and Semantics*

- Consistent naming conventions: camelCase
- Simplified comments: `//` (single-line), `/* */` (multi-line) replaced with `//` (single-line), `///` (multi-line)
- Clarified code block syntax: indentation-based, with clear rules for scope

*Data Types*

- Added date and time types: `date`, `time`, `datetime`
- Introduced nullable types: `?type` (e.g., `?kal`, `?nexa`)
- Enhanced numeric types: unsigned integer types (`uint`), arbitrary-precision numeric type (`arb`)

*Conditional Statements*

- If Statement: `omit condition: statement`
- Else Statement: `swot: statement`
- If-Else Statement: `omit condition: statement1 swot: statement2`

*Loops*

- While Loop: `surge condition: statement`
- For Loop: `torvik item in collection: statement`

*Functions*

- Function Declaration: `dox function_name(parameters): statement`
- Function Call: `function_name(arguments)`
- Return Statement: `fib value`

*Input/Output*

- Print Statement: `vokar message`
- Input Statement: `kalt prompt`

*Operators*

- Added bitwise operators: `&`, `|`, `^`, `?`
- Considered operator overloading: allowed for user-defined types

*Miscellaneous*

- Module system: introduced (`module`, `into`, `exto`)
- Macros or meta-programming: introduced (`macro`, `meta`)
- Concurrency support: introduced (`async`, `await`)

*Keywords*

- `omit` -> `if`
- `swot` -> `else`
- `surge` -> `while`
- `torvik` -> `for`
- `dox` -> `def`
- `vokar` -> `print`
- `kalt` -> `input`
- `fib` -> `return`
- `threx` -> `and`
- `flux` -> `or`
- `sygma` -> `not`

*Operators*

- `+` (addition)
- `-` (subtraction)
- `*` (multiplication)
- `/` (division)
- `==` (equality)
- `!=` (inequality)
- `<` (less than)
- `>` (greater than)
- `<=` (less than or equal)
- `>=` (greater than or equal)
- `&&` (Logical AND)
- `||` (Logical OR)
- `!` (Logical NOT)
- `&` (bitwise AND)
- `|` (bitwise OR)
- `^` (bitwise XOR)
- `?` (bitwise NOT)

*Data Types*

- `kal` (Integer)
- `nexa` (Float)
- `date` (Date)
- `time` (Time)
- `datetime` (DateTime)
- `?type` (Nullable type)
- `uint` (Unsigned Integer)
- `arb` (Arbitrary-precision numeric)
- `vix` (String)
- `dual` (Boolean)
- `sek` (List)
- `kor` (Tuple)
- `mapa` (Dictionary)
- `void` (Null)
- `unin` (Undefined)

