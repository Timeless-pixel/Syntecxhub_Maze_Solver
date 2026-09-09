# Syntecxhub Maze Solver using A* Search

## 📌 Project Overview

This project was developed as part of the Syntecxhub Artificial Intelligence Internship Program.

The project implements the **A* (A-star) Search Algorithm** to find the shortest path through a maze represented as a grid.

The algorithm navigates from a defined starting position to a goal position while avoiding walls.

## 🤖 Technologies Used

- Python 3
- A* Search Algorithm
- Manhattan Distance Heuristic
- Python `heapq` Priority Queue

## 🧠 How A* Search Works

A* is a pathfinding and graph-search algorithm that searches for an efficient route between a starting point and a goal.

The algorithm uses the following formula:

**f(n) = g(n) + h(n)**

Where:

- **g(n)** = cost of reaching the current position from the start
- **h(n)** = estimated cost from the current position to the goal
- **f(n)** = total estimated cost

This project uses **Manhattan Distance** as the heuristic:

**h(n) = |row1 - row2| + |column1 - column2|**

Movement is allowed in four directions:

- Up
- Down
- Left
- Right

## 🗺️ Maze Representation

The maze uses the following symbols:

| Symbol | Meaning |
|--------|---------|
| `S` | Starting position |
| `G` | Goal position |
| `#` | Wall |
| `.` | Open space |
| `*` | Shortest path |

## ⚙️ Features

- Represents a maze as a grid
- Identifies the start and goal positions
- Avoids walls
- Implements A* Search
- Uses Manhattan Distance
- Finds the shortest path
- Calculates the path length
- Tracks cells explored during the search
- Displays the solved maze
- Handles unreachable goals

## 📊 Test Results

The completed program successfully found a path from the starting position to the goal.

**Start:** `(0, 0)`

**Goal:** `(10, 10)`

**Shortest Path:** `20 moves`

**Cells Explored:** `56`

**Heuristic:** `Manhattan Distance`

### Solved Maze

```text
S . . . # . . . . . . .
* # # . # . # # # # # .
* * * # . # . . . . . #
. # * * * # . # # # . #
. # . # * . . . . # . #
. # . # * # # # # # . #
. # . # * * * * * * * #
. # . # # # # # # # * #
. # . . . . . . . . * #
. # # # # # # # # # * #
. . . . . . . . # . G .
