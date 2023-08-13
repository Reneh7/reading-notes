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