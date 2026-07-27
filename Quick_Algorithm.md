# Quick Sort Algorithm

## Aim

To sort a list of elements in ascending order using the Quick Sort algorithm.

---

## Objective

- To understand the working of Quick Sort.
- To implement the Divide and Conquer technique.
- To sort elements efficiently using a pivot element.
- To analyze the time and space complexity of Quick Sort.

---

## Introduction

Quick Sort is a highly efficient comparison-based sorting algorithm that follows the **Divide and Conquer** technique. It selects a pivot element and partitions the array so that elements smaller than the pivot are placed on the left, while larger elements are placed on the right. The same process is then recursively applied to the subarrays until the entire array is sorted.

---

## Algorithm

1. Start.
2. Read the number of elements.
3. Read the array elements.
4. Select a pivot element from the array.
5. Partition the array so that:
   - Elements smaller than the pivot are placed on the left.
   - Elements greater than the pivot are placed on the right.
6. Recursively apply Quick Sort to the left subarray.
7. Recursively apply Quick Sort to the right subarray.
8. Combine the sorted subarrays.
9. Display the sorted array.
10. Stop.

---

## Example

**Input**

```
10 7 8 9 1 5
```

**Output**

```
1 5 7 8 9 10
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n log n) |
| Average Case | O(n log n) |
| Worst Case | O(n²) |

---

## Space Complexity

```
O(log n) (Average)
```

---

## Advantages

- Very efficient for large datasets.
- Average time complexity is O(n log n).
- Requires less additional memory than Merge Sort.
- Widely used in practice due to its speed.

---

## Disadvantages

- Worst-case time complexity is O(n²).
- Recursive implementation may increase stack usage.
- Not a stable sorting algorithm.

---

## Applications

- Large datasets.
- General-purpose sorting.
- Database systems.
- Operating systems.
- Standard library sorting implementations (with optimizations).

---

## Conclusion

Quick Sort is one of the fastest and most widely used sorting algorithms. It uses the Divide and Conquer technique to efficiently sort data by partitioning the array around a pivot element. Although its worst-case time complexity is O(n²), its average-case performance of O(n log n) makes it an excellent choice for most practical applications.