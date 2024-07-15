# Pathfinding Algorithms Simulator

Welcome to Pathfinder Simulator! This application was built out of a fascination with pathfinding algorithms and a desire to visualize them in action. Enjoy exploring the world of pathfinding algorithms with this interactive tool.

## Table of Contents

- [Meet the Algorithms](#meet-the-algorithms)
- [More about the Swarm Algorithm](#more-about-the-swarm-algorithm)
- [Features](#features)
- 
## Meet the Algorithms

This application supports the following algorithms:

### Weighted Algorithms
- **Dijkstra's Algorithm**: The father of pathfinding algorithms; guarantees the shortest path.
- **A* Search**: Arguably the best pathfinding algorithm; uses heuristics to guarantee the shortest path much faster than Dijkstra's Algorithm.
- **Greedy Best-first Search**: A faster, more heuristic-heavy version of A*; does not guarantee the shortest path.
- **Swarm Algorithm**: A mixture of Dijkstra's Algorithm and A*; does not guarantee the shortest path.
- **Convergent Swarm Algorithm**: A faster, more heuristic-heavy version of Swarm; does not guarantee the shortest path.
- **Bidirectional Swarm Algorithm**: Swarm from both sides; does not guarantee the shortest path.

### Unweighted Algorithms
- **Breadth-first Search**: A great algorithm; guarantees the shortest path.
- **Depth-first Search**: A very bad algorithm for pathfinding; does not guarantee the shortest path.

### Maze Generation Algorithm
- **Recursive Division**: Generates a maze using a recursive division algorithm.

## More about the Swarm Algorithm

The Swarm Algorithm is an algorithm that I - at least presumably so (I was unable to find anything close to it online) - co-developed with a good friend and colleague, Hussein Farah. The algorithm is essentially a mixture of Dijkstra's Algorithm and A* Search; more precisely, while it converges to the target node like A*, it still explores quite a few neighboring nodes surrounding the start node like Dijkstra's. 

The algorithm differentiates itself from A* through its use of heuristics: it continually updates nodes' distance from the start node while taking into account their estimated distance from the target node. This effectively "balances" the difference in total distance between nodes closer to the start node and nodes closer to the target node, resulting in the triangle-like shape of the Swarm Algorithm. 

We named the algorithm "Swarm" because one of its potential applications could be seen in a video game where a character must keep track of a boss with high priority (the target node), all the while keeping track of neighboring enemies that might be swarming nearby.

## Features

- Interactive visualization of various pathfinding algorithms.
- Ability to place start and end nodes, as well as walls.
- Visual differentiation between visited nodes, shortest path nodes, and walls.
- Speed control for the visualization.
- Maze generation using the Recursive Division algorithm.
