# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver
## ************   Sandy W. Zhang   **********
## ************    Feb. 23, 2017   **********

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: *Student should provide answer here*
For each unit, we first single out all the boxes with two digits.  Then for each
of these 2-digit boxes, we will see if there is another identical 2-digit box
within this same unit.  If so, we record the two digits.  Finally go thru the rest
of the boxes within the same unit, to cross out those two digits.  

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: *Student should provide answer here*
For this problem, we don't have to modify much to our regular sudoku problem. All
we have to do is to add the two diagonal units to the unitlist.  Same constraint
propagation: each diagonal unit can't have any digit more than once; it must be
exactly once for each digit.  

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

[My pygame is not working properly.]
Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution. (Done.)
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
