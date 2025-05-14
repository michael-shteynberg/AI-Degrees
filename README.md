# Degrees

This project implements a search algorithm to find the shortest connection between any two actors through the movies they've appeared in, based on the famous "Six Degrees of Kevin Bacon" game. The program uses actual movie data to determine how actors are connected to each other, telling you not only how many "degrees of separation" exist between them, but also the specific chain of movies and co-stars that connect them.

The program uses a breadth-first search (BFS) algorithm to find the shortest possible path between two actors. It works by:

- Loading data about actors, movies, and their relationships from CSV files
- Allowing users to input the names of two actors
- Searching for the shortest path connecting these actors through movies they've starred in
- Displaying the connection path, showing each movie and actor along the way