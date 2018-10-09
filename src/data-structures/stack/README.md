# Stack

In computer science, a **stack** is an abstract data type that serves
as a collection of elements, with two principal operations:

* **push**, which adds an element to the collection, and
* **pop**, which removes the most recently added element that was not yet removed.

The order in which elements come off a stack gives rise to its
alternative name, LIFO (last in, first out). Additionally, a
peek operation may give access to the top without modifying
the stack. The name "stack" for this type of structure comes
from the analogy to a set of physical items stacked on top of
each other, which makes it easy to take an item off the top
of the stack, while getting to an item deeper in the stack
may require taking off multiple other items first

Simple representation of a stack runtime with push and pop operations.

![Stack](https://upload.wikimedia.org/wikipedia/commons/b/b4/Lifo_stack.png)

## References

- [Wikipedia](https://en.wikipedia.org/wiki/Stack_(abstract_data_type))
- [YouTube](https://www.youtube.com/watch?v=wjI1WNcIntg&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8&index=3&)

## More Notes

examples - stack of books, stack of plates, using the back and forward button on your browser, stack of pancakes :P
**the undo button**

_always add to the top of the stack(push)_
_always remove from the top of the stack(pop)_

**Top** is **O(1)** - the current position is always known
**Find** (search) would be **O(n)** - you would technically have to iterate over your storage until you found the value you were looking for (essentially the _indexOf_ method on Arrays)
