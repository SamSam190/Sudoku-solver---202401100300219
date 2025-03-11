# Sudoku-solver---202401100300219
Introduction:

Sudoku is a logic-based number puzzle game played on
a 9x9 grid. The objective is to fill the grid so that each
row, column, and 3x3 sub grid contains the numbers 1
to 9 without repetition. While simple Sudoku puzzles
can often be solved using logical reasoning, more
complex ones require systematic approaches, such as
algorithmic techniques.
This project presents a Python-based Sudoku Solver
that utilizes the backtracking algorithm. Backtracking is
a recursive technique that explores possible number
placements, checks for validity, and reverses incorrect
choices when necessary. This approach ensures an
efficient solution while strictly adhering to Sudoku
rules.
The solver can be used to solve any valid Sudoku
puzzle and can serve as a useful tool for
educational purposes, puzzle verification, and
automated game-solving applications.

Methodology: 

The Sudoku solver is implemented using a backtracking
algorithm, which is a recursive technique that systematically
explores all possible solutions while ensuring that the Sudoku
rules are followed. The methodology consists of the following
steps:
Identifying Empty Cells
The algorithm scans the 9x9 grid to locate an empty cell
(represented by 0).
Trying Possible Numbers (1 to 9)
The algorithm attempts to place numbers from 1 to 9 in the
empty cell.
Validation Check
Before placing a number, the is_valid() function verifies that it
does not violate Sudoku rules:
The number must not be present in the same row.
The number must not be present in the same column.
The number must not be present in the corresponding 3x3 sub
grid.
Recursive Solving
If a valid number is placed, the function recursively calls itself
to solve the remaining empty cells.
Backtracking (Undo & Retry) :
If no valid number can be placed in a cell, the algorithm
backtracks by resetting the last placed number and trying the
next possibility.
This process continues until the puzzle is fully solved or
determined to be unsolvable.
Solution Verification & Output
If a valid solution is found, the final solved Sudoku board is
displayed.
If no solution exists, an appropriate message is shown.
The backtracking approach ensures an efficient solution by
eliminating incorrect possibilities early, making it one of the
best techniques for solving constraint-based problems like
Sudoku.
