# 📘 Practical 12: Implementation of Travelling Salesman Problem using Dynamic Programming

## Aim

To implement the Travelling Salesman Problem (TSP) using Dynamic Programming and determine the minimum cost of a tour that visits every city exactly once and returns to the starting city.

---

## Objective

- To understand the Travelling Salesman Problem.
- To solve the TSP using Dynamic Programming.
- To determine the minimum-cost tour for a given set of cities.
- To understand the use of bitmasking in Dynamic Programming.
- To analyze the time and space complexity of the algorithm.

---

## Introduction

The **Travelling Salesman Problem (TSP)** is a well-known optimization problem in computer science. The objective is to find the shortest possible route that visits every city exactly once and returns to the starting city.

The distance or cost between each pair of cities is given in the form of a distance matrix.

Since checking every possible tour becomes computationally expensive as the number of cities increases, **Dynamic Programming** can be used to reduce repeated calculations by storing solutions to previously solved subproblems.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Travelling Salesman Problem using Dynamic Programming

---

## Algorithm

### Steps

1. Start.
2. Read the number of cities.
3. Read the distance matrix.
4. Select the first city as the starting city.
5. Represent the set of visited cities using a bitmask.
6. Recursively calculate the minimum cost of visiting all unvisited cities.
7. If all cities have been visited, add the cost of returning to the starting city.
8. For each unvisited city:
   - Calculate the cost of travelling to that city.
   - Recursively calculate the remaining tour cost.
   - Select the minimum total cost.
9. Store previously calculated results to avoid repeated computations.
10. Display the minimum travelling cost.
11. Stop.

---

## Pseudo Code

```text
TSP(graph)

1. Start

2. n ← number of cities

3. Define DP(current, visited)

4. If all cities are visited
      Return graph[current][0]

5. minimum_cost ← ∞

6. For each city from 0 to n-1

      If city is not visited

          cost ← graph[current][city]
                  + DP(city, visited ∪ {city})

          minimum_cost ← min(minimum_cost, cost)

7. Store the result for the current state.

8. Return minimum_cost.

9. Start the tour from city 0
   with only city 0 marked as visited.

10. Display minimum_cost.

11. Stop.
```

---

## Sample Input

```text
Enter number of cities: 4

Enter the distance matrix:
0 10 15 20
10 0 35 25
15 35 0 30
20 25 30 0
```

---

## Sample Output

```text
Minimum travelling cost = 80
```

One optimal tour is:

```text
0 → 1 → 3 → 2 → 0
```

Total cost:

```text
10 + 25 + 30 + 15 = 80
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n² × 2ⁿ) |
| Average Case | O(n² × 2ⁿ) |
| Worst Case | O(n² × 2ⁿ) |

Where:

- **n** = Number of cities

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| TSP using Dynamic Programming | O(n × 2ⁿ) |

The space is required to store the Dynamic Programming states for different combinations of current cities and visited cities.

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Travelling_Salesman_Problem.ipynb | Python implementation of Travelling Salesman Problem using Dynamic Programming |

---

## Applications

- Route Optimization
- Delivery and Logistics Planning
- Transportation Planning
- Tour Planning
- Vehicle Routing
- Network Optimization
- Supply Chain Management

---

## Conclusion

The Travelling Salesman Problem was successfully implemented using Dynamic Programming. The algorithm determines the minimum-cost tour that visits every city exactly once and returns to the starting city. Dynamic Programming with bitmasking avoids repeated calculations and provides an exact solution, although the computational complexity remains exponential as the number of cities increases.