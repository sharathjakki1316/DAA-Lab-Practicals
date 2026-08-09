# 📘 Practical 4: Implementation and Time Analysis of Factorial Program Using Iterative and Recursive Method

## Aim

To implement and analyze the performance of the Factorial program using both Iterative and Recursive methods in Python.

---

## Objective

- To understand the concept of factorial computation.
- To implement the factorial program using the Iterative method.
- To implement the factorial program using the Recursive method.
- To compare the time and space complexities of both methods.

---

## Introduction

The factorial of a non-negative integer **n** is the product of all positive integers less than or equal to **n**. It is represented as **n!**.

\[
n! = n \times (n-1) \times (n-2) \times \cdots \times 2 \times 1
\]

For example:

- 5! = 5 × 4 × 3 × 2 × 1 = 120
- 0! = 1

This practical demonstrates two different approaches to calculate the factorial of a number:

- **Iterative Method:** Uses a loop to calculate the factorial.
- **Recursive Method:** Uses a function that repeatedly calls itself until the base condition is reached.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Programs Included

1. Factorial using Iterative Method
2. Factorial using Recursive Method

---

## Algorithm

### Algorithm for Iterative Method

1. Start.
2. Read the input number **n**.
3. Initialize `fact = 1`.
4. Repeat from `1` to `n`:
   - Multiply `fact` by the current number.
5. Display the factorial.
6. Stop.

---

### Algorithm for Recursive Method

1. Start.
2. Read the input number **n**.
3. If `n` is 0 or 1, return 1.
4. Otherwise, return `n × factorial(n-1)`.
5. Display the factorial.
6. Stop.

---

## Time Complexity

| Method | Best Case | Average Case | Worst Case |
|--------|-----------|--------------|------------|
| Iterative | O(n) | O(n) | O(n) |
| Recursive | O(n) | O(n) | O(n) |

---

## Space Complexity

| Method | Space Complexity |
|--------|------------------|
| Iterative | O(1) |
| Recursive | O(n) |

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Factorial.ipynb | Python implementation of Factorial using Iterative and Recursive methods |

---

## Conclusion

The Factorial program was successfully implemented using both Iterative and Recursive methods in Python. The Iterative method uses constant extra space and is generally more efficient for larger inputs, while the Recursive method provides a simpler and more elegant solution but requires additional memory for recursive function calls. Both methods correctly compute the factorial of a given number.