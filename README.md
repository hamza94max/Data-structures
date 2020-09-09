# Data-stracture
data stracture in Java

<div class="container">
	<div class="Array">## Array

• Arrays give us the ability to:
- Store a (potentially large) collection of homogeneous data 
- Have direct access to any one element in the collection by its position 





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
newitems [i]=cars[i];}

</div>
	<div class="block"></div>
	<div class="block"></div>
	<div class="block"></div>
	<div class="block"></div>
</div>


