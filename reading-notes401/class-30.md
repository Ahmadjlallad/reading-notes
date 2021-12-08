# hash table

- What is a hash table simple explanation?
  A hash table is a data structure that uses a hash function to keep track of where data is put. Each piece of information to be stored has a name, which is called a key. For example, a key might be a person's name. Each name is matched up to one piece of data called a value, like the person's telephone number.
- hash table advantage

  - Hold unique values
  - Dictionary
  - Library

- What Are they

  - Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

- Hashing
  Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.

- Creating a Hash
  A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:

- Add or multiply all the ASCII values together.
  Multiply it by a prime number such as 599.
  Use modulo to get the remainder of the result, when divided by the total size of the array.
  Insert into the array at that index.
- Collisions
  A collision occurs when more than one key hashes to the same index in an array. As mentioned earlier, a “perfect hash” will never have any collisions. To put this into perspective, the worst possible hash is one that hashes every single key to the same exact index of an array. The more keys you have hashed to a specific index, the more key/value pair combos you can potentially have.

- Hash maps do this to store values:

accept a key
calculate the hash of the key
use modulus to convert the hash into an array index
store the key with the value by appending both to the end of a linked list

- Hash maps do this to read value:

accept a key
calculate the hash of the key
use modulus to convert the hash into an array index
use the array index to access the short LinkedList representing a bucket
search through the bucket looking for a node with a key/value pair that matches the key you were given

Internal Methods
Add()
When adding a new key/value pair to a hashtable:

send the key to the GetHash method.
Once you determine the index of where it should be placed, go to that index
Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
If something does exist, add the new key/value pair to the data structure within that bucket.
Find()
The Find takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

Contains()
The Contains method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the GetHash and check the hashtable if the key exists in the table given the index returned.

GetHash()
The GetHash will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
