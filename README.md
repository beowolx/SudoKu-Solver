# SudoKu Solver

Sudoku Solver was a very cool project that I developed using
an Algorithm of BackTracking. It can solve any sort of existing SudoKu, no matters the difficult level. It's written in Python.

## The methodology and the algorithm

Backtracking is a general algorithm for finding all (or some) solutions to some computational problems, notably constraint satisfaction problems,that incrementally builds candidates to the solutions, and abandons a candidate ("backtracks") as soon as it determines that the candidate 
cannot possibly be completed to a valid solution. 

Backtracking can be applied only for problems which admit the concept
 of a "partial candidate solution" and a relatively quick test of 
whether it can possibly be completed to a valid solution.  It is 
useless, for example, for locating a given value in an unordered table. 
 When it is applicable, however, backtracking is often much faster than brute force enumeration of all complete candidates, since it can eliminate many candidates with a single test.


Backtracking is an important tool for solving constraint satisfaction problems, such as crosswords, verbal arithmetic, Sudoku, and many other puzzles.  It is often the most convenient (if not the most efficient) technique for parsing, for the knapsack problem and other combinatorial optimization problems.  It is also the basis of the so-called logic programming languages such as  Icon, Planner and Prolog.

When I was wondering about an algorith to use in my program to solve SudoKus, the Backtracking was for me the best option.

In my backtracking algorithm, the program will first start with a sub-solution and if this sub-solution doesn't 
gives a correct final answer, then it'll just come back and change the 
sub-solution. 

The algorithm follows the following steps: 

* If there are no unallocated cells, then the Sudoku is already solved. It will just return true.
* Or else, it will fill an unallocated cell with a digit between 1 to 9
so that there are no conflicts in any of the rows, columns, or the 3x3 
sub-matrices
* Now, it will try to fill the next unallocated cell and if this happens successfully, then it will return true.
* Else, it will come back and change the digit it used to fill the cell. If there is no digit which fulfills the need, then it will just return false as there is no solution of this Sudoku.

## Specifications about the source code 

It's quite a shortcode but very efficient. I've tried to draw a Sudoku's board but the terminal design is not my strong point. If I have time, one day I'll develop a GUI interface for it using python. 

## Tools

* Python 3.8.2 or higher

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

You will only need Python installed on your computer. So you can get it directly from Python's website.



### Installing


Just download the repository here and open it with your TextEditor (I recommend Visual Studio Code).

Then, inside of SudoKuSolver.py, you will find the `board` list that it's responsible to draw the Sudoku board. You'll need to put the numbers of the Sudoku you want to solve on it, where the 0 are the white fields. Be aware to write it exactly as it's in your Sudoku.

After that just run the program and in a few seconds (around 2s) you will have the results.


That's all.



## License / Copyright

* This project is licensed under the MIT License.









