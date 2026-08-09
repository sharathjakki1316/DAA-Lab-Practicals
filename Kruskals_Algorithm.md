# 📘 Practical 10: Implementation of Kruskal's Algorithm

## Aim

To implement Kruskal's Algorithm to find the Minimum Spanning Tree (MST) of a connected weighted graph.

---

## Objective

- To understand the concept of Minimum Spanning Tree.
- To understand the working of Kruskal's Algorithm.
- To select edges with minimum weights without forming a cycle.
- To construct the Minimum Spanning Tree of a weighted graph.
- To analyze the time and space complexity of Kruskal's Algorithm.

---

## Introduction

Kruskal's Algorithm is a **greedy algorithm** used to find the Minimum Spanning Tree (MST) of a connected, weighted and undirected graph.

The algorithm sorts all the edges of the graph in increasing order of their weights. It then selects the smallest edge and adds it to the Minimum Spanning Tree if adding the edge does not create a cycle.

A **Disjoint Set (Union-Find)** data structure is used to efficiently detect cycles while constructing the Minimum Spanning Tree.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Kruskal's Algorithm for Minimum Spanning Tree

---

## Algorithm

### Steps

1. Start.
2. Read the number of vertices and edges.
3. Read all edges along with their weights.
4. Sort all edges in increasing order of weight.
5. Initialize a separate set for each vertex.
6. Select the edge with the smallest weight.
7. Check whether adding the edge creates a cycle.
8. If it does not create a cycle, add the edge to the Minimum Spanning Tree.
9. Merge the sets containing the two vertices.
10. Repeat Steps 6–9 until `V - 1` edges are selected.
11. Calculate and display the total weight of the Minimum Spanning Tree.
12. Stop.

---

## Pseudo Code

### Find Operation

```text
FIND(parent, i)

1. If parent[i] ≠ i
      parent[i] ← FIND(parent, parent[i])

2. Return parent[i]
```

### Union Operation

```text
UNION(parent, rank, x, y)

1. Find the root of x
2. Find the root of y

3. If the roots are different
      If rank[x] < rank[y]
          parent[x] ← y

      Else if rank[x] > rank[y]
          parent[y] ← x

      Else
          parent[y] ← x
          rank[x] ← rank[x] + 1

4. Stop
```

### Kruskal's Algorithm

```text
KRUSKAL(vertices, edges)

1. Start

2. Sort all edges in increasing order of weight.

3. Initialize parent and rank arrays.

4. Create an empty MST.

5. For each edge (u, v, weight) in sorted edges:

      Find the root of u
      Find the root of v

      If root(u) ≠ root(v)

          Add edge (u, v) to MST
          Add weight to total weight

          UNION the two sets

      If number of MST edges = V - 1
          Stop

6. Display the Minimum Spanning Tree.

7. Display the total weight.

8. Stop
```

---

## Sample Input

```text
Enter number of vertices: 5
Enter number of edges: 7

Enter edges (source destination weight):
0 1 2
0 3 6
1 2 3
1 3 8
1 4 5
2 4 7
3 4 9
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

| Case | Complexity |
|------|------------|
| Best Case | O(E log E) |
| Average Case | O(E log E) |
| Worst Case | O(E log E) |

Where:

- **E** = Number of edges
- **V** = Number of vertices

The dominant operation is sorting the edges by weight.

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| Kruskal's Algorithm | O(V + E) |

The space is used for the graph edges and the Disjoint Set data structure.

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Kruskals_Algorithm.ipynb | Python implementation of Kruskal's Algorithm |

---

## Applications

- Computer Network Design
- Electrical Grid Design
- Road and Transportation Networks
- Telecommunication Networks
- Connecting Multiple Locations with Minimum Cost
- Network Infrastructure Optimization

---

## Conclusion

Kruskal's Algorithm was successfully implemented to find the Minimum Spanning Tree of a weighted graph. The algorithm uses a greedy approach by selecting edges in increasing order of weight while avoiding cycles. The use of the Disjoint Set (Union-Find) data structure makes cycle detection efficient. The algorithm has a time complexity of **O(E log E)** due to sorting the edges.