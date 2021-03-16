### (1) String
#### Must be quoted
- Delimiter can be any non-alphabetical and non-numeric characters
- `"any string"`: 
    - Equals to `qq//`, or `qq^^`, or `qq||`, etc
	- variable interpolation
- `'another string'`: 
    - no variable interpolation
	- Equals to `q//`

#### Functions

| Purpose                                | API                                       |
|----------------------------------------|-------------------------------------------|
| Length                                 | `length($s)`                              |
| Lower case                             | `lc($s)`                                  |
| Upper case	                         | `uc($s)`                                  |
| Search substring from a given position | `index($s, $sub, <$pos>)`, `rindex()`     |
| Get / modify substring                 | `substr($s, $offset, $len, $replacement)` |
| Convert string to its number value     | `hex()`, `oct()`                          |
| Encrypt password in one-way fashion    | `crypt()`                                 |
| Return ASCII / UNICODE                 | `chr()`                                   |
| Reverse                                | `reverse()`                               |
| Formats string to be used with print() | `sprintf()`                               |
		

### (2) Operators
#### Operator Precedence
		
#### Numeric operators:
- Arithmetic operator
    - `+`, `-`, `*`, `/`, `**(power)`, `%(mod)`         
- Comparison operators
    - `==`, `!=`, `<`, `<=`, `>`, `>=`
	-  `<=>`: Compare and Return 1, 0, -1 for greater, equal, less, respectively
- Bit-wise operator
    - `&`, `|`, `^`(XOR), `~`(not), `>>`, `<<`

#### String operators
- Comparison operators:
    - `eq`, `ne`, `cmp`, `lt`, `gt`, `le`, `ge`
- Concatenation operators:
    -  `.`, e.g. `"This" . "is"`
    -  `x`, repetition, e.g	`"This" x 4`
    -  `chomp()`, Remove the last char in a string, return the number of characters that were removed.
- Logical Operators
    - `&&`, `||`, `!` 
