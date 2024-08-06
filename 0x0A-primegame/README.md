# Prime Game

## Project Overview

This project involves solving a game theory problem where two players, Maria and Ben, play a game with consecutive integers. The players take turns choosing prime numbers from the set, and then remove that number and its multiples from the set. The player unable to make a move loses the game. The task is to determine the winner of multiple rounds of the game based on optimal play.

## Concepts Covered

- **Prime Numbers**: Understanding prime numbers and efficient algorithms for identifying them.
- **Sieve of Eratosthenes**: An efficient algorithm for finding all prime numbers up to a given limit.
- **Game Theory**: Basic principles of competitive games and optimal strategies.
- **Dynamic Programming/Memoization**: Optimizing solutions using previously computed results.
- **Python Programming**: Implementing game logic and algorithms using Python.

## Requirements

- **Python Version**: 3.4.3
- **Editors**: vi, vim, emacs
- **PEP 8 Compliance**: Code should follow PEP 8 style guidelines.
- **Executable Files**: All files must be executable.
- **Shebang Line**: Each file should start with `#!/usr/bin/python3`.
- **File Endings**: All files should end with a new line.
- **No External Packages**: You cannot use any external packages.

## Project Tasks

### Task 0: Prime Game

**Description**: Maria and Ben play a game with a set of consecutive integers from 1 to n. They choose a prime number, remove it and its multiples from the set, and the player unable to make a move loses. Determine the winner for multiple rounds of the game.

**Function Prototype**:
```python
def isWinner(x, nums):
```

- `x`: Number of rounds.
- `nums`: List of integers representing the maximum number in each round.

**Return**: Name of the player who won the most rounds. If the winner cannot be determined, return `None`.

**Example**:
```python
x = 3
nums = [4, 5, 1]
```
- **First Round (4)**: Ben wins.
- **Second Round (5)**: Maria wins.
- **Third Round (1)**: Ben wins.

**Result**: "Ben" has the most wins.

## Usage

To run the code, execute the following command:
```bash
./main_0.py
```

## Repository Structure

- **Directory**: `0x0A-primegame`
- **File**: `0-prime_game.py` - Contains the solution for the Prime Game problem.
- **File**: `main_0.py` - Tests the implementation.

## Additional Resources

- **Prime Numbers and Sieve of Eratosthenes**:
  - Khan Academy: [Prime Numbers](https://www.khanacademy.org/math/algebra/x2f8bb115bf2c61e8:prime-numbers)
  - [Sieve of Eratosthenes in Python](https://realpython.com/python-prime-numbers/)
- **Game Theory Basics**:
  - [Game Theory Introduction](https://www.intmath.com/game-theory/)
- **Dynamic Programming**:
  - [What Is Dynamic Programming With Python Examples](https://www.geeksforgeeks.org/dynamic-programming/)

## Copyright

Copyright © 2024 ALX, All rights reserved.
