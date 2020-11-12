## Implementation: Hash Tables
To turn in your reading “Reply” to this discussion by teaching something that you learned from the readings listed below.

Hash tables are a data structure that is used to store large amounts of key value pairs for efficient retrieval.  A typical hash table stores elements along two axises, an array, where each slot is called a bucket, and a linked list within each bucket.  To store an element, the key is run through a hash function to determine which index of the array or 'bucket' the element should be stored in.  Then, the element is saved as a node in a linked list within that bucket.  Multiple keys may resolve to the same hash value, this is called colliding.  If a key collides and is stored in a bucket that already contains data, it is appended to the linked list that already exists within that bucket.  To retrieve data, the searched item's key is run against the hash function to return the index of the array to begin searching.  From there, the program will search the linked list until the desired key:value pair is returned.


## Resources

[Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
[what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
[basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
[hash table wiki](https://en.wikipedia.org/wiki/Hash_table)