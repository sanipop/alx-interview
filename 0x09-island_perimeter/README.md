# 0x09. Island Perimeter

## Project Overview
This project is part of the curriculum for a short specialization in algorithms and Python programming. It focuses on calculating the perimeter of an island within a grid. The task requires a good understanding of 2D arrays (matrices), conditional logic, and problem-solving strategies.

### Start Date: 
July 29, 2024, 6:00 AM

### End Date: 
August 2, 2024, 6:00 AM

### Checker Release Date:
July 30, 2024, 6:00 AM

### Auto Review:
An automatic review will be launched at the deadline.

## Concepts Needed
- **2D Arrays (Matrices):**
  - Accessing and iterating over elements in a 2D array.
  - Navigating through adjacent cells (horizontally and vertically).
- **Conditional Logic:**
  - Applying conditions to determine whether a cell contributes to the perimeter of the island.
- **Counting Techniques:**
  - Developing a method to count the edges that contribute to the island’s perimeter.
- **Problem-Solving Strategies:**
  - Breaking down the problem into smaller tasks, such as identifying land cells and calculating their contribution to the perimeter.
- **Python Programming:**
  - Using nested loops for iterating over grid cells.
  - Using conditional statements to check the status of adjacent cells.

## Resources
- **Python Official Documentation:**
  - [Nested Lists](https://docs.python.org/3/tutorial/datastructures.html#nested-list-comprehensions): Understanding how to work with lists within lists in Python.
- **GeeksforGeeks Articles:**
  - [Python Multi-dimensional Arrays](https://www.geeksforgeeks.org/python-using-2d-arrays-lists-the-right-way/): A guide to working with 2D arrays in Python effectively.
- **TutorialsPoint:**
  - [Python Lists](https://www.tutorialspoint.com/python/python_lists.htm): Explains how to create, access, and manipulate lists in Python.
- **YouTube Tutorials:**
  - [Python 2D arrays and lists](https://www.youtube.com/results?search_query=python+2d+arrays+and+lists)

## Additional Resources
- Mock Technical Interviews

## Requirements
- **General:**
  - Allowed editors: `vi`, `vim`, `emacs`
  - All files will be interpreted/compiled on Ubuntu 20.04 LTS using Python 3 (version 3.4.3)
  - All files should end with a new line
  - The first line of all files should be exactly `#!/usr/bin/python3`
  - A `README.md` file at the root of the project folder is mandatory
  - Code should adhere to the PEP 8 style (version 1.7)
  - Importing any module is not allowed
  - All modules and functions must be documented
  - All files must be executable

## Tasks
### 0. Island Perimeter (Mandatory)
Create a function `def island_perimeter(grid):` that returns the perimeter of the island described in `grid`:

- `grid` is a list of list of integers:
  - `0` represents water
  - `1` represents land
- Each cell is square, with a side length of 1
- Cells are connected horizontally/vertically (not diagonally).
- `grid` is rectangular, with its width and height not exceeding 100
- The grid is completely surrounded by water
- There is only one island (or nothing).
- The island doesn’t have “lakes” (water inside that isn’t connected to the water surrounding the island).

Example:
```python
#!/usr/bin/python3
"""
0-main
"""
island_perimeter = __import__('0-island_perimeter').island_perimeter

if __name__ == "__main__":
    grid = [
        [0, 0, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 1, 1, 0, 0],
        [0, 0, 0, 0, 0, 0]
    ]
    print(island_perimeter(grid))  # Output: 12
```

## Repository
- **GitHub repository:** `alx-interview`
- **Directory:** `0x09-island_perimeter`
- **File:** `0-island_perimeter.py`

---

© 2024 ALX, All rights reserved.
