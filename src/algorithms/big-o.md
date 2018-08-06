## What is Big O notation?

Big-O notation is a way of converting the overall steps of an algorithm into algebraic terms, then excluding lower order constants and coefficients that don't have that big an impact on the overall complexity of the problem.

- O(1) - **constant time**: given an input size n, it only takes a single step for the algorithm to accomplish the task
- O(log n) - **logarithmic time**: given an input size n, the number of steps it takes to accomplish the task are decreased by some factor with each step
- O(n) - **linear time**: given an input of size n, the number of steps required is directly related (1 to 1)
- O(n<sup>2</sup>) - **quadratic time**: given an input of size n, the number of steps it takes to accomplish a task is square of n
- O(C<sup>n</sup>) - **exponential time**: given an input of size n, the number of steps it takes to accomplish a task is a constant to the n power (pretty large number)


### Quadratic
- quadratic algorithms don't scale with technology
  - new computer may be 10x as fast, but has 10x as much memory, so to solve a problem that is 10x as big, it will take 10x as long!
- too slow
- gets slower as data gets bigger
- examples
  - loop within a loop (nested loop executes total of N * N times) which equals to O(N<sup>2</sup>)
  - performing linear search in matrix
  - time complexity of quick sort
  - insertion sort
- algorithms that scale in quadratic time are better to be avoided, once the input size reaches n = 100,000 element, it can take 10 seconds to complete, n = 1,000,000 can take ~16 min to complete... etc.
