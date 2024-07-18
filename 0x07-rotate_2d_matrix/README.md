# 0x07. Rotate 2D Matrix

## Table of Contents

1. [Project Overview](#project-overview)
2. [Concepts Needed](#concepts-needed)
3. [Resources](#resources)
4. [Additional Resources](#additional-resources)
5. [Requirements](#requirements)
6. [Tasks](#tasks)
7. [Usage](#usage)
8. [Repository Structure](#repository-structure)

## Project Overview

For the “0x07. Rotate 2D Matrix” project, you are tasked with implementing an in-place algorithm to rotate an n x n 2D matrix by 90 degrees clockwise. This challenge requires a good understanding of matrix manipulation and in-place operations in Python.

**Project Duration:**  
- **Start:** Jul 15, 2024 6:00 AM
- **End:** Jul 19, 2024 6:00 AM
- **Checker Release:** Jul 16, 2024 6:00 AM

An auto-review will be launched at the deadline.

## Concepts Needed

1. **Matrix Representation in Python:**
   - Understanding how 2D matrices are represented using lists of lists in Python.
   - Accessing and modifying elements in a 2D matrix.

2. **In-place Operations:**
   - Performing operations on data without creating a copy of the data structure.
   - The importance of minimizing space complexity by modifying the matrix in place.

3. **Matrix Transposition:**
   - Understanding the concept of transposing a matrix (swapping rows and columns).
   - Implementing matrix transposition as a step in the rotation process.

4. **Reversing Rows in a Matrix:**
   - Manipulating rows of a matrix by reversing their order as part of the rotation process.

5. **Nested Loops:**
   - Using nested loops to iterate through 2D data structures like matrices.
   - Modifying elements within nested loops to achieve the desired rotation.

## Resources

### Python Official Documentation:
- [Data Structures](https://docs.python.org/3/tutorial/datastructures.html)
- [More on Lists](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists)

### GeeksforGeeks Articles:
- [Inplace rotate square matrix by 90 degrees](https://www.geeksforgeeks.org/inplace-rotate-square-matrix-by-90-degrees/)
- [Transpose a matrix in Single line in Python](https://www.geeksforgeeks.org/transpose-matrix-single-line-python/)

### TutorialsPoint:
- [Python Lists](https://www.tutorialspoint.com/python/python_lists.htm)

By understanding these concepts and utilizing the provided resources, you will be able to approach the problem methodically, first transposing the matrix and then reversing each row to achieve a 90-degree clockwise rotation.

## Additional Resources
- Mock Technical Interview

## Requirements

- **General:**
  - Allowed editors: vi, vim, emacs
  - All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.10)
  - All your files should end with a new line
  - The first line of all your files should be exactly `#!/usr/bin/python3`
  - A `README.md` file, at the root of the folder of the project, is mandatory
  - Your code should use the `pycodestyle` style (version 2.8.0)
  - You are not allowed to import any module
  - All modules and functions must be documented
  - All your files must be executable

## Tasks

### 0. Rotate 2D Matrix
- **Mandatory**
- **Objective:** Given an n x n 2D matrix, rotate it 90 degrees clockwise.
- **Prototype:** `def rotate_2d_matrix(matrix):`
- Do not return anything. The matrix must be edited in-place.
- You can assume the matrix will have 2 dimensions and will not be empty.

```python
#!/usr/bin/python3
"""
Test 0x07 - Rotate 2D Matrix
"""
rotate_2d_matrix = __import__('0-rotate_2d_matrix').rotate_2d_matrix

if __name__ == "__main__":
    matrix = [[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]]

    rotate_2d_matrix(matrix)
    print(matrix)
```

**Expected Output:**
```python
[[7, 4, 1],
 [8, 5, 2],
 [9, 6, 3]]
```

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/alx-interview.git
    ```
2. Navigate to the project directory:
    ```bash
    cd alx-interview/0x07-rotate_2d_matrix
    ```
3. Run the provided test script:
    ```bash
    ./main_0.py
    ```

## Repository Structure

```plaintext
alx-interview/
├── 0x07-rotate_2d_matrix/
│   ├── 0-rotate_2d_matrix.py
│   ├── main_0.py
│   └── README.md
└── ...
```

---

Copyright © 2024 ALX, All rights reserved.
