# Insertion Sort Algorithm

## Aim

To sort a list of elements in ascending order using the Insertion Sort algorithm.

---

## Objective

- To understand the working of Insertion Sort.
- To arrange elements in ascending order.
- To analyze the time and space complexity of Insertion Sort.

---

## Introduction

Insertion Sort is a simple comparison-based sorting algorithm. It builds the sorted array one element at a time by taking each element from the unsorted part and inserting it into its correct position in the sorted part. It is efficient for small datasets and nearly sorted arrays.

---

## Algorithm

1. Start.
2. Read the number of elements.
3. Read the array elements.
4. Assume the first element is already sorted.
5. Pick the next element and store it as the key.
6. Compare the key with the elements before it.
7. Shift all larger elements one position to the right.
8. Insert the key into its correct position.
9. Repeat Steps 5–8 until all elements are sorted.
10. Display the sorted array.
11. Stop.

---

## Example

**Input**

```
12 11 13 5 6
```

**Output**

```
5 6 11 12 13
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

---

## Space Complexity

```
O(1)
```

---

## Advantages

- Simple and easy to implement.
- Efficient for small datasets.
- Performs well on nearly sorted data.
- Stable sorting algorithm.
- Requires constant extra memory.

---

## Disadvantages

- Inefficient for large datasets.
- More comparisons and shifts for randomly ordered data.
- Slower than Merge Sort and Quick Sort on large inputs.

---

## Applications

- Sorting small datasets.
- Sorting nearly sorted data.
- Used as a subroutine in advanced sorting algorithms.
- Suitable when memory usage must be minimal.

---

## Conclusion

Insertion Sort is an efficient algorithm for small or nearly sorted datasets. It inserts each element into its correct position in the sorted part of the array. Although its average and worst-case time complexity is O(n²), its simplicity and low memory usage make it useful in many practical situations.