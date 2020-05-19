# WeekEleven

There are 6 Data Types, which can be devided into 3 main categories.

Stack
Stack is a linear data structure that uses addition or removal of an element
follows a specific order(Last in, First out).

<!-- stack() //create an empty stack
boolean isEmpty() //check if the stack is empty
void push(item, item) //Push an item onto the stack
item pop() //return and remove the item that was inserted most recently
int size() //Number of items on stack -->



Queue
Queues can be used in JS with Arrays, by using the push or unshift functions to add elements, and using the shift and pop functions to remove them. Queues aren't very efficent in large queues as the shift and unshift 
functions move every item in the array.
 
<!-- class Queue //Queue class 
{ 
    // Array is used to implement a Queue 
    constructor() 
    { 
        this.items = []; 
    } 
                  
    // Functions to be implemented 
    // enqueue(item) 
    // dequeue() 
    // front() 
    // isEmpty() 
    // printQueue() 
}  -->



Linked Lists
Like arrays, Linked Lists store data elements in sequential order. They start at the 'Head' node, and chains down each node until it hits the 'tail' node. Every node points to the next node.

<!-- class LinkedList {
    constructor() {
        this.head = null;
        this.tail = null;
    }

    addToHead(value) {
        const node = new Node(value, null, this.head);
        if (this.head) this.head.next = node;
        else this.tail = node;
        this.head = node;
    } -->


Tree
A Tree is like a linked list, each node can have no more than one 'parent'. The 'DOM' structure, uses a root HTML node that branches into the head and body nodes, which further subdevide into all the familiar HTML tags.

<!-- const tree = new Tree(5);
for (const value of [3, 6, 1, 7, 8, 4, 10, 2, 9]) tree.insert(value); -->



Graph
If a 'Tree' is free to have more than one parent, it becomes a 'Graph'



Hash Tables
A hash table is a dictionary-like structure that pairs keys to values.
----------------------------------------------------------------------------
LINKED LISTS

Introduction to Linked Lists, 
Like arrays, Linked Lists store data elements in sequential order. They 
start at the 'Head' node, and chains down each node until it hits the 
'tail' node. Every node points to the next node.

Of course Linked Lists come with their advantages and disadvantages, some of these being:

ADVANTAGES, 
They are a dynamic data structure, which means you don't need to give an intial size of a linked list.
Insertion and deletion of nodes is a lot easier, as you just have to update 
the address present in the next pointer.
The is no memory wasted as comapired to an array, as memory is allocated only when required.

DISADVANTAGES,
More memory is required to store elements in linked list compaired to an array, as each node requires a pointer, it uses more memory.
The time required to access a node is longer, because you cant randomly access any element as you can in arrays by using an index.

A Real-World example of Linked Lists would be a Train. Each coach is connected to its previous and next coach. In terms of programming, each coach would be a node value and the connectors of the trains would be pointers to the next node.

Below is an example of a Linked List pseudocode.
<!-- // linkedlist class 
class LinkedList { 
    constructor() 
    { 
        this.head = null; 
        this.size = 0; 
    } 
  
    // functions to be implemented 
    // add(element) 
    // insertAt(element, location) 
    // removeFrom(location) 
    // removeElement(element) 
  
    // Helper Methods 
    // isEmpty 
    // size_Of_List 
    // PrintList
}  -->
----------------------------------------------------------------------------
RECURSIVE

Introduction to JS Recursive,
Recursive is a technique for iterating over an operation by having a function call itself repeatedly until it arrives at a result. Most loops can be rewritten in recursive style.

There are advantages and disadvantages of using Recursive, some of these are:

ADVANTAGES,
Once learnt they can reduce a lot of time in certain situations. Using Recursives keywords rather than other functions and keywords in JavaScript can reduce a lot of time.
Recursive adds clarity and reduces the time needed to write and debug code, if you were going to write a small code, it is a good way to 'de-clutter' your code.


DISADVANTAGES,
Recursive uses more memory, because the function has to add a stack with each recursive call and keeps the values there until the call is finished.
If Recursive is not implemented correctly it can be much slower than iteration.

What can recursive be used for? 
While it can be used in many situations, it is most effective for solving problems involving iterative branching, such as fractal math, sorting, or traversing the nodes of complex or non-linear data structures.


A real-world example of Recursive would be, there are lots of mathy examples here, but you wanted a real world example, so with a bit of thinking, this is possibly the best I can offer:

You find a person who has contracted a given contageous infection, which is non fatal, and fixes itself quickly( Type A) , Except for one in 5 people ( We'll call these type B ) who become permanently infected with it and shows no symptoms and merely acts a spreader.

This creates quite annoying waves of havoc when ever type B infects a multitude of type A.

Your task is to track down all the type Bs and immunise them to stop the backbone of the disease. Unfortunately tho, you cant administer a nationwide cure to all, because the people who are typeAs are also deadly allergic to the cure that works for type B.

The way you would do this, would be social discovery, given an infected person(Type A), choose all their contacts in the last week, marking each contact on a heap. When you test a person is infected, add them to the "follow up" queue. When a person is a type B, add them to the "follow up" at the head ( because you want to stop this fast ).

After processing a given person, select the person from the front of the queue and apply immunization if needed. Get all their contacts previously unvisited, and then test to see if they're infected.

Repeat until the queue of infected people becomes 0, and then wait for another outbreak..

A recursive pseudo code is,  

<!-- function countDown(fromNumber) {
    console.log(fromNumber);

    let nextNumber = fromNumber - 1;

    if (nextNumber > 0) {
        countDown(nextNumber);
    }
}
countDown(3); -->