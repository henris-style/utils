
## Characters

### safe-characters
Convert a string to safe letters. 

**Example:**
input: safe-characters('Bjørk');
output: Bjork
	
### character-set
Receive a list of letters. 
- Used in 'allowed-characters'

**Example:**

| input                    | output                                          |
| ------------------------ | ----------------------------------------------- |
| `character-set(('0-9'))` | `("0" "1" "2" "3" "4" "5" "5" "6" "7" "8" "9")` |

**Options**
| input | output                                                                                         |
| ----- | ---------------------------------------------------------------------------------------------- |
| `a-z` | Returns all letters from a to z lowercase.                                                     |
| `A-Z` | Returns all letters from A to Z uppercase.                                                     |
| `a-Z` | Returns all letters from a to Z lowercase and uppercase.                                       |
| `0-9` | Returns number from 0 to 9.                                                                    |
| `&`   | Returns '&' as a value in the list of allowed characters, this can be done with any character. |

### allowed-characters
Convert a string to a string with allowed-chars. So you can 

## Maps


### map-collect

### map-set
Set a map

### to-map
Convert a list to a map


## Lists / Strings

### prepend
Add a value to the beginning of a list. 

### str-to-list
Convert a string to a list. 

**Arguments**
| argument     | description                                                    |
| ------------ | -------------------------------------------------------------- |
| `$string`    | The string to be separated into a list                         |
| `$separator` | Find this value and break the string every time on this value. |

### list-to-str
Flatten a list and make it into a string. 


**Arguments**
| argument     | description                                     |
| ------------ | ----------------------------------------------- |
| `$list`      | The list to be flattened into a string          |
| `$separator` | After every value the separator will be placed. |

### to-list
Sometimes a list, or map is not the type list. Easily bring it into a list with 'to-list'

### to-letter-list
Convert a string to a list of all letters in the string.

### to-string
If a value is not a string, for instance a number. 'to-string' converts it into a string.

### shortest
Get the shortest of both given values. This can be either the length of a string or the total length of a list.

## Units

### strip-unit
Strip a unit from it's value.


### rem
Wrapper function to convert pixel values to rem

**Example:**

| input           | output                  |
| --------------- | ----------------------- |
| `rem(14)`       | `0.875rem`              |
| `rem(14 16 20)` | `0.875rem 1rem 1.25rem` |

**Arguments**
| input     | output                                            |
| --------- | ------------------------------------------------- |
| `$values` | Accept one value or multiple separated by spaces. |

### rem-calc
Does the calculation for the pixel to rem.

### px
Wrapper function to convert rem values to pixels

**Example:**

| input            | output             |
| ---------------- | ------------------ |
| `px(.75)`        | `12px`             |
| `rem(0.8 1 1.5)` | `12.8px 16px 24px` |

**Arguments**
| argument  | description                                       |
| --------- | ------------------------------------------------- |
| `$values` | Accept one value or multiple separated by spaces. |

### px-calc
Does the calculation for the pixel to rem.
