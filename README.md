# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?   
A: When 2 boxes in a unit (squares, rows, columns or diagonals) of sudoku grid are same and have each 2 exactly similar possible digits then 2 digits could only be filled in these boxes called naked twins. We iterate over all the other boxes in grid and remove digits present in naked twins pairs from its list of possible digits thus in a way propagating naked twins constraint to all other boxes in a unit.  

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: We take 2 diagonals as units to satisfy Sudoku constraint and include corresponding diagonal elements in peer list of each box in diagonal. Now whenever there is a box in diagonal solved i.e. only have 1 digit then this digit could not be possible in other boxes of this diagonal. so we remove this digit as possiblity from all other boxes in diagonal.  

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

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
