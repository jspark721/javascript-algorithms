## Guiding Principles for Analysis of algorithms

### Guiding Principle #1
- **worst-case analysis**: the running time bound holds for __every__ input of length n. calculate the upper bound on running time of an algorithm - know the case that causes maximum number of operations to be executed (__**EASIER TO ANALYZE**__)
- **average-case analysis**: analyze the average running time of an algorithm under some assumption about the relative frequencies of different inputs.
  - for example, in the sorting problem, you could assume that every possible input array is equally unlikely and then analyze the average running time of an algorithm
  - benchmark input - which are thought to represent practical or typical inputs for the algorithm

worst case analysis is particularly appropriate for "general-purpose" routines and usually mathematically much more attractable than trying to analyze the average performance of an algorithm on a particular set of benchmark inputs


### Guiding Principle #2
- don't worry about small constant factors or lower order terms
- **justifications**: 1. simply way easier mathematically 2. constants depend on architecture/ complier/ programmer etc. 3. we can just get away with it, we'll still get extremely accurate predictive power without the constant factors
<small>this does NOT mean that constant factors aren't important in practice - the point is just that understanding tiny constant factors in analysis is not necessary</small>


### Guiding Principle #3
-**asymptotic analysis**: focus on the case/running time of a large input size - (to infinity)
-**justifications**: (only big problems are interesting!)

as computers get faster, we think about how much a bigger a problem size we can solve
