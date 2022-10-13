# Introduction to Sudoku
Sudoku is a Data structure and Algorithm based sudoku validator. These are a suite of C++ programs which deal with Sudoku Puzzles.

# Contents

- Sudoku Solver
    - Overview and Usage
    - How it works ?
- Sudoku Validator
    - Overview and Usage
    - How it works ?
    
# Sudoku Solver
This is a program which solves 9x9 Sudoku puzzles. Written completely in C++ and built wholly from scratch, this program reads input either from a user or from a file containing the Sudoku values and solves the puzzle. It employs concepts such as backtracking and recursion.
## Usage
- Simply download the sudoku-solver.cpp file found in the Sudoku-Solver/ directory. Run it using any standard C++ compiler.
- Once downloaded, compiled and run; the program will require the user to input the Sudoku puzzle into it. There are two ways to do this.

    - The user can either input the values manually one-by-one when the program is running.
    - The user can write all the values into a file, seperated by whitespaces.
    
## How it works ?
- One of the more common methods to solve Sudoku puzzles is "backtracking". I've written a simple algorithm to give an idea of how the program works.

  - Start.
  - We start with the first empty cell.
  - We generate a list of possible valid values that can be filled in that cell.
  - We iterate over this list and start with the first value. This value is placed in the required cell.
  - We move on to the next cell. We again generate a list of possibilities. However, if no list can be generated, then this means that there is something wrong with the      value of the previous cell. We then move back to the previous cell and place the next value on the generated list in the cell now. We repeat this step until the        current cell has a valid value placed inside it.
  - We stop when we reach the 81st cell (the last cell in a Sudoku puzzle) and have placed a valid value.
  - The puzzle has now been solved.
  - Stop.
  
# Sudoku Validator
This is a program which validates solutions for 9x9 Sudoku puzzles. Written completely in C++ and built wholly from scratch, this program takes in input from the user or from a file containing the values.
## Usage
- Simply download the sudoku-validator.cpp file found in the Sudoku-Validator directory. Run it using any standard C++ compiler.
- Once downloaded, compiled and run; the program will require the user to input the Sudoku puzzle into it. There are two ways to do this.
    - The user can either input the values manually one-by-one when the program is running.
    - The user can write all the values into a file, seperated by whitespaces. 
    
## How it works ?
- The workings of the Sudoku Validator are quite simple, to be honest. Here's a simple algorithm explaining them all.
    - Start
    - The values in all the cells are checked to see if they are in the range 1-9. If not, the puzzle is invalid.
    - Every row is checked to see if it contains 1-9 atleast once. If not, the solution is invalid.
    - Every column is checked to see if it contains 1-9 atleast once. If not, the solution is invalid.
    - Every 3x3 grid is checked to see if it contains 1-9 atleast once. If not, the solution is invalid.
    - If all the criteria have been satisfied, the solution is valid.
    - Stop
    
# Future Scope
  - Thinking to build a website or an android application.
      
# Tools
  - Sublime Text
