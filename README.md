# MaxHeap Implementation in Python

## Overview
This project demonstrates a **MaxHeap** data structure built from scratch in Python. A MaxHeap is a binary heap where the **parent node is always greater than or equal to its children**, making it useful for priority queues and sorting algorithms.

The MaxHeap in this project supports:

- **Insert**: Add a new element while maintaining the heap property.
- **Pop**: Remove and return the maximum element.
- **Heapify-Up**: Restore the heap property after insertion.
- **Heapify-Down**: Restore the heap property after removing the maximum.

The project also demonstrates using the MaxHeap to **sort integers in descending order**.

---

## Features
- Custom MaxHeap class implemented from scratch.
- Efficient insertion and removal operations.
- Automatically maintains heap property using heapify-up and heapify-down.
- Visual demonstration of sorting elements by repeatedly popping the maximum.

---

## Example Usage

```python
# Sample usage
heap = MaxHeap()
for num in [15, 10, 30, 40, 20]:
    heap.insert(num)

print("Heap after insertions:", heap.data)

print("Popping elements in descending order:")
while heap.data:
    print(heap.pop())
