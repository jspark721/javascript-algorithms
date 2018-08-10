### Merge sort is a _divide and conquer_ algorithm

an efficient, general-purpose, comparison based sorting algorithm

> Merge sort is a divide-and-conquer algorithm based on the idea of breaking down a list into several sub-lists until each sublist consists of a single element and merging those sublists in a manner that results into a sorted list.

- divides input array in two halves, call itself for the two halves and then merges the two sorted halves

**idea:**
- divide the unsorted list into _**N**_ sublists, each containing 1 element
- take adjacent pairs of two singleton lists and merge them to form a list of 2 elements. _**N**_ will now convert into _**N/2**_ lists of size 2
- repeat the process until a single sorted list is obtained

while comparing two sublists for merging, the first element of both lists is taken into consideration - while sorting in ascending order, the element that is of a lesser value becomes a new element of the sorted list - this procedure is repeated until both the smaller sublists are empty and the new combined sublist comprises all the elements of both the sublists

![Merge Sort](images/2018/08/merge-sort.png)

### time complexity:
the list of size _**N**_ is divided into a max of _**logN**_ parts, and the merging of all sublists into a single list takes _**O(N)**_ time, the **worst case** run time of this algorithm is _**O(NLogN)**_
