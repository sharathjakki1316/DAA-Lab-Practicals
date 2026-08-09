# 📘 Practical 9: Implementation of Prim's Algorithm

## Aim

To implement Prim's Algorithm to find the Minimum Spanning Tree (MST) of a connected weighted graph.

---

## Objective

- To understand the concept of Minimum Spanning Tree.
- To understand the working of Prim's Algorithm.
- To construct a Minimum Spanning Tree from a weighted graph.
- To calculate the minimum total weight of the spanning tree.
- To analyze the time and space complexity of Prim's Algorithm.

---

## Introduction

Prim's Algorithm is a **greedy algorithm** used to find the Minimum Spanning Tree (MST) of a connected, weighted and undirected graph.

A Minimum Spanning Tree is a spanning tree that connects all the vertices of a graph with the minimum possible total edge weight.

Prim's Algorithm starts with a selected vertex and repeatedly chooses the minimum-weight edge that connects a vertex already included in the MST to a vertex outside the MST.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Prim's Algorithm for Minimum Spanning Tree

---

## Algorithm

### Steps

1. Start.
2. Read the number of vertices.
3. Read the weighted adjacency matrix of the graph.
4. Select the starting vertex.
5. Mark the starting vertex as selected.
6. Find the minimum-weight edge connecting a selected vertex to an unselected vertex.
7. Add the selected edge to the Minimum Spanning Tree.
8. Mark the newly connected vertex as selected.
9. Repeat Steps 6–8 until all vertices are included in the MST.
10. Calculate and display the total weight of the Minimum Spanning Tree.
11. Stop.

---

## Pseudo Code

```text
PRIM(graph)

1. Start

2. n ← number of vertices

3. Create an array selected[n]
   Initialize all values as False

4. Select the starting vertex
   selected[0] ← True

5. total_weight ← 0

6. Repeat n-1 times:

      minimum ← ∞
      x ← -1
      y ← -1

      For i ← 0 to n-1
          If selected[i] = True

              For j ← 0 to n-1
                  If selected[j] = False
                     AND graph[i][j] ≠ 0

                      If graph[i][j] < minimum
                          minimum ← graph[i][j]
                          x ← i
                          y ← j

      Add edge (x, y) to MST
      Display edge and its weight

      total_weight ← total_weight + graph[x][y]

      selected[y] ← True

7. Display total_weight

8. Stop
```

---

## Sample Input

```text
Enter number of vertices: 5

Enter the adjacency matrix:
0 2 0 6 0
2 0 3 8 5
0 3 0 0 7
6 8 0 0 9
0 5 7 9 0
```

---

## Sample Output

```text
Edges in Minimum Spanning Tree:
Edge    Weight
0 - 1   2
1 - 2   3
1 - 4   5
0 - 3   6

Minimum Spanning Tree Weight: 16
```

---

## Time Complexity

For the adjacency matrix implementation:

| Case | Complexity |
|------|------------|
| Best Case | O(V²) |
| Average Case | O(V²) |
| Worst Case | O(V²) |

Where:

- **V** = Number of vertices

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| Prim's Algorithm | O(V²) |

The graph is represented using an adjacency matrix.

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Prims_Algorithm.ipynb | Python implementation of Prim's Algorithm |

---

## Applications

- Network Design
- Computer Network Infrastructure
- Electrical Grid Design
- Road and Transportation Networks
- Telecommunication Networks
- Connecting Multiple Locations with Minimum Cost

---

## Conclusion

Prim's Algorithm was successfully implemented to find the Minimum Spanning Tree of a weighted graph. The algorithm uses a greedy approach by repeatedly selecting the minimum-weight edge that connects a selected vertex to an unselected vertex. The adjacency matrix implementation has a time complexity of **O(V²)** and efficiently constructs the Minimum Spanning Tree for the given graph.