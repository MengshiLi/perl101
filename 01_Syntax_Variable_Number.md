### 1) Syntax
	
#### Variables:
- No explicit type declaration.
    - e.g. `$x = 10;`
	
#### Expression:
- Anything that returns a value.
    - e.g. literal number
    - e.g. complex expression w/ operators
    - e.g. function calls
	
#### Statements:
- Made up of expressions
- Executed by perl at run-time
- Must be ended with `;`
	
#### Blocks:
- A bunch of **statements** enclosed with `{ }`.
- Variable declared inside a block has its own scope
    - i.e. once the block execution is done, the variable vanishes.
	
#### Comments:
- Started with `#`
- Can start on a new line or append to a statement
- Ignored at compile or run time.
	
#### Whitespace:
- Including spaces, tabs, newlines
- Flexible: doesn't care about whitespace.
    - No need to add `\` for new lines


### 2) Variables:
#### Types:
- Scalars: numbers and strings
- Lists
- Hashes
	
#### Format:
- Start with `$`, followed by a *letter* or `_`
- Case-sensitive
- Only allow *letter*, `_`, *number*
	
#### Declare:
- No need to declare before use --> too loose
- use pragma `strict`: must declare before use.
- Keyword: `my` declares a *lexically-scoped* variable.
    - i.e. only accessible inside its enclosing block (or nested block inside). 
- Keyword: `our`, *global* variables
    - throughout the program or from external packages.
	
#### Scope:		
	
#### Variable Interpolation:
- Variables in double-quoted strings are interpolated, i.e. transform its value (NOT its name) into string.


### 3) Numbers
#### Integers
- Big number seperator: `_`
    - e.g. `$big_data = 123_456_789;`
- Decimal: `123`
- Binary integer: `0b123`
- Octal integer: `0255`
- Hexadecimal integer: `0x255`
	
#### Floating point numbers
- Fixed point: `100.25`
- Scientific:
    - e.g. -1.0025e2 (-100.25)
	- 8Byte width,
	- Range determined by underlay C-lib
