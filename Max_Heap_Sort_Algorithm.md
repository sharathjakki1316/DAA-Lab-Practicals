# 📘 Practical 3: Implementation of Max-Heap Sort Algorithm

## Aim

To implement the Max-Heap Sort algorithm using Python.

---

## Objective

- To understand the working of the Max-Heap data structure.
- To implement Heap Sort using a Max-Heap.
- To learn how heap operations are used for sorting.
- To analyze the time and space complexity of Heap Sort.

---

## Introduction

Heap Sort is a comparison-based sorting algorithm that uses a **Binary Heap** data structure. In Max-Heap Sort, the largest element is stored at the root of the heap. The algorithm repeatedly removes the maximum element from the heap and places it at the end of the array until all elements are sorted.

Heap Sort is efficient for large datasets and guarantees **O(n log n)** time complexity in the best, average, and worst cases.

---

## Software Used

- Python 3.x
- Anaconda Distribution
- Jupyter Notebook

---

## Program Included

- Max-Heap Sort

---

## Algorithm

### Steps

1. Start.
2. Read the array elements.
3. Build a Max-Heap from the input array.
4. Swap the root element with the last element.
5. Reduce the heap size by one.
6. Apply the Heapify operation to restore the Max-Heap property.
7. Repeat Steps 4–6 until the heap size becomes one.
8. Display the sorted array.
9. Stop.

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n log n) |

---

## Space Complexity

| Algorithm | Space Complexity |
|-----------|------------------|
| Heap Sort | O(1) (Ignoring recursion stack) |

---

## Files Included

| File Name | Description |
|-----------|-------------|
| Max_Heap_Sort.ipynb | Python implementation of Max-Heap Sort |

---

## Conclusion

The Max-Heap Sort algorithm was successfully implemented using Python. It efficiently sorts elements by building a Max-Heap and repeatedly extracting the maximum element. Heap Sort provides consistent O(n log n) performance and is suitable for sorting large datasets.