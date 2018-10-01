## Asymptotic Analysis

The design & analysis of algorithms (e.g., "the big-o notation")
- the sweet spot for high-level reasoning about Algorithms
- coarse enough to suppress architecture/ choice of programming language/ compiler/
- sharp enough to make useful comparisons between different algorithms, especially true for large inputs (e.g., sorting or integer multiplication, etc.)

##### High-level idea: suppress constant factors & lower-order terms

constant factors: too system-dependent
lower-order terms: irrelevant for large inputs

## Three Forms: big-Θ (Theta) notation, big-O notation, and big-Ω (Omega) notation.

- big-Θ: asymptotic tight bounds on the running time **gives both**
- big-O: asymptotic upper bounds (since it bounds the growth of the running time from above for larget enough input sizes) **worst case running time**
  - example: (one million dollars is an upper bound on 10 dollars, just as O(n) is an upper bound on the running time of binary search)
- big-Ω: asympototic lower bounds // **best case** running time for a given algorithm

[Big-O, Little-o, Theta, Omega][5f24ce76]

  [5f24ce76]: https://cathyatseneca.gitbooks.io/data-structures-and-algorithms/content/analysis/notations.html "Big-O, Little-o, Theta, Omega"
