# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Note on unit test
In unit test, the print results show that I have passed all the cases but the assertion errors are still reported.
I think this may caused by the order of items in dictionary.

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?
A: 
- For each unit, find the boxes with only 2 possible outcomes and add them into a default dict.
- Then if the default dict has a item which appears 2 times , then that is a twin. 
- Then iterating through all boxes in this unit and eliminate the digits that appear in this twin except the twins themselves.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?
A:
- For diagonal sudoku, the only difference is that 2 more units are added in unitlist. So this is changed in variable initialization phase with no change in solution functions.
- The basic solving procedure is reduce, then check, then search.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in function.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
