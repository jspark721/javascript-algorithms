## What is Big O notation?

Big-O notation is a way of converting the overall steps of an algorithm into algebraic terms, then excluding lower order constants and coefficients that don't have that big an impact on the overall complexity of the problem.

#### Big O Notation is used in computer science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario and can be used to describe the execution time required or the space used by an algorithm

- O(1) - **constant time**: given an input size n, it only takes a single step for the algorithm to accomplish the task
  - _describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set_
- O(log n) - **logarithmic time**: given an input size n, the number of steps it takes to accomplish the task are decreased by some factor with each step
  - _binary search_ used to search sorted data sets -- it works by selecting the middle element of the data set (essentially a median) and compares it against a target value. if the values match, it will return success - if the target value is higher than the value, it will take the upper half of the data set and perform the same operation against it - it will continue to halve the data set with each iteration until the value has been found or until it can no longer split the data
  - _iterative halving of data sets produces a growth curve that peaks at the beginning and slowly flattens out as the size of the data sets increase_
  - doubling the size of the input data set has little effect on its growth as after a single iteration of the algorithm the data set will be halved and therefore on a par with an input data set half the size 
- O(n) - **linear time**: given an input of size n, the number of steps required is directly related (1 to 1)
  - _describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set_
- O(n<sup>2</sup>) - **quadratic time**: given an input of size n, the number of steps it takes to accomplish a task is square of n
  - _represents an algorithm whose performance is directly proportional to the square of the size of the input data set - this is common with algorithms that involve nested iterations over the data set_
  - deeper nested iterations will result in O(N<sup>3</sup>), O(N<sup>4</sup>) etc.
- O(C<sup>n</sup>) - **exponential time**: given an input of size n, the number of steps it takes to accomplish a task is a constant to the n power (pretty large number)
  - _denotes an algorithm whose growth doubles with each addition to the input data set_
  - starting off very shallow, then rising meteorically
  - an example of an O(2<sup>n</sup>) function is the recursive calculation of Fibonacci numbers


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
