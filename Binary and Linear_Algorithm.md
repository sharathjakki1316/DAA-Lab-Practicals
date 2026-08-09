# 📘 Practical 2: Implementation and Time Analysis of Linear Search and Binary Search Algorithms

## Aim

To implement and analyze the performance of Linear Search and Binary Search algorithms using Python.

---

## Objective

- To understand the working of Linear Search and Binary Search.
- To implement searching algorithms using Python.
- To compare the efficiency of both searching techniques.
- To analyze the time and space complexities of each algorithm.

---

## Introduction

Searching is the process of finding the location of a specific element in a collection of data.

This practical covers two commonly used searching algorithms:

- **Linear Search:** Sequentially checks each element until the target is found.
- **Binary Search:** Searches a sorted array by repeatedly dividing the search interval into two halves.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Programs Included

1. Linear Search
2. Binary Search

---

# Linear Search Algorithm

### Steps

1. Start.
2. Read the array elements.
3. Read the element to be searched.
4. Compare the key element with each array element one by one.
5. If the element is found, display its position.
6. Otherwise, continue searching.
7. If the last element is reached and the key is not found, display "Element Not Found."
8. Stop.

---

# Binary Search Algorithm

### Steps

1. Start.
2. Read the sorted array.
3. Read the key element.
4. Initialize `low = 0` and `high = n - 1`.
5. Find the middle element:
   - `mid = (low + high) // 2`
6. Compare the key with the middle element.
7. If the key equals the middle element, display its position.
8. If the key is smaller, search the left half.
9. If the key is larger, search the right half.
10. Repeat until the element is found or the search interval becomes empty.
11. If the element is not found, display "Element Not Found."
12. Stop.

---

## Time Complexity

| Algorithm | Best Case | Average Case | Worst Case |
|-----------|-----------|--------------|------------|
| Linear Search | O(1) | O(n) | O(n) |
| Binary Search | O(1) | O(log n) | O(log n) |

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| Linear Search | O(1) |
| Binary Search (Iterative) | O(1) |
| Binary Search (Recursive) | O(log n) |

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Linear_Search.ipynb | Python implementation of Linear Search |
| Binary_Search.ipynb | Python implementation of Binary Search |

---

## Conclusion

The Linear Search and Binary Search algorithms were successfully implemented using Python. Linear Search is suitable for both sorted and unsorted data but is less efficient for large datasets. Binary Search is significantly faster but requires the input array to be sorted.