# 0x01. Lockboxes

## Description

This project is part of the ALX software engineering program. It focuses on developing an efficient solution to determine if all boxes in a set can be opened, given certain constraints and initial conditions.

## Learning Objectives

To successfully complete this project, you need a solid understanding of the following key concepts:

### Lists and List Manipulation
- Accessing elements
- Iterating over lists
- Modifying lists dynamically
- [Python Lists (Python Official Documentation)](https://docs.python.org/3/tutorial/datastructures.html)

### Graph Theory Basics
- Traversal algorithms (Depth-First Search or Breadth-First Search)
- Nodes and edges representation
- [Graph Theory (Khan Academy)](https://www.khanacademy.org/computing/computer-science/algorithms#graphs)

### Algorithmic Complexity
- Time and space complexity
- [Big O Notation (GeeksforGeeks)](https://www.geeksforgeeks.org/analysis-of-algorithms-set-1-asymptotic-analysis/)

### Recursion
- Recursive approaches for traversal
- [Recursion in Python (Real Python)](https://realpython.com/python-recursion/)

### Queue and Stack
- Implementing breadth-first search (BFS) or depth-first search (DFS)
- [Python Queue and Stack (GeeksforGeeks)](https://www.geeksforgeeks.org/queue-in-python/)

### Set Operations
- Keeping track of visited boxes and available keys
- [Python Sets (Python Official Documentation)](https://docs.python.org/3/tutorial/datastructures.html#sets)

## Additional Resources

- Mock Technical Interview

## Requirements

### General
- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
- All files should end with a new line
- The first line of all files should be exactly `#!/usr/bin/python3`
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should be documented
- Your code should use the PEP 8 style (version 1.7.x)
- All files must be executable

## Task

### 0. Lockboxes
**Mandatory**

You have `n` number of locked boxes in front of you. Each box is numbered sequentially from `0` to `n - 1` and each box may contain keys to the other boxes.

Write a method that determines if all the boxes can be opened.

- **Prototype:** `def canUnlockAll(boxes)`
- `boxes` is a list of lists
- A key with the same number as a box opens that box
- You can assume all keys will be positive integers
- There can be keys that do not have boxes
- The first box `boxes[0]` is unlocked
- Return `True` if all boxes can be opened, else return `False`

Example usage:
```python
#!/usr/bin/python3

canUnlockAll = __import__('0-lockboxes').canUnlockAll

boxes = [[1], [2], [3], [4], []]
print(canUnlockAll(boxes))  # True

boxes = [[1, 4, 6], [2], [0, 4, 1], [5, 6, 2], [3], [4, 1], [6]]
print(canUnlockAll(boxes))  # True

boxes = [[1, 4], [2], [0, 4, 1], [3], [], [4, 1], [5, 6]]
print(canUnlockAll(boxes))  # False
```

### Repository
- **GitHub repository:** `alx-interview`
- **Directory:** `0x01-lockboxes`
- **File:** `0-lockboxes.py`

---

## Copyright
© 2024 ALX, All rights reserved.
