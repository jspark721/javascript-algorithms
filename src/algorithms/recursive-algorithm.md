## Recursive Algorithms

**recursion** means "defining a problem in terms of itself". this can be a powerful tool in writing algorithms. __recursion is the process of defining a problem (or solution to a problem) in terms of (a simpler version of) itself__

#### recursion in computer science is a method of solving a problem where the solution depends on solutions to smaller instances of the same problem (as opposed to iteration)

> "the power of recursion evidently lies in the possibility of defining an infinite set of objects by a finite statement. in the same manner, an infinite number of computations can be described by a finite recursive program, even if this program contains no explicit repetitions."

**A recursive algorithm is an algorithm which calls itself with "smaller (or simpler)" input values, and which obtains the result for the current input by applying simple operations to the returned value for the smaller (or simpler) input.**

### What is Recursion?

The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc.

#### What is base condition in recursion?
In recursive program, the solution to base case is provided and solution of bigger problem is expressed in terms of smaller problems.

#### How a particular problem is solved using recursion?
The idea is represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop recursion. For example, we compute factorial n if we know factorial of (n-1). Base case for factorial would be n = 0. We return 1 when n = 0.

__in a recursive algorithm, the computer "remembers" every previous state of the problem. this information is "held" by the computer on the "**activation stack**" (i.e., inside of each functions workspace)__

## recursion is where a function calls itself

[how recursion works (simple explanation)](https://medium.freecodecamp.org/how-recursion-works-explained-with-flowcharts-and-a-video-de61f40cb7f9)

#### recursive approach in pseudocode
```
function look_for_key(box) {
  for (item in box) {
    if (item.is_a_box()) {
      look_for_key(item)
    } else if (item.is_a_key()) {
      console.log("found the key!")
    }
  }
}
```

there is no performance benefit to using recursion over the iterative approach with loops - it can just be clearer to read (simplicity of recursion is sometimes preferred)
