# Data Structures :

## Arrays :

```

How RAM works (Random access memory) - Measured in Bytes.

1 byte - 8 bits
1 bit - can store either 1/0 (binary value)

All values we want to store in memory can be represented in binary. And thats how they are stored in the ram.
ex : 1 -> binary notation 0001 ; for type int in X64 arch. the int data type is 64 bits / 8 bytes long.
    so it will be stored in memory as 63 x 0's and 1 (...0001)

=> Two parts of ram : Addr + value

* for an int64 array - the Addr will be in increments of 8. 
* ex : [0, 8, 16, ...] -> each address represents the starting position of 8 bytes that can store value.
    so the first value in the array spns over addr 0 - 7 . 2nd element will be 8 - 15

=> Prpperties of Array :- 

Two types
- Static Arrays (Fixed size. Need to know the max size before hand)
- Dynamic Arrays (Can grow during the runtime of the program)

=> Time complexity :-

Read   - O(1) (any pos)
Write  - O(1) (any pos)
Delete - O(1) (deletion from last)
Insert - O(n) (insert in middle)
```

## Stack :

```
A data structure that has three operations, Implemets LIFO / FILO (Last in first out/ First in last out)
1. push - O(1)
2. pop  - O(1)
3. peek - O(1)

Generally implemented throught dynamic arrays.
```

## Linked List :

```
Two parts : value + pointer (to a Next Node)

=> Time complexity :-
All operations are O(1) like Insert, Delete, Read, Write.
The issue is To perform any of these operations on an arbitrary node to which we dont have a pointer too is going to take O(n).
Except for Nodes to which we have pointers, all other nodes will take O(n) time.

Time complexity remains the same for doubly linked list.
```

## Queues :

```
A data structure that has two operations, Implemets FIFO (First in first out)
1. enqueue - O(1)
2. dequeue - O(1)

Generally implemented throught linked list.
```