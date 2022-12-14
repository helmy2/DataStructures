## Doubly Linked List

A linked list that provides forward iteration from the start to the end of the list,
and reverse iteration, from end to start.
![Doubly linked list image](../images/doubly-linked-list.webp)
We add a pointer to the previous node in a doubly-linked list. Thus, we can go in either direction: forward or backward.

### Time Complexity

|            | Worst case      | Average Case       |
|------------|-----------------|--------------------|
| Search     | O(n)            | O(n)               |
| Insert     | O(1)            | O(1)               |
| Deletion   | O(1)            | O(1)               |

### Space Complexity

    O(n)

### Linked List Applications

- Dynamic memory allocation
- Implemented in stack and queue
- In undo functionality of software
- Hash tables, Graphs

### Usage

- [Doubly Linked List implementation](../src/main/java/org/example/linked_list/DoublyLinkedList.java)
- [Doubly Linked List Test](../src/test/java/org/example/linked_list/DoublyLinkedListTest.java)
- Create
    ```java
    DoublyLinkedList<Integer> linkedList = new DoublyLinkedList<>();
    ```

- isEmpty
  ```java
  boolean empty = linkedList.isEmpty();
  ```
  > check if the list is empty

  > Complexity **O(1)**

- getHead
  ```java
  Integer result = linkedList.getHead();
  ```
  > return The last node in the first or null if empty

  > Complexity **O(1)**

- getTail
  ```java
  Integer result = linkedList.getTail();
  ```
  > return The last node in the last or null if empty

  > Complexity **O(1)**

- addHead
  ```java
  Integer value = 10;
  linkedList.addHead(value);
  ```
  > Adds the specified value to the start of the linked list

  > Complexity **O(1)**

- addTail
  ```java
  Integer value = 10;
  linkedList.addTail(value);
  ```
  > Adds the specified value to the end of the linked list

  > Complexity **O(1)**

- find
  ```java
  Integer value = 10;
  Node found = find(value);
  ```
  > Finds the first node whose value equals the provided argument

  > Complexity **O(n)**

- contains
  ```java
  Integer value = 10;
  boolean isfound = linkedList.contain(value);
  ```
  > Returns true if the specified value exists in the list, false otherwise

  > Complexity **O(n)**

- remove
  ```java
  Integer value = 10;
  boolean isRemoved = linkedList.remove(value);
  ```
  > Removes the first node whose value is equal to the argument

  > Complexity **O(n)**

- removeHead
  ```java
  Integer value = 10;
  boolean isRemoved = linkedList.removeHead(value);
  ```
  > Removes the start node from the list.

  > Complexity **O(1)**

- removeTail
  ```java
  Integer value = 10;
  boolean isRemoved = linkedList.removeTail(value);
  ```
  > Removes the end node from the list.

  > Complexity **O(1)**

- iterator
  ```java
  Iterator<Integer>  iterator = linkedList.iterator();
  ```
  > Iterate over the linked list values from Head to Tail

  > Complexity **O(n)**

- reverseIterator
  ```java
   Iterator<Integer>  iterator = linkedList.reverseIterator();
  ```
  > Iterate over the linked list values from Tail to Head

  > Complexity **O(n)**
  