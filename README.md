# N-Queens Problem: A* Search vs. Constraint Satisfaction Problem (CSP)

This project explores two different Artificial Intelligence approaches to solve the classic **N-Queens Puzzle**. The objective is to place $N$ chess queens on an $N \times N$ chessboard so that no two queens threaten each other (no two queens share the same row, column, or diagonal).

## 🧩 Problem Description
The N-Queens problem is a well-known combinatorial challenge used to test search algorithms and optimization solvers. In this project, we represent the board as an array of $N$ integers, where the index represents the column and the value represents the row of the queen in that column.

We compare two paradigms:
1. **State-Space Search (A*)**: Fixing queens in columns and moving them across rows to minimize conflicts using a heuristic function.
2. **Constraint Satisfaction Problem (CSP)**: Modeling the board as a set of variables and constraints, solved using the Google OR-Tools CP-SAT solver.

## 🚀 Project Features
- **A* Algorithm Implementation**: Uses a custom heuristic (number of attacking pairs) and optimal search strategies (duplicate elimination).
- **CSP Modeling**: Implements global constraints (`AllDifferent`) for rows and diagonals.
- **Performance Analysis**: A comprehensive test suite comparing execution time, nodes expanded (A*), and internal solver metrics like branches and conflicts (CSP).
- **Visualization**: Graphical representation of the board in the console and data analysis visualization using Matplotlib and Pandas.

## 🛠 Requirements
To run the Jupyter Notebook or Python scripts, you need the following dependencies:

- **Python 3.7+**
- **OR-Tools**: Google's specialized solver for CP problems.
- **Pandas**: For data manipulation and summary tables.
- **Matplotlib**: For generating performance charts.

You can install the required libraries using pip:
```bash
pip install ortools pandas matplotlib