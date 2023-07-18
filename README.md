# Sudoku Solver

Hello, my name is `sonnymay`, and this is my Python project that solves Sudoku puzzles. It uses a backtracking algorithm to fill in the cells in a Sudoku grid and determine the correct solution.

## How it Works

The algorithm starts at the first empty cell in the grid, and begins by placing the number `1` in that cell. It then moves on to the next empty cell and does the same, but if it reaches a cell where `1` is not valid due to the Sudoku rules, it will try `2`, then `3`, and so on, until it finds a number that works or it has tried all numbers up to `9`.

If the algorithm placed `9` in the previous cell and determined that it was not a valid number for the next cell, it will backtrack, i.e., go back to the previous cell, increment the number in that cell by one, and then move forward again. This continues until a solution for the Sudoku puzzle is found or until all possible number combinations in the grid have been exhausted.

## Running the Solver

1. First, clone this repository to your local machine using `git clone https://github.com/sonnymay/sudoku-solver.git`.

2. Navigate into the cloned repository's directory.

3. Run the Python script with the command `python3 main.py`. Please ensure that you have Python3 installed on your machine.

Please note: the Sudoku grid is hardcoded into the Python script. If you want to solve a different puzzle, you will need to modify the `grid` variable in the `main.py` script.

## Limitations

This solver assumes that the input Sudoku puzzle has a valid solution. If the puzzle is unsolvable, the script will not terminate correctly.

## Contributing

If you have suggestions for how I could improve this project, please let me know. Feel free to fork the project and create a pull request with your changes. I am always looking forward to learning and improving.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
