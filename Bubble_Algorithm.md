# Bubble Sort Algorithm

## Aim

To sort a list of elements in ascending order using the Bubble Sort algorithm.

---

## Objective

- To understand the working of Bubble Sort.
- To arrange elements in ascending order.
- To analyze the time and space complexity of Bubble Sort.

---

## Introduction

Bubble Sort is one of the simplest sorting algorithms. It repeatedly compares two adjacent elements and swaps them if they are in the wrong order. After each pass, the largest unsorted element moves to its correct position, just like a bubble rises to the surface of water.

---

## Algorithm

1. Start.
2. Read the number of elements.
3. Read the array elements.
4. Compare each pair of adjacent elements.
5. If the first element is greater than the second element, swap them.
6. Repeat the process for all elements in the array.
7. Continue the passes until the array is completely sorted.
8. Display the sorted array.
9. Stop.

---

## Example

**Input**

```
64 34 25 12 22 11 90
```

**Output**

```
11 12 22 25 34 64 90
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

- Easy to understand.
- Easy to implement.
- Stable sorting algorithm.
- Suitable for small datasets.

---

## Disadvantages

- Slow for large datasets.
- Performs many unnecessary comparisons.
- Not efficient compared to Merge Sort or Quick Sort.

---

## Applications

- Educational purposes.
- Small datasets.
- When simplicity is more important than efficiency.

---

## Conclusion

Bubble Sort is a simple comparison-based sorting algorithm. Although it is easy to understand and implement, it is inefficient for large datasets because its average and worst-case time complexity is O(n²). It is mainly used for learning basic sorting concepts.