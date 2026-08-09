# 📘 Practical 7: Implementation of Making Change Problem using Dynamic Programming

## Aim

To implement the Making Change Problem using Dynamic Programming and determine the minimum number of coins required to make a given amount.

---

## Objective

- To understand the concept of Dynamic Programming.
- To solve the Making Change Problem efficiently.
- To determine the minimum number of coins required for a given amount.
- To analyze the time and space complexity of the algorithm.

---

## Introduction

The Making Change Problem is a classic Dynamic Programming problem in which the objective is to find the minimum number of coins needed to make a given amount using a set of available coin denominations.

Dynamic Programming is used to store solutions to smaller subproblems and reuse them to compute the optimal solution efficiently.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Making Change Problem using Dynamic Programming

---

## Algorithm

### Steps

1. Start.
2. Read the number of coin denominations.
3. Read the coin values.
4. Read the target amount.
5. Create a DP array of size `(amount + 1)`.
6. Initialize `dp[0] = 0` and all other values as infinity.
7. For each amount from 1 to target amount:
   - Check all coin denominations.
   - Update the minimum number of coins required.
8. Display the minimum number of coins needed.
9. Stop.

---

## Pseudo Code

```text
MIN_COINS(coins, amount)

Create array dp[0...amount]

dp[0] ← 0

For i ← 1 to amount
    dp[i] ← ∞

For i ← 1 to amount
    For each coin in coins
        If coin ≤ i
            dp[i] ← min(dp[i], dp[i - coin] + 1)

If dp[amount] = ∞
    Return -1
Else
    Return dp[amount]
```

---

## Sample Input

```text
Enter number of coin denominations: 3

Enter coin denominations:
1
2
5

Enter amount: 11
```

---

## Sample Output

```text
Minimum coins required = 3
```

Explanation:

```text
11 = 5 + 5 + 1
```

---

## Time Complexity

| Case | Complexity |
|--------|--------|
| Best Case | O(n × A) |
| Average Case | O(n × A) |
| Worst Case | O(n × A) |

Where:

- n = Number of coin denominations
- A = Target amount

---

## Space Complexity

| Algorithm | Space Complexity |
|------------|------------|
| Making Change Problem | O(A) |

---

## Files Included

| File Name | Description |
|------------|------------|
| Making_Change_Problem.ipynb | Python implementation of Making Change Problem using Dynamic Programming |

---

## Applications

- Currency Exchange Systems
- ATM Cash Dispensing
- Financial Software
- E-commerce Payment Systems
- Resource Allocation Problems

---

## Conclusion

The Making Change Problem was successfully implemented using Dynamic Programming. The algorithm efficiently determines the minimum number of coins required to make a given amount by storing solutions to smaller subproblems and reusing them to compute the optimal solution.