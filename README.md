# Sudoku Solver Project (Mathematics + Python)

## Author

Hristina Todorova

## Project Overview

This project explores **Sudoku** as both a mathematical puzzle and a computational problem.

Sudoku is modeled as a **constraint satisfaction problem (CSP)**, where each cell in the grid represents a variable that must satisfy row, column, and subgrid constraints.

The goal of this project is to implement and compare different solving strategies, and to understand how mathematical structure can improve algorithmic performance.

## Motivation

I chose this project because Sudoku is a familiar puzzle, but it reveals interesting mathematical and algorithmic properties when analyzed more deeply.

This makes it a good example of how abstract mathematical ideas can be applied to practical problem-solving.

## Methods Implemented

The project includes the following approaches:

### 1. Backtracking

A recursive algorithm that:

- tries possible values
- checks constraints
- backtracks when a contradiction is found

### 2. Constraint Propagation

A method that:

- reduces possible values for each cell
- fills cells that have only one valid option

### 3. MRV Heuristic (Minimum Remaining Values)

An improvement that:

- selects the most constrained cell first
- reduces the size of the search tree

## Experiments

The algorithms are tested on:

- Easy Sudoku
- Medium Sudoku
- Hard Sudoku

The following metrics are analyzed:

- runtime
- number of recursive calls
- number of assignments
- number of backtracks

## Key Results

- Backtracking is correct but can be slow on harder puzzles
- MRV significantly reduces the number of recursive calls
- Constraint propagation improves efficiency by eliminating unnecessary search

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook sudoku_project.ipynb
```

## Project Structure

- `sudoku_project.ipynb` — main notebook with theory, code, and experiments
- `README.md` — project description
- `requirements.txt` — dependencies

## Conclusion

This project demonstrates that Sudoku is not only a game, but also a structured mathematical problem.

By applying algorithmic techniques such as backtracking, heuristics, and constraint propagation, it is possible to significantly improve solving efficiency.

## Future Work

Possible extensions include:

- implementing more advanced solving strategies
- comparing with SAT solvers or Algorithm X
- building an interactive Sudoku visualizer
