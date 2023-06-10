# HillClimbing
 
Hill climbing is a simple local search algorithm used for optimization problems. It starts with an initial solution and iteratively makes small improvements by considering neighboring solutions. The algorithm explores the solution space by moving towards neighboring solutions with better objective values until it reaches a local optimum.

To find the shortest path in a Traveling Salesman Problem (TSP) using hill climbing, you can follow these steps:

1. The randomSolution function generates a random initial solution by shuffling the cities randomly.

2. The routeLength function calculates the total length of the route for a given solution by summing the distances between consecutive cities.

3. The getNeighbours function generates all possible neighboring solutions by swapping two cities in the current solution.

4. The getBestNeighbour function finds the best neighboring solution with the shortest route length.

5. The hillClimbing function performs the hill climbing algorithm. It starts with a random initial solution and iteratively improves it by selecting the best neighbor until no better solution can be found.

6. The main function initializes the tsp matrix, which represents the distances between cities. It then calls the hillClimbing function and prints the resulting best solution and its route length.

## Note
The `tsp` variable represents a matrix that defines the distances between cities in a Traveling Salesman Problem (TSP) instance. In this case, the TSP consists of 4 cities, and the distances between them are defined as follows:

```
      | City 0 | City 1 | City 2 | City 3
-----------------------------------------
City 0|   0    |  400   |  500   |  300
City 1|  400   |   0    |  300   |  500
City 2|  500   |  300   |   0    |  400
City 3|  300   |  500   |  400   |   0
```

The distances are symmetric, meaning that the distance from City A to City B is the same as the distance from City B to City A. For example, the distance from City 1 to City 2 is 300, which is the same as the distance from City 2 to City 1.

This matrix represents the problem instance for which the hill climbing algorithm will try to find the shortest possible route that visits all cities exactly once and returns to the starting city.
