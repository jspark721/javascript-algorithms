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
