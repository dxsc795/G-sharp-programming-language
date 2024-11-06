*Ternyx Grammar*

*Terminals*

- `omit` (if)
- `swot` (else)
- `surge` (while)
- `torvik` (for)
- `dox` (def)
- `vokar` (print)
- `kal` (Integer)
- `nexa` (Float)
- `vix` (String)
- `dual` (Boolean)
- `+`, `-`, `*`, `/`, `==`, `!=`, `<`, `>`, `<=`, `>=`
- `(`, `)`, `[`, `]`, `{`, `}`
- `;` (statement separator)
- `.` (period)

*Non-Terminals*

- `Program`
- `Statement`
- `Expression`
- `Declaration`
- `FunctionDefinition`
- `FunctionCall`
- `ParameterList`
- `Variable`
- `Constant`
- `Type`

*Productions*

*Program*

1. `Program` → `Statement*` (a program consists of zero or more statements)

*Statement*

1. `Statement` → `omit` `Expression` `swot` `Statement` (if-else statement)
2. `Statement` → `surge` `Expression` `Statement` (while loop)
3. `Statement` → `torvik` `Variable` `in` `Expression` `Statement` (for loop)
4. `Statement` → `dox` `FunctionDefinition` (function definition)
5. `Statement` → `vokar` `Expression` `;` (print statement)
6. `Statement` → `Declaration` `;` (variable declaration)

*Expression*

1. `Expression` → `Term` `((` `Operator` `Term` )*)` (expression with operators)
2. `Expression` → `FunctionCall` (function call)
3. `Expression` → `Variable` (variable reference)
4. `Expression` → `Constant` (constant value)

*Declaration*

1. `Declaration` → `Type` `Variable` `=` `Expression` (variable declaration)

*FunctionDefinition*

1. `FunctionDefinition` → `FunctionName` `(` `ParameterList` `)` `{` `Statement*` `}` (function definition)

*FunctionCall*

1. `FunctionCall` → `FunctionName` `(` `ExpressionList` `)` (function call)

*ParameterList*

1. `ParameterList` → `Parameter` `(` `Parameter` `)*` (parameter list)
2. `Parameter` → `Type` `Variable` (parameter declaration)

*Variable*

1. `Variable` → `Identifier` (variable name)

*Constant*

1. `Constant` → `IntegerConstant` (integer constant)
2. `Constant` → `FloatConstant` (float constant)
3. `Constant` → `StringConstant` (string constant)
4. `Constant` → `BooleanConstant` (boolean constant)

*Type*

1. `Type` → `kal` (Integer type)
2. `Type` → `nexa` (Float type)
3. `Type` → `vix` (String type)
4. `Type` → `dual` (Boolean type)

*Operator*

1. `Operator` → `+` (addition)
2. `Operator` → `-` (subtraction)
3. `Operator` → `*` (multiplication)
4. `Operator` → `/` (division)
5. `Operator` → `==` (equality)
6. `Operator` → `!=` (inequality)
7. `Operator` → `<` (less than)
8. `Operator` → `>` (greater than)
9. `Operator` → `<=` (less than or equal)
10. `Operator` → `>=` (greater than or equal)

This grammar defines the structure of Ternyx programs, including statements, expressions, declarations, functions, and types.

Designing a standard library for Ternyx involves identifying essential modules and functions to support various programming tasks.

_Ternyx Standard Library (TSL) Proposal_

*Core Modules*

1. `(ternyx.io)` - Input/Output operations (file, console, network)
2. `ternyx.math` - Mathematical functions (algebra, geometry, statistics)
3. `ternyx.string` - String manipulation (parsing, formatting, encoding)
4. `ternyx.collection` - Data structures (lists, maps, sets)
5. `ternyx.util` - Utility functions (logging, debugging, timing)

*Data Structures*

1. `ternyx.list` - Dynamic arrays
2. `ternyx.map` - Hash tables
3. `ternyx.set` - Unordered sets
4. `ternyx.queue` - First-In-First-Out (FIFO) queues
5. `ternyx.stack` - Last-In-First-Out (LIFO) stacks

*File I/O*

1. `ternyx.file.read` - Read file contents
2. `ternyx.file.write` - Write file contents
3. `ternyx.file.append` - Append to file

*Networking*

1. `ternyx.net.tcp` - TCP socket operations
2. `ternyx.net.udp` - UDP socket operations
3. `ternyx.net.http` - HTTP client

*Mathematical Functions*

1. `ternyx.math.sin` - Sine
2. `ternyx.math.cos` - Cosine
3. `ternyx.math.sqrt` - Square root

*String Manipulation*

1. `ternyx.string.split` - Split string
2. `ternyx.string.join` - Join strings
3. `ternyx.string.format` - Format string

*Utility Functions*

1. `ternyx.util.log` - Log message
2. `ternyx.util.debug` - Debug output
3. `ternyx.util.time` - Get current time

*Implementation*

1. Write modules in Ternyx
2. Use Ternyx's foreign function interface (FFI) for external library integration
3. Test and document each module
