# 📘 Practical 6: Implementation of Matrix Chain Multiplication using Dynamic Programming

## Aim

To implement Matrix Chain Multiplication using Dynamic Programming and determine the minimum number of scalar multiplications required to multiply a chain of matrices.

---

## Objective

- To understand the concept of Dynamic Programming.
- To find the optimal order of matrix multiplication.
- To minimize the total number of scalar multiplications.
- To analyze the time and space complexity of the algorithm.

---

## Introduction

Matrix Chain Multiplication is a classical Dynamic Programming problem used to determine the most efficient way to multiply a sequence of matrices. Since matrix multiplication is associative, matrices can be multiplied in different orders. Different orders require different numbers of scalar multiplications.

Dynamic Programming is used to find the optimal parenthesization that minimizes the multiplication cost.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Matrix Chain Multiplication using Dynamic Programming

---

## Algorithm

### Steps

1. Start.
2. Read the number of matrices.
3. Read the dimensions of the matrices.
4. Create a DP table to store multiplication costs.
5. Initialize diagonal elements as zero.
6. Compute costs for chains of increasing lengths.
7. For every possible partition:
   - Calculate multiplication cost.
   - Store the minimum cost.
8. Display the minimum multiplication cost.
9. Stop.

---

## Pseudo Code

```text
MATRIX_CHAIN_ORDER(p)

n ← length(p)

Create matrix m[n][n]

for i ← 1 to n-1
    m[i][i] ← 0

for L ← 2 to n-1
    for i ← 1 to n-L
        j ← i + L - 1
        m[i][j] ← ∞

        for k ← i to j-1
            q ← m[i][k] +
                 m[k+1][j] +
                 p[i-1] × p[k] × p[j]

            if q < m[i][j]
                m[i][j] ← q

return m[1][n-1]
```

---

## Sample Input

```text
Enter number of matrices: 4

Enter dimensions:
10
20
30
40
30
```

---

## Sample Output

```text
Minimum number of multiplications = 30000
```

---

## Time Complexity

| Case | Complexity |
|--------|--------|
| Best Case | O(n³) |
| Average Case | O(n³) |
| Worst Case | O(n³) |

Where:
- n = Number of matrices

---

## Space Complexity

| Algorithm | Space Complexity |
|------------|------------|
| Matrix Chain Multiplication | O(n²) |

---

## Files Included

| File Name | Description |
|------------|------------|
| Matrix_Chain_Multiplication.ipynb | Python implementation of Matrix Chain Multiplication using Dynamic Programming |

---

## Applications

- Database Query Optimization
- Scientific Computing
- Computer Graphics
- Numerical Analysis
- Linear Algebra Operations
- Compiler Optimization

---

## Conclusion

Matrix Chain Multiplication was successfully implemented using Dynamic Programming. The algorithm efficiently determines the optimal order of matrix multiplication and minimizes the total number of scalar multiplications. Dynamic Programming reduces redundant computations and provides an optimal solution for this optimization problem.