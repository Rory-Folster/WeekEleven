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