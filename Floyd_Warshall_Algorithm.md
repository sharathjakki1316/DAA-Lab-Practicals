# 📘 Practical 11: Implementation of Floyd-Warshall Algorithm

## Aim

To implement the Floyd-Warshall Algorithm to find the shortest paths between all pairs of vertices in a weighted graph.

---

## Objective

- To understand the concept of the all-pairs shortest path problem.
- To understand the working of the Floyd-Warshall Algorithm.
- To find the shortest distance between every pair of vertices.
- To use Dynamic Programming for solving the shortest path problem.
- To analyze the time and space complexity of the algorithm.

---

## Introduction

The **Floyd-Warshall Algorithm** is a Dynamic Programming algorithm used to find the shortest paths between all pairs of vertices in a weighted graph.

The algorithm considers each vertex as an intermediate vertex and checks whether a shorter path exists through that vertex. It systematically updates the distance matrix until the shortest distances between all pairs of vertices are obtained.

The algorithm can handle positive edge weights and can also detect negative-weight cycles when appropriate.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Floyd-Warshall Algorithm for All-Pairs Shortest Paths

---

## Algorithm

### Steps

1. Start.
2. Read the number of vertices.
3. Read the weighted adjacency matrix.
4. Initialize the distance matrix with the given graph distances.
5. Set the distance from each vertex to itself as zero.
6. Consider each vertex as an intermediate vertex one by one.
7. For every pair of vertices `(i, j)`, check whether the path through the intermediate vertex `k` is shorter.
8. Update the distance if a shorter path is found.
9. Display the final shortest distance matrix.
10. Stop.

---

## Pseudo Code

```text
FLOYD_WARSHALL(graph)

1. Start

2. n ← number of vertices

3. Create distance matrix dist

4. Copy graph into dist

5. For k ← 0 to n-1
      For i ← 0 to n-1
          For j ← 0 to n-1

              If dist[i][k] ≠ ∞ AND dist[k][j] ≠ ∞

                  dist[i][j] ← min(
                      dist[i][j],
                      dist[i][k] + dist[k][j]
                  )

6. Display the shortest distance matrix

7. Stop
```

---

## Sample Input

```text
Enter number of vertices: 4

Enter the adjacency matrix:
0 5 INF 10
INF 0 3 INF
INF INF 0 1
INF INF INF 0
```

---

## Sample Output

```text
Shortest Distance Matrix:

0    5    8    9
INF  0    3    4
INF  INF  0    1
INF  INF  INF  0
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(V³) |
| Average Case | O(V³) |
| Worst Case | O(V³) |

Where:

- **V** = Number of vertices

The algorithm uses three nested loops, resulting in a time complexity of **O(V³)**.

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| Floyd-Warshall Algorithm | O(V²) |

The distance matrix requires **O(V²)** space.

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Floyd_Warshall_Algorithm.ipynb | Python implementation of Floyd-Warshall Algorithm |

---

## Applications

- Network Routing
- Shortest Path Computation
- Transportation Networks
- Communication Networks
- Route Optimization
- Graph Analysis
- Finding Shortest Paths Between All Pairs of Locations

---

## Conclusion

The Floyd-Warshall Algorithm was successfully implemented to determine the shortest paths between all pairs of vertices in a weighted graph. The algorithm uses a Dynamic Programming approach by considering each vertex as an intermediate vertex and repeatedly updating the distance matrix. It provides an efficient solution for the all-pairs shortest path problem with a time complexity of **O(V³)** and a space complexity of **O(V²)**.