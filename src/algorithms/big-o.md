## What is Big O notation?

Big-O notation is a way of converting the overall steps of an algorithm into algebraic terms, then excluding lower order constants and coefficients that don't have that big an impact on the overall complexity of the problem.

- O(1) - **constant time**: given an input size n, it only takes a single step for the algorithm to accomplish the task
- O(log n) - **logarithmic time**: given an input size n, the number of steps it takes to accomplish the task are decreased by some factor with each step
- O(n) - **linear time**: given an input of size n, the number of steps required is directly related (1 to 1)
- O(n<sup>2</sup>) - **quadratic time**: given an input of size n, the number of steps it takes to accomplish a task is square of n
- O(C<sup>n</sup>) - **exponential time**: given an input of size n, the number of steps it takes to accomplish a task is a constant to the n power (pretty large number)
