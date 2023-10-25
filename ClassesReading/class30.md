# Android Reading 5

## Analogy - "The Library Analogy"

 Imagine a library as a giant collection of books. When you want to find a specific book, you don't want to search through every book in the library. Instead, the library uses a card catalog where each book is listed with its title and the location of the book on the shelf. In this analogy, the card catalog is like a hash table. It helps you quickly find the book you're looking for by indexing it based on its title (key).

## In-Depth Explanation - "How Hash Tables Work"

Hash tables are data structures that use a hash function to map keys to specific locations in an array. The hash function takes the key as input and produces an index in the array where the data associated with that key is stored. Hash tables are used to achieve constant-time (O(1)) access to data, making them efficient for tasks like data retrieval and data insertion.

## What, why, how

- What: A hash table is a data structure that stores key-value pairs and uses a hash function to determine the index for each key.
- Why: Hash tables provide fast access to data based on a key, making them ideal for tasks like searching, indexing, and caching.
- How:
Create a hash table.
Choose a hash function to map keys to indices.
Handle collisions (when multiple keys hash to the same index).
Insert, retrieve, and delete data from the hash table efficiently.