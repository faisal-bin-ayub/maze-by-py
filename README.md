# Maze Solver

This project implements a maze-solving algorithm using depth-first search (DFS) or breadth-first search (BFS) to find a path from a starting point ('A') to a goal point ('B') in a text-based maze.

## Features

- Reads maze from a text file.
- Visualizes the maze and the solution.
- Outputs the number of states explored during the search.

## Requirements

- Python 3.x
- Pillow (for image generation)

>You can install the required package using pip:
pip install Pillow

## Classes
### Node: 
Represents a state in the maze. Each node keeps track of its state (position), parent node, and action (movement direction).

### StackFrontier: 
Implements a stack to explore nodes in a Depth-First Search (DFS) manner.

### QueueFrontier: 
Inherits from StackFrontier and implements a queue to explore nodes in a Breadth-First Search (BFS) manner.

### Maze: 
Manages the maze structure, initializes the maze from the file, and provides methods to solve the maze, print the solution, and output an image.

## Functions
### __init__(filename): 
Initializes the maze by reading the input file, determines the start and goal positions, and stores the maze structure.
### solve(): 
Solves the maze using DFS (or BFS if QueueFrontier is used). Explores nodes, keeps track of visited nodes, and finds the solution.
### neighbors(state): 
Returns all possible valid moves from a given state.
### print(): 
Prints the current state of the maze, including the solution path.

