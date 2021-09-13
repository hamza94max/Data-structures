# Data Structures 

### Data Structures in Java<br>
A **data structure** is a data organization, management, and storage format that enables efficient access and modification<br><br>
<img src = "https://user-images.githubusercontent.com/54688005/93380732-ec675d00-f85f-11ea-9669-63765174f253.jpg" width =60%>
  <img width ="10%"/> 
  <br><br><br>
  
 
  
<details close>
<summary>Array</summary>
<br>
• Arrays give us the ability to:
- Store a (potentially large) collection of homogeneous data 
- Have direct access to any one element in the collection by its position <br>


**Syntax**
type[] array_name = new type[length];  <br/>  <br/> 
<img src = "https://user-images.githubusercontent.com/54688005/92636834-499b6580-f2d8-11ea-859f-5c13d50db502.PNG" width =55%>
  <img width ="5%"/> 

**Access the Elements of an Array**
> String[] cars = {"Volvo", "BMW", "Ford", "Mazda"}; <br/> 
 System.out.println(cars[0]);<br/>
// Outputs Volvo


**Change an Array Element**

> String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};<br/>
 cars[0] = "Opel";<br/>
 System.out.println(cars[0]);<br/>
// Now outputs Opel instead of Volvo

**Array Length**
To find out how many elements an array has, use the length property:<br/>
> String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};<br/>
System.out.println(cars.length);<br/>
// Outputs 4<br/>

**loop to print all elements in Array**
>String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};<br/>
for (int i = 0; i < cars.length; i++) {<br/>
  System.out.println(cars[i]);}
  
  
  **Resize the size of array** 
 when you reach capacity, resize to double the size
> int count =cars.length;<br/>
String [] newitems =new String [count*2];<br/>
//copy the elements to new array <br/>
for (int i=0;i<count;i++){<br/>
newitems [i]=cars[i];}<br/><br/>

<img src = "https://user-images.githubusercontent.com/54688005/104125479-a464cc80-535f-11eb-9248-416f69348321.jpg" width =50%>
  <img width ="10%"/> 
  <br>





 **Time**<br/>
- O(1) to add/remove at end (amortized for allocations for more space), index, or update<br/>
- O(n) to insert/remove elsewhere<br/>

 **Space**<br/>
- contiguous in memory, so proximity helps performance<br/>
- space needed = (array capacity, which is >= n) * size of item, but even if 2n, still O(n)<br/>


