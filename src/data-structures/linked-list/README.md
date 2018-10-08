# Linked List

In computer science, a **linked list** is a linear collection
of data elements, in which linear order is not given by
their physical placement in memory. Instead, each
element points to the next. It is a data structure
consisting of a group of nodes which together represent
a sequence. Under the simplest form, each node is
composed of data and a reference (in other words,
a link) to the next node in the sequence. This structure
allows for efficient insertion or removal of elements
from any position in the sequence during iteration.
More complex variants add additional links, allowing
efficient insertion or removal from arbitrary element
references. A drawback of linked lists is that access
time is linear (and difficult to pipeline). Faster
access, such as random access, is not feasible. Arrays
have better cache locality as compared to linked lists.

![Linked List](https://upload.wikimedia.org/wikipedia/commons/6/6d/Singly-linked-list.svg)

## References

- [Wikipedia](https://en.wikipedia.org/wiki/Linked_list)
- [YouTube](https://www.youtube.com/watch?v=njTh_OwMljA&index=2&t=1s&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)

## More Notes

**data structure** consisting of a collection of nodes which together represent a sequence

each **node** contains:
- data
- reference (in other words, a _link_)
- the last node has a reference to _null_
- the entry point into a linked list is called the **head** of the list (head is not a separate node, but the reference to the first node)
  - if the list list is empty, then the head is a null reference

this structure allows for efficient insertion or removal of nodes at arbitrary positions.

- arrays are static structure and cannot be easily extended or reduced to fit the data set
- arrays are also expensive to maintain new insertions and deletions

linked list is a _linear data structure_ where each element is a _separate object_

#### Linked List is a dynamic data structure
> the number of nodes in a list is not fixed and can grow and shrink on demand -- any application which deals with unknown number of objects will need to use a linked list

#### Disadvantage of Linked List
- it uses more memory compared to an array
- access time is linear (difficult to pipeline)
- faster access (such as random access) is not feasible
- arrays have better cache locality compared to linked lists
- nodes are stored incontiguously, greatly increasing the time periods required to access individual elements within the list (especially with a CPU cache)
- difficulties arise when it comes to reverse traversing

### Types of Linked Lists
- **singly linked list** - a list that has reference to the next node in line of nodes (a link to the next node)
- **doubly linked list** - a list that has two references, one to the next node and another to previous node
- **multiply linked list** - each node contains two or more link fields, each field being used to connect the same set of data records in a different order of the same set (e.g., by name, by department, by date of birth, etc)
- **circular linked list** - last node of the list points back to the first node (or the head) of the list
