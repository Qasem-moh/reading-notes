# Hash Tables
* **Hashtables** are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value
* **Hash** is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array to store the key into this data structure, and quickly retrieve the value.

* **Buckets** is what is contained in each index of the array of the hashtable. Each Index of the array contain “buckets”.. Each of these “buckets” holds one key/value pair combination. The hash table starts each bucket empty and overwrites their value once a key generates a hashCode that corresponds with an index.

* **Collisions** is what happens when more than one key gets hashed to the same location of the hashtable(same index of the array), it's solved by changing the initial state of the buckets. Instead of starting them all as null we can initialize a LinkedList in each one

* **usage** 
    1. Hold unique values
    2. Dictionary
    3. Library

* constant time to the hash map is ``O(1)``
* hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

## Structure
*  a hash code turns a key into an integer
*  hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.
* hashtable traditionally is created from an ar
* steps"
    1. determine size of array ``===>1024``
    2. Add or multiply all the ASCII values together. ``Key = "Cat" ====>67 + 97 + 116 = 280``
    3. Multiply it by a prime number such as 599. ``280 * 599 = 69648``
    4. Use modulo to get the remainder of the result, when divided by the total size of the array. ``69648 % 1024 = 16``
    5. Insert into the array at that index. ``Key gets placed in index of 16``