**resources**
1. [Arrays (Video](https://www.coursera.org/lecture/data-structures/arrays-OsBSF)
2. [ Array funcations](https://archive.org/details/0102WhatYouShouldKnow/03_01-resizableArrays.mp4)
3. [Dynamic Arrays (resize array)](https://www.coursera.org/lecture/data-structures/dynamic-arrays-EwbnV)

</details>



<details close>
  
  
<summary>2D Array</summary>
 <br/>
A multidimensional array is an array of arrays. Each element of a multidimensional array is an array itself. For example <br/>
  
  >  int[][] a = new int[3][4];<br/><br/>
  
 <img src = "https://user-images.githubusercontent.com/54688005/93002312-69c86000-f536-11ea-9ac8-57681ba2fff4.PNG" width =40%>
  <img width ="5%"/> 
  
  **Loop to print 2D array**<br/>
>int[][] board = new int[3][3];<br/>
for (int i = 0; i < board.length; i++) {<br/>
for (int j = 0; j < board[i].length; j++) {<br/>
board[i][j] = i + j; } }<br/>


**Resources**<br/>
[2D Array](https://archive.org/details/0102WhatYouShouldKnow/02_05-multidimensionalArrays.mp4)<br/>
</details>

<details close>
<summary>LinkedList</summary>
<br>
is a data structure wherein each element contains both  a data value and a pointer to next element in the list<br><br>
  
  
  Linked lists accommodate items of varying sizes and allow easy insertion
and deletion of items.<br>
  One potential disadvantage of using a list is that
performance for retrieving a specified item in a list of size n is linear — **O(n)**,
as it requires potentially traversing all n elements in the worst case.<br><br>
  
  ### **Lists are sometimes used directly by kernel algorithms**
  
  
  
  <img src = "https://user-images.githubusercontent.com/54688005/93519501-a7f6c280-f92e-11ea-9772-8f414ce997a7.PNG" width =75%>
  <img width ="10%"/> 
  <br>
  
  **Array V.S Linkedlist** 
  1) Size of the array is fixed **v.s** Linked list allows dynamic memory allocation   <br>
  2) Array elements need contiguous memory locations to store their values **v.s** Linked list elements don’t need contiguous memory locations  <br>
  3) Inserting an element in an array is performance wise expensive **v.s**  Insert and delete operations in the Linked list are not performance wise expensive because adding      and deleting an element from the linked list does’t require element shifting, only the pointer of the previous and the next node requires change.  <br>
  
  
  
  
  
  
  **Funcations**
> LinkedList<String> al=new LinkedList<String>();  <br>
  al.add("Ravi");  <br>
  al.addFirst("First Item");<br>
  al.getFirst();<br>
  al.getLast();<br>
  al.addLast("Last Item");<br>
  al.removeFirst();<br>
  al.removeLast();<br>
  al.remove(2);<br>
  al.get(2);<br>
  al.size();<br>
  // clear the list<br>
  llist.clear();<br>
  // clone al ( returns the exact same copy of the Linked List object )<br>
  list2 = (LinkedList) al.clone();<br>
  
  
   **Time**<br/>
- **O(1)** to add/remove at end (amortized for allocations for more space), index, or update<br/>
- **O(n)** to insert/remove elsewhere<br/>

 **Space**<br/>
- The amount of data stored increases linearly with the number of nodes in the list. Therefore, the space complexity of the linked list is linear:  **O(n)**
 
  
  
  **Resources**
- [Website ](https://beginnersbook.com/2013/12/linkedlist-in-java-with-example/)
- [Video ](https://archive.org/details/ucberkeley_webcast_htzJdKoEmO0)
- [Lists vs. Arrays](https://www.coursera.org/learn/data-structures-optimizing-performance/lecture/QUaUd/in-the-real-world-lists-vs-arrays)
- [Why you should avoid Linked Lists](https://www.youtube.com/watch?v=YQs6IC-vgmo)

</details>

<details close>
<summary>Stack</summary>
 <br/>
  
  A **Stack** is a sequentially ordered data structure that uses the last in, first
out (LIFO) principle for adding and removing items, meaning that the last item
placed onto a stack is the first item removed. The operations for inserting and
removing items from a stack are known as push and pop, respectively.
  
 ### operating system often uses a stack when invoking function calls.<br>
  
  Parameters,local variables, and the return address are pushed onto the stack when a
function is called; returning from the function call pops those items off the
stack.
  
  
  
 <img src = "https://user-images.githubusercontent.com/54688005/93125319-3f5bdb80-f6cb-11ea-868b-a57b1c4556c2.jpg" width =50%>
  <img width ="8%"/> <br/> <br/>


**Creating a Stack**
> Stack <Type> stacks = new Stack<>();<br/>

**example**<br/>
>       Stack <String> animals= new Stack<>();
        animals.push("Dog");
        animals.push("Horse");
        System.out.println("Stack: " + animals);
_**When we push an element into the stack the top is increased by 1.**_ <br/><br/>
  
   <img src = "https://user-images.githubusercontent.com/54688005/93127817-dece9d80-f6ce-11ea-8522-edfed130477f.PNG" width =40%>
  <img width ="5%"/> <br/> <br/>
  
  
  
  
**other Funcations**
>
**empty()**	The method checks the stack is empty or not.<br/>
**push(E item)** The method pushes (insert) an element onto the top of the stack.<br/>
**pop()**	The method removes an element from the top of the stack and returns the same element as the value of that function.<br/>
**peek()**	The method looks at the top element of the stack without removing it.<br/>
**search(Object o)**	The method searches the specified object and returns the position of the object<br/>
**size()** to get the size of the Stack <br/>

**Resources**<br/>
- [Stacks (Last In First Out)](https://archive.org/details/0102WhatYouShouldKnow/05_01-usingStacksForLast-inFirst-out.mp4)<br/>
- [Stacks](https://www.coursera.org/lecture/data-structures/stacks-UdKzQ)





</details>

<details close>
<summary>Queue </summary>
 <br/> <br/>
  
 **Queue** is a data structure which follows the principle of **FIFO** (First-In-First-Out) <br/>
  items are removed from a queue in the order
in which they were inserted. There are many everyday examples of queues,
including shoppers waiting in a checkout line at a store and cars waiting in line
at a traffic signal. Queues are also quite common in operating systems—jobs
that are sent to a printer are typically printed in the order in which they were
submitted, for example<br/> <br/>
  
  **tasks that are waiting to be run on an available CPU are often organized in queues.**
  <br/><br/><br/>
  
  
  
  
  
  
   <img src = "https://user-images.githubusercontent.com/54688005/93380962-4831e600-f860-11ea-833b-9e551dddf44d.PNG" width =45%>
  <img width ="5%"/> <br/> <br/>
  
**FRONT** track the first element of the queue<br/>
**REAR** track the last elements of the queue<br/>
_**initially, set value of FRONT and REAR to -1**_ <br/><br/>
  
  **Funcations**<br/>
- **Enqueue()**: Add an element to the end of the queue _(increase the REAR index by 1)_
- **Dequeue()**: Remove an element from the front of the queue _(increase the FRONT index by 1)_
- **IsEmpty()**: Check if the queue is empty
- **IsFull()**: Check if the queue is full
- **Peek()**: Get the value of the front of the queue without removing it<br/><br/>
  
  
  
**Complexity Analysis**<br/>
The complexity of enqueue and dequeue operations in a queue using an array is ***O(1)**.<br/>
a bad implementation using linked list where you enqueue at head and dequeue at tail would be O(n) because you'd need the next to last element, causing a full traversal each dequeue<br/><br/>

**Applications of Queue**
-  Serving requests on a single shared resource, like a printer, CPU task scheduling etc.
-  In real life scenario, Call Center phone systems uses Queues to hold people calling them in an order, until a service representative is free.<br/><br/>
  

**Resources**<br/>
[Queue (video)](https://www.coursera.org/lecture/data-structures/queues-EShpq)<br/>
[FIFO in Queue](https://archive.org/details/0102WhatYouShouldKnow/05_03-usingQueuesForFirst-inFirst-out.mp4)<br/>
[Website](https://www.programiz.com/dsa/queue)<br/>
 [Code Resources](https://www.softwaretestinghelp.com/java-queue-interface/)<br/>

  
  
  </details>




<details close>
<summary>Hash table </summary>
 <br/>
  
  **Hashtable** is a combination of an array and linkedlist inside of it .
  Called Dictionary in Python<br/>
  
A **hash function** takes data as its input, performs a numeric operation on this
data, and returns a numeric value. This numeric value can then be used as an
index into a table (typically an array) to quickly retrieve the data. <br/><br/><br/>
  
  **Because of this performance, hash functions are used extensively in
operating systems.**<br/>




 <img src = "https://user-images.githubusercontent.com/54688005/93521481-6a933480-f930-11ea-8907-9a088b883fac.PNG" width =85%>
  <img width ="10%"/> <br/> <br/>
  
  
  
  ### One potential difficulty with hash functions is that two inputs can result in the same output value—that is, they can link to the same table location. We can accommodate this hash collision by having a linked list at that table location that contains all of the items with the same hash value. Of course, the more collisions there are, the less efficient the hash function is.<br/><br/>
  
  
  

- The Hash Function should be such that the keys generated are uniformly distributed.
- The size of the Hash Table is dependent on the Hash Function. So, the choice of Hash Function should be done perfectly.
- In the case of a collision in the Hash Table, apply proper collision handling technique.
 
 

>Hashtable<Integer, String> hashtable = new Hashtable<>();<br/>
        //2. Add mappings to hashtable <br/>
        hashtable.put(1,  "A");<br/>
        hashtable.put(2,  "B" );<br/>
        hashtable.put(3,  "C");<br/>
        System.out.println(hashtable);<br/>
        //output <br/>
        {3=C, 2=B, 1=A}<br/>






**Methods**
- **Object put(Object key, Object value) :** It maps the specified key to the specified value in this hashtable. Neither the key nor the value can be null.
- **Object remove(Object key) :** It removes the key (and its corresponding value) from hashtable.
- **boolean containsValue(Object value) :** It returns true if specified value exist within the hash table for any pair, else return false.
- **void clear()** : It is used to remove all pairs in the hashtable.
- **Object get(Object key) :** It returns the value to which the specified key is mapped. Returns null if no such key is found.
- **void rehash() :** It is used to increase the size of the hash table and rehashes all of its keys.
- **int size() :** It returns the number of entries in the hash table.




**Time** <br/>
The Hash Table will perform the insertion, deletion, and searching operation in **O(1)** time.<br/>
  searching for a data item through a list of size n can require up to **O(n)**
comparisons in the worst case<br/>

  
**Resources** <br/>
[Hash tables (CS50) ](https://www.youtube.com/watch?v=nvzVHwrrub0) <br/>
[CS 50 lecture](https://www.youtube.com/watch?v=4IrUAqYKjIA&list=PLhQjrBD2T381L3iZyDTxRwOBuUt6m1FnW&index=6&t=4702s) <br/>








 </details>
 
 

<details close>
<summary>Tree </summary>
 <br/>
  
A **tree** is a data structure that can be used to represent data hierarchically. Data
values in a tree structure are linked through parent–child relationships. <br/>
  
  
  
  In a binary tree, a parent **may have at most two children**, which we term the left child
and the right child<br/>
  
  additionally requires an ordering between the parent’s two children in which lef t child <= right child.<br/>
                                                                                                  
   **Linux uses a balanced binary search tree as part its CPU-scheduling algorithm.**
  
   
 <img src = "https://user-images.githubusercontent.com/54688005/125168657-d4721880-e1a6-11eb-94d7-9e98f05383cb.PNG" width =35%>
  <img width ="8%"/> <br/> <br/> 

  
  
  
  
 <img src = "https://user-images.githubusercontent.com/54688005/94467951-f70ce500-01c3-11eb-88e8-52b5028c7ae4.PNG" width =70%>
  <img width ="8%"/> <br/> <br/>
  
  
- **Root**:  Root is the node that is present at the top of the tree. There can be only one root of a particular tree.
- **Parent**:  All the nodes having at least one child is called the parent node.
- **Child**:  The node below the parent node is called the child node of the parent node.
- **Leaf**:  The node having zero children is called the leaf node.
  
  
  
 ## **Time**<br/>
  When we search for an item in a binary search tree, the worst-case performance is **O(n)**


**Resources**<br/>
[ Introduction To Trees ( Arabic )](https://www.youtube.com/watch?v=XDDZNL-yG2U)


 </details>

  
  
  <details close>
<summary> Graph</summary>
 <br/>
  What is a graph? <br/>
A graph models a set of connections. For 
example, suppose you and your friends are 
playing poker, and you want to model who owes 
whom money. Here’s how you could say, “Alex 
owes Rama money.” <br/><br/>
  
  
   <img src = "https://user-images.githubusercontent.com/54688005/132846337-b736c969-99f8-4e3a-bcd6-bd56cddad201.PNG" width = 45%>
  <img width ="7%"/> <br/> <br/>
  
  **That’s all there is to it! Graphs are made up of nodes and edges. A node can be directly connected to many other nodes.**
  
  Vertex: Vertices are the point that joints edges. It represents the data. It is also known as a node. It is denoted by a circle and it must be labeled. To construct a graph there must be at least a node. For example, house, bus stop, etc.
  
  Edge: An edge is a line that connects two vertices. It represents the relation between the vertices. Edges are denoted by a line. For example, a path to the bus stop from your house.
  
  
  **resources**
1. [Graph](https://www.javatpoint.com/java-graph)

  
  
  
   </details>
  
  

  
  


  
 <img src = "https://user-images.githubusercontent.com/54688005/114392321-e4bf2b00-9b98-11eb-8daa-ab95a7522dd6.PNG" width =85%>
  <img width ="100%"/> <br/> <br/>






## Books 
- [Grokking Algorithms ](https://github.com/camoverride/lit/blob/master/Grokking-Algorithms.pdf)




## Courses
- [CS 50 (Course)](https://www.youtube.com/watch?v=4IrUAqYKjIA&list=PLhQjrBD2T381L3iZyDTxRwOBuUt6m1FnW&t=0s)
- [Blog (MindOrks)](https://blog.mindorks.com/android-developer-should-know-these-data-structures-for-next-interview)
- [Data stracture (Coursera)](https://www.coursera.org/learn/data-structures)
- [Data Structures and Performance (Course)](https://www.coursera.org/learn/data-structures-optimizing-performance)
- [Data Structures in java (Article)](https://www.linkedin.com/pulse/data-structures-java-omar-ismail/)








