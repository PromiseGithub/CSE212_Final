# **Introduction**
#### This type of data structure is like a liknked  list in terms of connecting with each other with pointers. The difference is that in Trees, a node can connect to multiple different nodes. The connecting lines or pointers in Trees are called edge(s). Other unique fetures of this data structure is the components that it's made of. These includes
* Subtree
* Root Node
* Parent Node
* Child Node
* Leaf Node

Before we dive in into what we have for Trees, there are few important terms that you have to familiarize yourself with.

**Subtree:** This comsist of a node that serves as a root to other nodes while being attached to a bigger tree. As the name implies, this is a tree in a tree. \
**Node:** . \
**Front/Head:** Get the front item from queue. \
**Rear/Tail:** Get the last item from queue.  
\
**The picture below will help you understand Queue.**

![Picture](tree.png)
<div align="center">Image source: <a href="https://www.geeksforgeeks.org/introduction-to-tree-data-structure-and-algorithm-tutorials/">Geeksforgeeks</a></div>
 
## **Performance**
There are few sets of operations that you can perfrom in Queue. Each of them has a time that it will take them to run, which is also called a run time.

**enqueue(value):** This operation Adds "value" to the back of the queue. You can perform this operation with the following command; my_queue.append(value). Performance of adding to the end of the dynamic array is O(1).

**deenqueue():** This operation removes the very first value from a queue. It would have being an O(1) opertion because we are removing the very first value that we know the position. However, this is an O(n) because every value behind the one that we removed will have to take one step forward. And we usually do not know the entire value before the operation.

## **Use Cases**
As already explained, queue works on FIFO strategy. The two situtation where we can think of the real life application of this:
1. Ticket windows or oulets. When people buy event tickets, the person who comes first gets the first ticket while the peron who comes last get the last ticket.
2. Another good example of real life application of queue is the toll-gates. The vehicle that gets to the toll-gate first, get to leave the toll-gate first.
## **Two Problem to Solve**
Using the above two use cases, solve the following problem
1. I got to a ticket both to buy a ticket. Check to see if there is some before me. If there is serve the very first person and check again if there is some one before me. Continue until there is no one left before me, then serve me.
2. I drove up to a toll-gate, check if I am the first to get there. If I am, let me through, otherwise, have me wait. 