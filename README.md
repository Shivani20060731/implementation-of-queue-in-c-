# implementation-of-queue-in-c-
Implementation of Queue in C++


Aim

To study and implement the Queue data structure in C++ using arrays.

Software Required


Online C++ Compiler

Theory

Concept of Queue

A Queue is a linear data structure that follows the FIFO (First-In-First-Out) principle. This means that the element inserted first will be removed first, much like a real-world queue (line) at a ticket counter.

Insertion (Enqueue): New elements are added at the rear (end) of the queue.

Deletion (Dequeue): Elements are removed from the front (start) of the queue.

Linear Queue Using Array

In this program, the queue is implemented using a static array of size SIZE = 5. Two variables start and end are used to keep track of the front and rear of the queue.

Initialization

start = -1, end = -1 represent an empty queue.


Enqueue Operation (Insertion)

1. If end == SIZE - 1, the queue is full (overflow).


2. If the queue is empty (start == -1), set start = 0.


3. Increment end and insert the new element at position end.

Dequeue Operation (Deletion)

1. If start == -1 or start > end, the queue is empty (underflow).


2. Otherwise, remove the element at start and increment start.

Display Function

If the queue is empty, print "Queue is empty".

Otherwise, traverse from start to end and display all elements.

Advantages of Linear Queue (Array-based)

Simple and easy to implement.

Efficient for small, fixed-size applications.


Limitations

Fixed Size: The maximum number of elements is limited by array size.

Wasted Space: Once elements are dequeued, that space cannot be reused unless a circular queue is implemented.


This makes the linear queue suitable for basic learning, but in practical applications, dynamic queues or circular queues are preferred.


Algorithm

Stepwise Algorithm for Linear Queue (Array Implementation):

1. Start


2. Initialize start = -1, end = -1, and declare an array queue[SIZE].


3. Enqueue(x):

If end == SIZE - 1 → print "Queue Overflow".

Else if start == -1 → set start = 0.

Increment end and set queue[end] = x.

4. Dequeue():

If start == -1 or start > end → print "Queue Underflow".

Else remove queue[start] and increment start.
5. Display():

If start == -1 → print "Queue is empty".

Else print elements from queue[start] to queue[end].



6. In main(), perform a series of enqueue, dequeue, and display operations.


7. Stop


Conclusion

The array-based implementation of a Linear Queue demonstrates the fundamental working of queues:

Insertion (enqueue) happens at the rear,

Deletion (dequeue) happens at the front.


By maintaining two pointers (start and end), the program effectively manages queue operations while handling overflow and underflow conditions.
