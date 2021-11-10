# Stacks and Queues

**A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.**

||||
|---|----|----|
|FILO|First In Last Out|The first item added in the stack will be the last item popped out of the stack.|
|LIFO|Last In First Out|The last item added to the stack will be the first item popped out of the stack|
|Stack Visualization|The topmost item is denoted as the top|||
|Push O(1)|Pushing a Node onto a stack will always be an O(1) operation|
|Pop O(1)|Popping a Node off a stack is the action of removing a Node from the top. |
|Peek O(1)|When conducting a peek, you will only be inspecting the top Node of the stack.|
|IsEmpty O(1)||
|FIFO|First In First Out|The first item in the queue will be the first item out of the queue.|
|LILO|Last In Last Out| the last item in the queue will be the last item out of the queue.|
|Queue Visualization||
|Enqueue O(1)||
|Dequeue O(1)||
|Peek O(1)||
|IsEmpty O(1)||
***Stack Visualization***
![Stack Visualization](https://miro.medium.com/max/554/1*HgSDnflZkAjg9aXD5Fq9ZA.jpeg)


***What is a Queue***

Common terminology for a queue is

* Enqueue - Nodes or items that are added to the queue.
* Dequeue - Nodes or items that are removed from the queue. If called when the * queue is empty an exception will be raised.
* Front - This is the front/first Node of the queue.
* Rear - This is the rear/last Node of the queue.
* Peek - When you peek you will view the value of the front Node in the queue. * If called when the queue is empty an exception will be raised.
* IsEmpty - returns true when queue is empty otherwise returns false.

**[READ MORE](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)**


![Stacks and Queues](https://media.geeksforgeeks.org/wp-content/cdn-uploads/Stack-Queue.png)



Difference between Stack and Queue Data Structures

|Stacks	|Queues|
|-------|---|
Stacks are based on the LIFO principle, i.e., the element inserted at the last, is the first element to come out of the list.	|Queues are based on the FIFO principle, i.e., the element inserted at the first, is the first element to come out of the list.
Insertion and deletion in stacks takes place only from one end of the list called the top.|	Insertion and deletion in queues takes place from the opposite ends of the list. The insertion takes place at the rear of the list and the deletion takes place from the front of the list.
Insert operation is called push operation.|	Insert operation is called enqueue operation.
Delete operation is called pop operation.	|Delete operation is called dequeue operation.
In stacks we maintain only one pointer to access the list, called the top, which always points to the last element present in the list.	|In queues we maintain two pointers to access the list. The front pointer always points to the first element inserted in the list and is still present, and the rear pointer always points to the last inserted element.
Stack is used in solving problems works on recursion.|	Queue is used in solving problems having sequential processing.

 #### &copy; Dima Alabsi; 202
 
 
