*trenyx Grammar*

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

This grammar defines the structure of Trenyx programs, including statements, expressions, declarations, functions, and types.

Designing a standard library for Trenyx involves identifying essential modules and functions to support various programming tasks.

_Trenyx Standard Library (TSL) Proposal_

*Core Modules*

1. `(trenyx.io)` - Input/Output operations (file, console, network)
2. `trenyx.math` - Mathematical functions (algebra, geometry, statistics)
3. `trenyx.string` - String manipulation (parsing, formatting, encoding)
4. `trenyx.collection` - Data structures (lists, maps, sets)
5. `trenyx.util` - Utility functions (logging, debugging, timing)

*Data Structures*

1. `trenyx.list` - Dynamic arrays
2. `trenyx.map` - Hash tables
3. `trenyx.set` - Unordered sets
4. `trenyx.queue` - First-In-First-Out (FIFO) queues
5. `trenyx.stack` - Last-In-First-Out (LIFO) stacks

*File I/O*

1. `trenyx.file.read` - Read file contents
2. `trenyx.file.write` - Write file contents
3. `trenyx.file.append` - Append to file

*Networking*

1. `trenyx.net.tcp` - TCP socket operations
2. `trenyx.net.udp` - UDP socket operations
3. `trenyx.net.http` - HTTP client

*Mathematical Functions*

1. `trenyx.math.sin` - Sine
2. `trenyx.math.cos` - Cosine
3. `trenyx.math.sqrt` - Square root

*String Manipulation*

1. `trenyx.string.split` - Split string
2. `trenyx.string.join` - Join strings
3. `trenyx.string.format` - Format string

*Utility Functions*

1. `trenyx.util.log` - Log message
2. `trenyx.util.debug` - Debug output
3. `trenyx.util.time` - Get current time
