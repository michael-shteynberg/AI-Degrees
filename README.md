# Degrees of Separation: Graph Search AI

A pathfinding system using breadth-first search to find shortest connections between actors through their movie collaborations.

## Overview

This AI solves the "Six Degrees of Kevin Bacon" problem by implementing graph search algorithms. It finds the shortest chain of movie connections between any two actors in a database, demonstrating fundamental pathfinding techniques used throughout AI.

## Key AI Concepts

### Breadth-First Search (BFS)
The system uses BFS, an uninformed search algorithm that explores all nodes at the current depth before moving deeper. This guarantees finding the shortest path in unweighted graphs. The algorithm systematically expands the search frontier level by level, ensuring optimality without needing domain-specific knowledge.

### Graph Representation
The actor-movie database forms a bipartite graph where actors are nodes and movies create edges between co-stars. This abstraction transforms a complex relational database into a mathematical structure amenable to algorithmic analysis, showing how AI systems model real-world relationships.

### State Space Search
The problem is formulated as navigating through a state space where each state represents an actor, and actions are movie collaborations. The system searches from an initial state (source actor) to a goal state (target actor), finding the minimum-cost path. This demonstrates the general framework used in AI planning and problem-solving.

### Frontier Management
The implementation uses a queue-based frontier for BFS, ensuring first-in-first-out exploration. This data structure choice determines search behavior - a queue guarantees shortest path discovery while a stack would perform depth-first search. The abstraction shows how algorithm behavior emerges from fundamental design decisions.

### Cycle Detection and Graph Traversal
The system maintains an explored set to prevent revisiting states, converting potentially infinite search trees into finite graph exploration. This cycle detection is crucial for real-world graphs where multiple paths exist between nodes, demonstrating how AI handles complex, interconnected search spaces.

## Why This Matters

- **Foundation for Complex AI**: Same techniques scale to route planning, puzzle solving, and automated planning
- **Optimality Guarantees**: Provably finds shortest paths without heuristics
- **Graph Algorithms**: Core to social networks, recommendation systems, and knowledge graphs
- **Search Fundamentals**: Basis for both classical AI and modern pathfinding
