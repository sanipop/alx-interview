# 0x05. N Queens

## Project Overview

The "0x05. N Queens" project is a classic problem in computer science and mathematics. The objective is to place N non-attacking queens on an N×N chessboard using a backtracking algorithm. This project aims to develop your understanding and implementation skills of algorithms, recursion, and Python programming.

### Key Concepts

1. **Backtracking Algorithms**
   - Understanding how backtracking algorithms work to explore all potential solutions to a problem and backtrack when a solution cannot be completed.
   - **Resources**: 
     - [Backtracking Introduction](https://example.com)

2. **Recursion**
   - Using recursive functions to implement backtracking algorithms.
   - **Resources**:
     - [Recursion in Python](https://example.com)

3. **List Manipulations in Python**
   - Creating and manipulating lists, especially to store the positions of queens on the board.
   - **Resources**:
     - [Python Lists](https://example.com)

4. **Python Command Line Arguments**
   - Handling command-line arguments with the `sys` module.
   - **Resources**:
     - [Command Line Arguments in Python](https://example.com)

### Additional Resources
- [Mock Interview](https://example.com)

## Requirements

### General

- Allowed editors: `vi`, `vim`, `emacs`
- All your files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
- All your files should end with a new line
- The first line of all your files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the PEP 8 style (version 1.7.*)
- All your files must be executable

## Tasks

### 0. N Queens

#### Description

The N queens puzzle is the challenge of placing N non-attacking queens on an N×N chessboard. Write a program that solves the N queens problem.

#### Usage

```sh
./0-nqueens.py N
```

- If the user called the program with the wrong number of arguments, print `Usage: nqueens N`, followed by a new line, and exit with the status 1.
- Where `N` must be an integer greater or equal to 4.
- If `N` is not an integer, print `N must be a number`, followed by a new line, and exit with the status 1.
- If `N` is smaller than 4, print `N must be at least 4`, followed by a new line, and exit with the status 1.
- The program should print every possible solution to the problem.
- One solution per line.
- Format: see example below.
- You don’t have to print the solutions in a specific order.
- You are only allowed to import the `sys` module.

#### Example

```sh
julien@ubuntu:~/0x05. N Queens$ ./0-nqueens.py 4
[[0, 1], [1, 3], [2, 0], [3, 2]]
[[0, 2], [1, 0], [2, 3], [3, 1]]
julien@ubuntu:~/0x05. N Queens$ ./0-nqueens.py 6
[[0, 1], [1, 3], [2, 5], [3, 0], [4, 2], [5, 4]]
[[0, 2], [1, 5], [2, 1], [3, 4], [4, 0], [5, 3]]
[[0, 3], [1, 0], [2, 4], [3, 1], [4, 5], [5, 2]]
[[0, 4], [1, 2], [2, 0], [3, 5], [4, 3], [5, 1]]
julien@ubuntu:~/0x05. N Queens$
```

## Repository

- **GitHub repository**: `alx-interview`
- **Directory**: `0x05-nqueens`
- **File**: `0-nqueens.py`

---

© 2024 ALX, All rights reserved.
