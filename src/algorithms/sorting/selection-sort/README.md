# Selection Sort

Selection sort is a sorting algorithm, specifically an
in-place comparison sort. It has O(n2) time complexity,
making it inefficient on large lists, and generally
performs worse than the similar insertion sort.
Selection sort is noted for its simplicity, and it has
performance advantages over more complicated algorithms
in certain situations, particularly where auxiliary
memory is limited.

![Algorithm Visualization](https://upload.wikimedia.org/wikipedia/commons/b/b0/Selection_sort_animation.gif)

![Algorithm Visualization](https://upload.wikimedia.org/wikipedia/commons/9/94/Selection-Sort-Animation.gif)

## Complexity

| Name                  | Best            | Average             | Worst               | Memory    | Stable    | Comments  |
| --------------------- | :-------------: | :-----------------: | :-----------------: | :-------: | :-------: | :-------- |
| **Selection sort**    | n<sup>2</sup>   | n<sup>2</sup>       | n<sup>2</sup>       | 1         | No        |           |

## References

[Wikipedia](https://en.wikipedia.org/wiki/Selection_sort)

## More Notes

The list is divided into two parts, the sorted part at the left end and the unsorted part at the right end - initially, the sorted part is empty and the unsorted part is the entire list

The smallest element is selected from the unsorted array and swapped with the leftmost element and that element becomes a part of the sorted array. The process continues moving through the unsorted array boundary by one element to the right

**not suitable for large data sets as its average and worst case complexities are Ο(n<sup>2</sup>)
