# Project Title: Binomial Heap Implementation

## Project Description

This project involves the implementation of a Binomial Heap in Java as part of a Data Structures course. The Binomial Heap is a specific type of heap data structure that supports quick merging of two heaps.

## Repository Structure

- `BinomialHeap.java`: Contains the source code for the Binomial Heap implementation.
- `README.md`: Project overview and instructions.

## Requirements

- **Programming Language**: Java 17
- **Libraries**: No external libraries are used. The implementation based solely on standard Java.

## Implementation Details

The Binomial Heap implementation include the following functionalities:

- **Insert**: `insert(int key, String info)` - Inserts a node with key `key` and value `info` into the heap, returns the created `HeapItem`.
- **Delete Min**: `deleteMin()` - Deletes the minimum key node from the heap.
- **Find Min**: `findMin()` - Returns the node with the minimum key in the heap.
- **Decrease Key**: `decreaseKey(HeapItem item, int diff)` - Decreases the key of node `item` by `diff` and rebalances the heap.
- **Delete**: `delete(HeapItem item)` - Deletes the node `item` from the heap.
- **Meld**: `meld(BinomialHeap heap2)` - Merges the current heap with another heap `heap2`.
- **Size**: `size()` - Returns the number of elements in the heap.
- **Empty**: `empty()` - Returns whether the heap is empty.
- **Num Trees**: `numTrees()` - Returns the number of binomial trees in the heap.
- **Find Previous**: `findPrevious(HeapNode node)` - Returns the previous node of the given node.
- **Find New Min**: `findNewMin()` - Searches and returns the new minimal `HeapItem`.
- **Link**: `link(HeapNode x, HeapNode y)` - Links two heap nodes with the same rank into one.
- **Merge**: `merge(BinomialHeap heap2)` - Merges two Binomial Heaps into one without linking nodes with the same rank.
- **Heap to Array**: `HeapToArray(BinomialHeap heap)` - Converts a Binomial Heap to an array.
- **Array to Heap**: `ArrayToHeap(HeapNode[] arr)` - Converts an array to a Binomial Heap.

### Classes

- **HeapNode**: Represents a node in the binomial heap.
  - `item` - The heap item stored in this node.
  - `child` - The child node with the maximum rank.
  - `next` - The next sibling node in the circular list.
  - `parent` - The parent node in the heap.
  - `rank` - The rank of the binomial tree rooted at this node.
  - Methods to set `item`, `child`, `next`, `parent`, and `rank`.

- **HeapItem**: Represents an item in the binomial heap.
  - `key` - The key stored in this item.
  - `info` - The information stored in this item.
  - `node` - The heap node where this item is stored.
  - Methods to set `node`, `key`, and `info`.
