# Class five Reading

## WHY, WHAT, HOW teaching method

- Why: Linked arrays are used when the number of elements is unknown or may change dynamically, as they allow efficient addition and removal.
- What: Linked arrays consist of individual elements containing data and pointers to the next element.
- How: To create a linked array, each element is created with data and a reference to the next element. This forms a chain that can be traversed, added to, or removed from easily.

## Example 

```java
public class LinkedArrayExample {
    public static void main(String[] args) {
        LinkedArrayElement first = new LinkedArrayElement(5);
        LinkedArrayElement second = new LinkedArrayElement(10);
        LinkedArrayElement third = new LinkedArrayElement(15);

        first.next = second;
        second.next = third;

        LinkedArrayElement current = first;
        while (current != null) {
            System.out.println("Value: " + current.value);
            current = current.next;
        }
    }
}


class LinkedArrayElement {
    int value;
    LinkedArrayElement next;

    public LinkedArrayElement(int value) {
        this.value = value;
        this.next = null;
    }
}
```

## Vocabulary/Definition List for Stack and Heap Memories

Stack Memory: A region of memory used for storing function call information, local variables, and control flow data. It follows the Last-In-First-Out (LIFO) principle.

Heap Memory: A dynamically allocated memory region used for managing complex data structures, such as objects and arrays. Memory allocation and deallocation are controlled by the programmer.

Allocation: The process of reserving a portion of memory for data storage. In the stack, memory is automatically allocated and deallocated as functions are called and returned. In the heap, manual allocation and deallocation are necessary.

Deallocation: The process of releasing memory that is no longer needed, making it available for reuse. This is particularly important in heap memory to prevent memory leaks.

Local Variables: Variables defined within a function that are stored in the stack memory. They have limited scope and are destroyed when the function exits.

Dynamic Memory Allocation: The process of requesting and releasing memory at runtime from the heap. It enables creating data structures whose size is determined during program execution.

Memory Leak: A situation where memory that was allocated in the heap is not properly deallocated, leading to a gradual loss of available memory over time.

Stack Overflow: An error that occurs when the stack memory is exhausted due to excessive function calls or large local variable allocations.

## Visualization / Cartoon of Stack and Heap Memories

Imagine memory as a bookshelf: The stack is like a stack of books, with each book representing a function call. As you add more books (function calls) to the stack, you have to finish reading the top book before moving to the one below. When you're done, you remove the top book (function call) from the stack.

On the other hand, the heap is like a storage room where you can place items (data) wherever you find space. You're responsible for putting things in and taking them out. If you forget to take something out, the storage room could get cluttered and messy (memory leak).

In this visual, the stack represents organized and automatic management, while the heap represents manual control over memory. It's important to keep both tidy to ensure efficient memory usage.