# Merge Sort Algorithm

## Aim

To sort a list of elements in ascending order using the Merge Sort algorithm.

---

## Objective

- To understand the working of Merge Sort.
- To implement the Divide and Conquer technique.
- To sort elements efficiently.
- To analyze the time and space complexity of Merge Sort.

---

## Introduction

Merge Sort is an efficient, stable, comparison-based sorting algorithm that follows the **Divide and Conquer** technique. It divides the array into smaller subarrays until each subarray contains only one element. Then, it merges the subarrays in sorted order to produce the final sorted array.

---

## Algorithm

1. Start.
2. Read the number of elements.
3. Read the array elements.
4. Divide the array into two equal halves.
5. Recursively apply Merge Sort to the left half.
6. Recursively apply Merge Sort to the right half.
7. Merge the two sorted halves into a single sorted array.
8. Repeat until the entire array is sorted.
9. Display the sorted array.
10. Stop.

---

## Example

**Input**

```
38 27 43 3 9 82 10
```

**Output**

```
3 9 10 27 38 43 82
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n log n) |

---

## Space Complexity

```
O(n)
```

---

## Advantages

- Efficient for large datasets.
- Stable sorting algorithm.
- Guaranteed O(n log n) time complexity.
- Suitable for linked lists and external sorting.

---

## Disadvantages

- Requires additional memory.
- Recursive implementation increases function call overhead.
- Slower than Quick Sort for some in-memory datasets.

---

## Applications

- Sorting large datasets.
- External sorting (large files).
- Linked list sorting.
- Applications where stable sorting is required.

---

## Conclusion

Merge Sort is a fast and reliable sorting algorithm based on the Divide and Conquer technique. It consistently performs in O(n log n) time for all cases, making it suitable for large datasets. Although it requires extra memory, its stability and predictable performance make it one of the most widely used sorting algorithms.