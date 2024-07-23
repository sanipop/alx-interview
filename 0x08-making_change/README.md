# 0x08. Making Change

## Overview

The "0x08. Making Change" project is part of the ALX Curriculum and focuses on solving the classic coin change problem using algorithms. The primary objective is to determine the minimum number of coins required to make up a given total amount, given a list of coin denominations. This project emphasizes the application of greedy algorithms and dynamic programming to devise an efficient and correct solution.

## Learning Objectives

By the end of this project, you should be able to:

- Understand and implement greedy algorithms.
- Recognize scenarios where greedy algorithms might not be optimal.
- Apply dynamic programming principles to solve optimization problems.
- Analyze the time and space complexity of algorithms.
- Break down complex problems into manageable sub-problems.
- Implement efficient looping and conditional statements in Python.

## Concepts Needed

### Greedy Algorithms

- Basic understanding of greedy algorithms.
- Application to the coin change problem.
- Limitations of greedy algorithms in providing optimal solutions.

### Dynamic Programming

- Principles of dynamic programming.
- Concepts of overlapping subproblems and optimal substructure.
- Difference between iterative and recursive approaches.

### Algorithmic Complexity

- Time and space complexity analysis.
- Striving for lower complexity solutions to meet runtime constraints.

### Problem-Solving Strategies

- Breaking down problems into sub-problems.
- Iterative vs recursive approaches in dynamic programming.

### Python Programming

- Manipulating lists and using list comprehensions.
- Efficient function implementation with loops and conditionals.

## Resources

### Python Official Documentation

- [More Control Flow Tools](https://docs.python.org/3/tutorial/controlflow.html)

### GeeksforGeeks Articles

- [Coin Change | DP-7](https://www.geeksforgeeks.org/coin-change-dp-7/)
- [Greedy Algorithm to find Minimum number of Coins](https://www.geeksforgeeks.org/greedy-algorithm-to-find-minimum-number-of-coins/)

### YouTube Tutorials

- [Dynamic Programming - Coin Change Problem](https://www.youtube.com/watch?v=Y0ZqKpToTic)

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
- All files should end with a new line
- The first line of all files should be exactly `#!/usr/bin/python3`
- A `README.md` file at the root of the project folder is mandatory
- Code should use the PEP 8 style (version 1.7.x)
- All files must be executable

## Task

### 0. Change comes from within

**File:** `0-making_change.py`

**Prototype:**
```python
def makeChange(coins, total)
```

**Return:**
- The fewest number of coins needed to meet the total.
- If the total is 0 or less, return 0.
- If the total cannot be met by any number of coins you have, return -1.

**Description:**
- `coins` is a list of the values of the coins in your possession.
- The value of a coin will always be an integer greater than 0.
- Assume an infinite number of each denomination of coin in the list.

**Example:**
```python
#!/usr/bin/python3
"""
Main file for testing
"""

makeChange = __import__('0-making_change').makeChange

print(makeChange([1, 2, 25], 37))  # Output: 7

print(makeChange([1256, 54, 48, 16, 102], 1453))  # Output: -1
```

## Repository

- **GitHub repository:** `alx-interview`
- **Directory:** `0x08-making_change`
- **File:** `0-making_change.py`

---

**Note:** Don't forget to run `$ npm install` when you have the `package.json`.

## Additional Resources

- **Mock Technical Interview**

## License

- © 2024 ALX, All rights reserved.

---
