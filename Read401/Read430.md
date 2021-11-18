# Hashtables

### What is a Hashtable?


* Hash is the output of an operation of converting a string value to a value that could be used for either security or some other purpose.

* Buckets is the contents of each index in hashtable.

* Collisions - A collision is what happens when more than one key is hashed to the same location of the hash.

### Why do we use them?

1. Hold unique values
2. Dictionary
3. Library

### What Are they

* Hashtables are a data structure that utilize key value pairs. (key ,value)

* The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value.

* Hash functions are used to convert large keys smaller ones.

* The quick retrieving of values that are stored in hashtable is the main idea of using them, since the time complexity is O(1).

### Hashing

* a hash code turns a key into an integer.

* Hash codes should never have randomness to them. The same key should always produce the same hash code.


### Collisions

1. A collision occurs when more than one key hashes to the same index in an array and a “perfect hash” will never have any collisions.

2. Collisions are solved by changing the initial state of the buckets.


### Hashmaps store and read the values

**Hash maps do this to store values:**

1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. store the key with the value by appending both to the end of a linked list

**Hash maps do this to read value:**

1. accept a key
2. calculate the hash of the key
3. use modulus to convert the hash into an array index
4. use the array index to access the short LinkedList representing a bucket
5. search through the bucket looking for a node with a key/value pair that matches the key you were given



### What is the benifits of Hash ,Buckets,Collisions

1. Hold unique values
2. Dictionary
4. Library

### Internal Methods :

1. Add()
2. Find()
3. Contains()
4. GetHash()

**************
[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

[what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)

[basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
**************