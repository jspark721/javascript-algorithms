# Hash Table

In computing, a **hash table** (hash map) is a data
structure which implements an *associative array*
abstract data type, a structure that can *map keys
to values*. A hash table uses a *hash function* to
compute an index into an array of buckets or slots,
from which the desired value can be found

Ideally, the hash function will assign each key to a
unique bucket, but most hash table designs employ an
imperfect hash function, which might cause hash
collisions where the hash function generates the same
index for more than one key. Such collisions must be
accommodated in some way.

![Hash Table](https://upload.wikimedia.org/wikipedia/commons/7/7d/Hash_table_3_1_1_0_1_0_0_SP.svg)

Hash collision resolved by separate chaining.

![Hash Collision](https://upload.wikimedia.org/wikipedia/commons/d/d0/Hash_table_5_0_1_1_1_1_1_LL.svg)

## References

- [Wikipedia](https://en.wikipedia.org/wiki/Hash_table)
- [YouTube](https://www.youtube.com/watch?v=shs0KM3wKv8&index=4&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)

## More Notes

In a hash table, data is stored in an array format, where each data value has its own unique index value - acces of data becomes very fast if we know the index of the desired data

**Hashing** is a technique to convert a range of key values into a range of indexes of an array

##### Basic Operations
**Search** - searches an element in a hash table
**Insert** - inserts an element in a hash table
**delete** - deletes an element from a hash table

> a hash table is a data structure that maps keys to values for highly efficient lookup. there are a number of ways of implementing a hash table
