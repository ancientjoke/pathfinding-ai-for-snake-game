# Pathfinding AI for Snake game

![pathfinding](https://github.com/user-attachments/assets/37b0d6c2-23b9-4a2a-9615-31d71f85a977)

## Setup and Execution

1. Download and install [Python 3](https://www.python.org).
2. Install the required modules by executing the following command in your terminal:
```bash
pip install pygame
```
3. Run `play.py` to start the game.

## Functionality

1. Finding the Shortest Path:
- The snake employs the BFS (Breadth-First Search) algorithm to calculate the shortest path (path_1) to the apple. If path_1 is not available, the process skips to step 4.

2. Simulating Movement:
- A virtual snake, mirroring the state of the actual snake, is created and programmed to follow path_1.

3. Validating Tail Path:
- After the virtual snake reaches the apple, the accessibility of a secondary path (path_2) between its head and tail is verified. If path_2 is accessible, the actual snake follows path_1.

4. Fallback Strategy:
- If either path_1 or path_2 is inaccessible, the actual snake is directed to follow its own tail as a fallback measure.
