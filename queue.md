# **Introduction**
#### A queue a Data sructure operation that follows a particular order. The that a queue follow is know as First In First out (FIFO). This simply means that in this operation the first data or request to come in will be the first to go out or taken care of respectively. A good and common example of this is cutomers in a queue. The first customer to come in, will be the first to be served.
#### If you have worked with stack, I guess by now you can tell that this sounds a lot like stack. The major difference is that stack uses a method of operation know as First In Last out(FILO). This means that in stacks, the first data that goes in, will be the last to come out.
Before we dive in into what we have for stack, there are few important terms that you have to familiarize yourself with.

**Enqueue:** Adds an item to the queue. If the queue is full, then it is said to be an Overflow condition. \
**Dequeue:** Removes an item from the queue. The items are popped in the same order in which they are pushed. If the queue is empty, then it is said to be an Underflow condition. \
**Front/Head:** Get the front item from queue. \
**Rear/Tail:** Get the last item from queue.  
\
**The picture below will help you understand Queue.**

![Picture](Queue.png)
 
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