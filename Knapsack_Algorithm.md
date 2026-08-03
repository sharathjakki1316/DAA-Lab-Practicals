#   Knapsack Problem using Dynamic Programming Algorithm

## Aim

To implement the 0/1 Knapsack Problem using Dynamic Programming and determine the maximum profit that can be obtained without exceeding the given knapsack capacity.

---

## Objective

- To understand the concept of Dynamic Programming.
- To solve the 0/1 Knapsack Problem using Dynamic Programming.
- To maximize the total profit while satisfying the weight constraint.
- To analyze the time and space complexity of the algorithm.

---

## Introduction

The **0/1 Knapsack Problem** is one of the most popular optimization problems in computer science. Given a set of items, each with a weight and a value, the objective is to determine the maximum total value that can be placed into a knapsack with a limited weight capacity.

In the **0/1 Knapsack Problem**, each item can either be:
- Included exactly once (1)
- Not included at all (0)

Dynamic Programming solves this problem by storing solutions to smaller subproblems and using them to build the final solution efficiently.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- 0/1 Knapsack Problem using Dynamic Programming

---

## Algorithm

### Steps

1. Start.
2. Read the number of items.
3. Read the value and weight of each item.
4. Read the capacity of the knapsack.
5. Create a Dynamic Programming (DP) table of size `(number of items + 1) × (capacity + 1)`.
6. Initialize the first row and first column with zero.
7. For each item:
   - If the item's weight is less than or equal to the current capacity:
     - Choose the maximum of:
       - Including the item.
       - Excluding the item.
   - Otherwise, exclude the item.
8. Store the maximum value in the DP table.
9. Display the maximum profit.
10. Stop.

---

## Sample Input

```
Enter the number of items: 4

Values : 1 4 5 7
Weights: 1 3 4 5

Knapsack Capacity: 7
```

---

## Sample Output

```
Maximum Profit = 9
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n × W) |
| Average Case | O(n × W) |
| Worst Case | O(n × W) |

Where:
- **n** = Number of items
- **W** = Knapsack capacity

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| 0/1 Knapsack | O(n × W) |

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Knapsack_Problem.ipynb | Python implementation of the 0/1 Knapsack Problem using Dynamic Programming |

---

## Applications

- Resource Allocation
- Budget Planning
- Cargo Loading
- Investment Planning
- Project Selection
- Inventory Management

---

## Conclusion

The 0/1 Knapsack Problem was successfully implemented using Dynamic Programming. The algorithm efficiently computes the maximum profit by solving and storing solutions to smaller subproblems. Dynamic Programming significantly reduces redundant computations compared to a recursive approach, making it suitable for optimization problems involving overlapping subproblems.
