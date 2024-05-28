# Pascal's Triangle Project

## Overview
This project involves implementing a function to generate Pascal’s Triangle up to a given number of rows. Pascal's Triangle is a triangular array of binomial coefficients, where each number is the sum of the two directly above it.

## Must Know

To successfully complete this project, you should revise the following Python concepts:

### Lists and List Comprehensions
- **Lists**: Understand how to create, access, modify, and iterate over lists.
- **List Comprehensions**: Utilize list comprehensions for more concise and readable code, especially for generating rows of Pascal’s Triangle.

### Functions
- **Define and Call Functions**: Know how to define and call functions.
- **Parameters and Return Values**: Pass parameters and return values, particularly how to return a list of lists representing Pascal’s Triangle.

### Loops
- **For and While Loops**: Use for and while loops to iterate through sequences.
- **Nested Loops**: May be necessary for generating each row and calculating the values of Pascal’s Triangle.

### Conditional Statements
- **If, Elif, Else**: Apply conditions to implement logic based on the position within Pascal’s Triangle (e.g., the edges of the triangle always being 1).

### Recursion (Optional)
- **Understanding Recursion**: Provides an alternative approach to generating Pascal’s Triangle.
- **Base Cases and Recursive Cases**: Recognize base cases and recursive cases for a function that generates the triangle’s rows.

### Arithmetic Operations
- **Addition**: Fundamental for calculating each element of Pascal’s Triangle as the sum of the two elements directly above it.

### Indexing and Slicing
- **Access Elements and Slices**: Crucial for identifying and summing the correct elements when constructing each row of the triangle.

### Memory Management
- **Lists Storage and Copying**: Be mindful of how lists are stored and copied, especially when creating new rows based on the values of the previous row.

### Error and Exception Handling (Optional)
- **Try-Except Blocks**: Handle potential errors, such as invalid input types or values.

### Efficiency and Optimization
- **Time and Space Complexity**: Consider the time and space complexity of different approaches to generating Pascal’s Triangle.
- **Performance Optimizations**: Evaluate and apply optimizations to improve the performance of the solution.

By revisiting these concepts, you will be well-prepared to tackle the challenges of implementing Pascal’s Triangle in Python, applying both your mathematical understanding and programming skills to develop an efficient and effective solution.

## Tasks

### 0. Pascal's Triangle
**Mandatory**

Create a function `def pascal_triangle(n):` that returns a list of lists of integers representing Pascal’s triangle of `n`:

- Returns an empty list if `n <= 0`
- You can assume `n` will always be an integer

Example:

```python
guillaume@ubuntu:~/0x00$ cat 0-main.py
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

guillaume@ubuntu:~/0x00$ 
guillaume@ubuntu:~/0x00$ ./0-main.py
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
guillaume@ubuntu:~/0x00$ 
```

## Repository

- **GitHub repository**: `alx-interview`
- **Directory**: `0x00-pascal_triangle`
- **File**: `0-pascal_triangle.py`

## Example Implementation

Here is an example implementation of the `pascal_triangle` function:

```python
def pascal_triangle(n):
    """ Returns a list of lists of integers representing Pascal’s triangle of n. """
    if n <= 0:
        return []

    triangle = [[1]]

    for i in range(1, n):
        row = [1]
        for j in range(1, i):
            row.append(triangle[i-1][j-1] + triangle[i-1][j])
        row.append(1)
        triangle.append(row)

    return triangle
```

This function initializes the triangle with the first row `[1]`, and iteratively builds each subsequent row by summing the appropriate elements from the previous row.
