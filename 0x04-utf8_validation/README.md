# 0x04. UTF-8 Validation

## Description

This project involves validating whether a given dataset represents a valid UTF-8 encoding. It applies knowledge in bitwise operations, the UTF-8 encoding scheme, and Python programming.

## Concepts and Resources

### Bitwise Operations in Python
- Understanding how to manipulate bits in Python, including:
  - AND (`&`)
  - OR (`|`)
  - XOR (`^`)
  - NOT (`~`)
  - Shifts (`<<`, `>>`)
- **Resources**:
  - [Python Bitwise Operators](https://docs.python.org/3/library/stdtypes.html#bitwise-operations-on-integer-types)

### UTF-8 Encoding Scheme
- Familiarity with UTF-8 encoding rules, including:
  - How characters are encoded into one or more bytes
  - Patterns that represent a valid UTF-8 encoded character
- **Resources**:
  - [UTF-8 Wikipedia](https://en.wikipedia.org/wiki/UTF-8)
  - [Characters, Symbols, and the Unicode Miracle](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

### Data Representation
- How to represent and work with data at the byte level
- Handling the least significant bits (LSB) of integers to simulate byte data

### List Manipulation in Python
- Iterating through lists
- Accessing list elements
- Understanding list comprehensions
- **Resources**:
  - [Python Lists](https://docs.python.org/3/tutorial/datastructures.html)

### Boolean Logic
- Applying logical operations to make decisions within the program

By studying these concepts and utilizing the resources provided, you will be equipped to tackle the UTF-8 validation project effectively, applying bitwise operations and logical reasoning to determine the validity of UTF-8 encoded data.

### Additional Resource
- [Mock Technical Interview](https://www.interviewbit.com/mock-interview/)

## Requirements

### General
- Allowed editors: `vi`, `vim`, `emacs`
- All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.4.3)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the PEP 8 style (version 1.7.x)
- All your files must be executable

## Tasks

### 0. UTF-8 Validation
**Mandatory**

Write a method that determines if a given data set represents a valid UTF-8 encoding.

- **Prototype**: `def validUTF8(data)`
- **Return**: `True` if data is a valid UTF-8 encoding, else return `False`
- A character in UTF-8 can be 1 to 4 bytes long
- The data set can contain multiple characters
- The data will be represented by a list of integers
- Each integer represents 1 byte of data, therefore you only need to handle the 8 least significant bits of each integer

#### Example
```python
#!/usr/bin/python3
"""
Main file for testing
"""

validUTF8 = __import__('0-validate_utf8').validUTF8

data = [65]
print(validUTF8(data))  # True

data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
print(validUTF8(data))  # True

data = [229, 65, 127, 256]
print(validUTF8(data))  # False
```

## Repository
- **GitHub repository**: `alx-interview`
- **Directory**: `0x04-utf8_validation`
- **File**: `0-validate_utf8.py`
