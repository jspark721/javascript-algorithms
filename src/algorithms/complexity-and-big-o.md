## Complexity and Big-O Notation

### How efficient is an algorithm or piece of code?
- CPU (time) usage
- memory usage
- disk usage
- network usage

#### _Differentiate between performance and complexity_
1. **performance**: how much time/memory/disk.. is actually used when a program is run. This depends on the machine, complier, etc. as well as the code.
2. **complexity**: how do the resource requirements of a program or algorithm scale, i.e., what happens as the size of the problem being solved gets bigger

#### Complexity affects performance but not the other way around

##### The time required by a method is proportional to the number of "basic operations" that it performs

examples of **basic operations**:
- one arithmetic operation (e.g., +, *)
- one assignment
- one test (e.g., x == 0)
- one read
- one write (of a primitive type)

**constant time**: methods that always perform just one operation and it's independent of the size of the _list_ (data, array, etc)

**important factors** (the paragmeters and/or fields whose values affect the number of operations performed): the **problem size** or the **input size**

when we consider the **complexity** of a method, we don't really care about the **exact** number of operations that are performed; instead, we care about how the number of operations relates to the problem size

usually interested in the **worst case**: what is the **most** operations that might be performed for a given problem size

### Complexity Examples

Assume lists are implemented using an array, for each of the following _List_ methods, say whether (in the worst case) the number of operations is independent of the size of the list (**constant-time** method) or is proportional to the size of the list (**linear-time** method)

- **constructor**: this method allocates the initial array, sets current to -1 and sets numItems to 0. It has nothing to do with the sequence size and is **constant-time**
- _add_ (to the end of the list): in the worst case, the array was full and you have to allocate a new, larger array and _copy_ **all** the items -- in this case, the number of operations is proportional to the size of the list. So it's **linear-time** if the list is full, but **constant-time** if the array is not full because all you have to do is copy one value into the array and increment numItems
- _add_ (at a given position in the list): if the array is full, it's proportional - however, even if the array is not full this _add_ can require time proportional to the size of the list because when adding at position _k_, all of the items in positions _k_ to the end must be moved over
- _isEmpty_: this method simply returns the result of comparing numItems with 0; this is a **constant-time** operation
- _contains_: this method involves looking at each item in the list to see if it's equal to the given item - in the worst case, (the given item is at the end of the list, or not in the list at all), it's proportional to the size of the list -- **linear-time**
- _get_: this method checks for a bad position and either throws an exception or returns the value in the given position in the array- in either case, it is independent of the size of the list- so it's a **constant-time** operation
