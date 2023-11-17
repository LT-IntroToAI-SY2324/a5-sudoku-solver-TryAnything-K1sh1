# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

Breadth first search has better performance in solving the sudoku when the sudoku is not hard and following one path of placing the most likely option into a position will lead you to the end but when thesudoku is hard enough that at multiple points there are multiple possible answers depth first search is more optimal.

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Another algorhithim that might work is if the computer ran multiple boards at the same time and makes a new board for each time a situation where multiple answers could be placed for a solution while the computer is running all boards at the same time it deletes boards that turn up and error and adds new boards until the one complete board is found



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

It could be used for larger puzes as long as you exapnd the code and use a quantum computer to run multiple simulations at the same time, lessons learned from this assignment could be used in predicitve moddling like the effects of a building on the surrounding ares by giving the computer a bunch of causes and running through all the possible effects while changing the way the cause is built until you get the effect with the least damage to the surrounding area


