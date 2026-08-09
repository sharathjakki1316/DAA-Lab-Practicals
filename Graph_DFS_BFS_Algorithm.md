# 📘 Practical 8: Implementation of Graph and Searching (DFS and BFS)

## Aim

To implement a graph and perform searching using Depth First Search (DFS) and Breadth First Search (BFS) algorithms in Python.

---

## Objective

- To understand the concept of graphs and graph representation.
- To implement a graph using an adjacency list.
- To implement Depth First Search (DFS).
- To implement Breadth First Search (BFS).
- To analyze the time and space complexity of DFS and BFS.

---

## Introduction

A **Graph** is a non-linear data structure consisting of a set of vertices (nodes) and edges that connect pairs of vertices.

Graphs can be represented in different ways. In this practical, an **adjacency list** is used to represent the graph.

Two fundamental graph traversal algorithms are implemented:

- **Depth First Search (DFS):** Traverses a graph by exploring as far as possible along one branch before backtracking.
- **Breadth First Search (BFS):** Traverses a graph level by level, visiting all neighboring vertices before moving to the next level.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Graph Representation using Adjacency List
- Depth First Search (DFS)
- Breadth First Search (BFS)

---

## Algorithm

### Algorithm for Graph Representation

1. Start.
2. Create an empty adjacency list for the vertices.
3. Add an edge between two vertices.
4. Store each connected vertex in the corresponding adjacency list.
5. Repeat until all required edges are added.
6. Stop.

---

### Algorithm for Depth First Search (DFS)

1. Start.
2. Select the starting vertex.
3. Mark the vertex as visited.
4. Display the current vertex.
5. Visit an unvisited adjacent vertex.
6. Recursively repeat the process for the selected vertex.
7. Continue until all reachable vertices are visited.
8. Stop.

---

### Algorithm for Breadth First Search (BFS)

1. Start.
2. Select the starting vertex.
3. Create an empty queue.
4. Mark the starting vertex as visited and insert it into the queue.
5. Remove a vertex from the front of the queue.
6. Display the vertex.
7. Add all unvisited adjacent vertices to the queue and mark them as visited.
8. Repeat Steps 5–7 until the queue becomes empty.
9. Stop.

---

## Pseudo Code

### Pseudo Code for Graph Representation

```text
ADD_EDGE(graph, u, v)

1. Start
2. Add v to graph[u]
3. Add u to graph[v]
4. Stop
```

---

### Pseudo Code for Depth First Search (DFS)

```text
DFS(graph, start, visited)

1. Start
2. If start is not in visited
      Add start to visited
      Display start

3. For each neighbor of start
      If neighbor is not in visited
          DFS(graph, neighbor, visited)

4. Stop
```

---

### Pseudo Code for Breadth First Search (BFS)

```text
BFS(graph, start)

1. Start
2. Create an empty set visited
3. Create an empty queue
4. Add start to visited
5. Insert start into the queue

6. While queue is not empty
      Remove a vertex from the front
      Display the vertex

      For each neighbor of the vertex
          If neighbor is not visited
              Add neighbor to visited
              Insert neighbor into the queue

7. Stop
```

---

## Sample Graph

```text
        0
       / \
      1   2
     / \
    3   4
```

### Edges

```text
0 — 1
0 — 2
1 — 3
1 — 4
```

---

## Sample Output

```text
DFS Traversal:
0 1 3 4 2

BFS Traversal:
0 1 2 3 4
```

> The traversal order may vary depending on the order of vertices in the adjacency list.

---

## Time Complexity

For a graph represented using an adjacency list:

| Algorithm | Time Complexity |
|-----------|-----------------|
| DFS | O(V + E) |
| BFS | O(V + E) |

Where:

- **V** = Number of vertices
- **E** = Number of edges

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| DFS | O(V) |
| BFS | O(V) |

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Graph_DFS_BFS.ipynb | Python implementation of Graph, DFS and BFS |

---

## Applications

### Applications of DFS

- Maze solving
- Path finding
- Cycle detection
- Topological sorting
- Connected component analysis

### Applications of BFS

- Shortest path in unweighted graphs
- Network broadcasting
- Social network analysis
- Web crawling
- Level-order traversal

---

## Conclusion

The Graph was successfully implemented using an adjacency list, and both **Depth First Search (DFS)** and **Breadth First Search (BFS)** were implemented in Python. DFS explores vertices deeply before backtracking, whereas BFS explores the graph level by level. Both algorithms provide an efficient way to traverse graph structures and have a time complexity of **O(V + E)** when an adjacency list is used.