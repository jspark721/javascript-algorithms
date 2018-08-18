### JavaScript Hash Table

a data structure used to implement an associate array, a structure that can map keys to values -- **hash table** uses a hash function to compute an index into an array of buckets or slots, from which the desired value can be found.

- hash tables combine the random access ability of an array with the dynamism of a linked list
- assuming the hash table is implemented well
  - insertion get towards close to O(1)
  - deletion get towards close to O(1)
  - lookup get towards close to O(1)
- combine the advantages of an array and linked list while mitigating the disadvantages
- the trade off is that hash tables are not great at ordering or sorting data
