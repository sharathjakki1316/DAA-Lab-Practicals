# Selection Sort Algorithm

## Aim

To sort a list of elements in ascending order using the Selection Sort algorithm.

---

## Objective

- To understand the working of Selection Sort.
- To sort elements by repeatedly selecting the smallest element.
- To analyze the time and space complexity of Selection Sort.

---

## Introduction

Selection Sort is a simple comparison-based sorting algorithm. It repeatedly finds the smallest element from the unsorted portion of the array and places it at the beginning of the sorted portion. This process continues until the entire array is sorted.

---

## Algorithm

1. Start.
2. Read the number of elements.
3. Read the array elements.
4. Assume the first unsorted element is the minimum.
5. Compare it with the remaining unsorted elements.
6. Find the smallest element in the unsorted portion.
7. Swap the smallest element with the first unsorted element.
8. Repeat Steps 4–7 until all elements are sorted.
9. Display the sorted array.
10. Stop.

---

## Example

**Input**

```
64 25 12 22 11
```

**Output**

```
11 12 22 25 64
```

---

## Time Complexity

| Case | Complexity |
|------|------------|
| Best Case | O(n²) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

---

## Space Complexity

```
O(1)
```

---

## Advantages

- Simple and easy to understand.
- Performs a minimum number of swaps.
- Requires constant extra memory.
- Suitable for small datasets.

---

## Disadvantages

- Inefficient for large datasets.
- Time complexity remains O(n²) even for sorted arrays.
- Not a stable sorting algorithm in its basic implementation.

---

## Applications

- Educational purposes.
- Small datasets.
- Situations where minimizing the number of swaps is important.

---

## Conclusion

Selection Sort repeatedly selects the smallest element from the unsorted portion of the array and places it in its correct position. Although it is simple to implement and requires only constant extra memory, its O(n²) time complexity makes it unsuitable for large datasets.