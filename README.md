# Data-stracture
data stracture in Java

<details open>
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



<details open>
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

<details open>
<summary>LinkedList</summary>
<br>
is a data structure wherein each element contains both  a data value and a pointer to next element in the list<br><br>
  
  <img src = "https://user-images.githubusercontent.com/54688005/93020778-56bd9a80-f5df-11ea-9327-bb0dae8f6ee6.PNG" width =50%>
  <img width ="5%"/> 
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






